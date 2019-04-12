# Kafka

## 术语

  - **Broker**：Kafka 集群包含一个或多个服务器，这种服务器被称为 `broker` 。
  - **Topic**：每条发布到 Kafka 集群的消息都有一个类别，这个类别被称为 Topic。（物理上不同 Topic 的消息分开存储，逻辑上一个 Topic 的消息虽然保存于一个或多个 broker 上，但用户只需指定消息的 Topic 即可生产或消费数据而不必关心数据存于何处）。
  - **Partition**： `Partition` 是物理上的概念，每个 `Topic` 包含一个或多个 `Partition` 。
  - **Producer**：负责发布消息到 Kafka broker。
  - **Consumer**：消息消费者，向 Kafka broker 读取消息的客户端。
  - **Consumer Group**：每个 `Consumer` 属于一个特定的 `Consumer Group`（可为每个 Consumer 指定 group name，若不指定 group name 则属于默认的 group）。

## 拓扑结构

![image](images/9a9bab37c896c086e2fee7b3e15a9ae3.png)

如上图所示，一个典型的 `Kafka` 集群中包含若干 `Producer` （可以是web前端产生的Page View，或者是服务器日志，系统CPU、Memory等），若干 `broker` （Kafka支持水平扩展，一般broker数量越多，集群吞吐率越高），若干 `Consumer Group` ，以及一个 `Zookeeper` 集群。 `Kafka` 通过 `Zookeeper` 管理集群配置，选举 `leader` ，以及在 `Consumer Group` 发生变化时进行 rebalance。 `Producer` 使用 push 模式将消息发布到broker，Consumer使用pull模式从broker订阅并消费消息。

## Topic & Partition

**Topic 在逻辑上可以被认为是一个 queue** ，每条消费都必须指定它的 `Topic` ，可以简单理解为必须指明把这条消息放进哪个 `queue` 里。为了使得 Kafka 的吞吐率可以线性提高，**物理上把 `Topic` 分成一个或多个 `Partition`** ，每个 `Partition` 在物理上对应一个文件夹，该文件夹下存储这个 `Partition` 的所有消息和索引文件。若创建 `topic1` 和 `topic2` 两个 `topic` ，且分别有 13 个和 19 个分区，则整个集群上会相应会生成共 32 个文件夹（本文所用集群共8个节点，此处 `topic1` 和 `topic2` `replication-factor` 均为1）。

> Partition 都是通过 顺序读写，所以效率很高

> replication-factor 配置 partition 副本数。配置副本之后,每个 partition 都有一个唯一的 leader ，有 0 个或多个 follower 。所有的读写操作都在 leader 上完成，followers 从 leader 消费消息来复制 message，就跟普通的 consumer 消费消息一样。一般情况下 partition 的数量大于等于 broker 的数量，并且所有 partition 的 leader 均匀分布在 broker 上。

对于传统的 MQ 而言，一般会删除已经被消费的消息，而 Kafka 集群会保留所有的消息，无论其被消费与否。当然，因为磁盘限制，不可能永久保留所有数据（实际上也没必要），因此 Kafka 提供两种策略删除旧数据。一是基于时间，二是基于 Partition 文件大小。

## Producer 消息路由

Producer 发送消息到 broker 时，会根据 Paritition 机制选择将其存储到哪一个 Partition 。如果 Partition 机制设置合理，所有消息可以均匀分布到不同的 Partition 里，这样就实现了负载均衡。如果一个 Topic 对应一个文件，那这个文件所在的机器I/O将会成为这个 Topic 的性能瓶颈，而有了 Partition 后，不同的消息可以并行写入不同 broker 的不同 Partition 里，极大的提高了吞吐率。

可以在 `$KAFKA_HOME/config/server.properties` 中通过配置项 `num.partitions` 来指定新建 `Topic` 的默认 `Partition` 数量，也可在创建 `Topic` 时通过参数指定，同时也可以在 Topic 创建之后通过 Kafka 提供的工具修改。

在发送一条消息时，可以指定这条消息的 `key` ，Producer 根据这个 `key` 和 Partition 机制来判断应该将这条消息发送到哪个 Parition 。Paritition机制可以通过指定 Producer 的 `paritition.class` 这一参数来指定，该 class 必须实现 `kafka.producer.Partitioner` 接口。

## Consumer Group

![image](images/e54deac5512215cfc6801890bb83d792.png)

这是 Kafka 用来实现一个 Topic 消息的广播（发给所有的 Consumer ）和单播（发给某一个 Consumer ）的手段。一个 Topic 可以对应多个 Consumer Group 。如果需要实现广播，只要每个 Consumer 有一个独立的 Group 就可以了。要实现单播只要所有的 Consumer 在同一个 Group 里。用 Consumer Group 还可以将 Consumer 进行自由的分组而不需要多次发送消息到不同的 Topic 。

## Consumer 个数与 Parition 数有什么关系？

**topic 下的一个分区只能被同一个 consumer group 下的一个 consumer 线程来消费**，但反之并不成立，即一个 consumer 线程可以消费多个分区的数据。比如 Kafka 提供的 `ConsoleConsumer` ，默认就只是一个线程来消费所有分区的数据。

> 即分区数决定了同组消费者个数的上限

![image](images/5290a719713da5ce4e83422ded5bdf0c.png)

所以，如果你的分区数是 N ，那么最好线程数也保持为 N ，这样通常能够达到最大的吞吐量。超过 N 的配置只是浪费系统资源，因为多出的线程不会被分配到任何分区。

## Push vs. Pull　　

作为一个消息系统，Kafka 遵循了传统的方式，选择由 Producer 向 broker `push` 消息并由 Consumer 从 broker `pull` 消息。事实上，push 模式和 pull 模式各有优劣。

  - Push模式 很难适应消费速率不同的消费者，因为消息发送速率是由broker决定的。push模式的目标是尽可能以最快速度传递消息，但是这样很容易造成 Consumer 来不及处理消息，典型的表现就是拒绝服务以及网络拥塞。
  - Pull模式 可以根据Consumer的消费能力以适当的速率消费消息。

对于 Kafka 而言，Pull模式 更合适。Pull模式 可简化 broker 的设计，Consumer 可自主控制消费消息的速率，同时 Consumer 可以自己控制消费方式——即可批量消费也可逐条消费，同时还能选择不同的提交方式从而实现不同的传输语义。

## 参考

[Kafka设计解析](http://www.jasongj.com/2015/03/10/KafkaColumn1/)
