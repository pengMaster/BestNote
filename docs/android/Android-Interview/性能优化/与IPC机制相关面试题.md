### 源码分析相关面试题

- [Volley源码分析](http://www.jianshu.com/p/ec3dc92df581)
- [注解框架实现原理](http://www.jianshu.com/p/20da6d6389e1)
- [okhttp3.0源码分析](http://www.jianshu.com/p/9ed2c2f2a52c)
- [onSaveInstanceState源码分析](http://www.jianshu.com/p/cbf9c3557d64)
- [静默安装和源码编译](http://www.jianshu.com/p/2211a5b3c37f)

### Activity相关面试题

- [保存Activity的状态](http://www.jianshu.com/p/cbf9c3557d64)

### 与XMPP相关面试题

- [XMPP协议优缺点](http://www.jianshu.com/p/2c04ac3c526a)
- [极光消息推送原理](http://www.jianshu.com/p/d88dc66908cf)

### 与性能优化相关面试题

- [内存泄漏和内存溢出区别](http://www.jianshu.com/p/5dd645b05c76)
- [UI优化和线程池实现原理](http://www.jianshu.com/p/c22398f8587f)
- [代码优化](http://www.jianshu.com/p/ebd41eab90df)
- [内存性能分析](http://www.jianshu.com/p/2665c31b9c2f)
- [内存泄漏检测](http://www.jianshu.com/p/1514c7804a06)
- [App启动优化](http://www.jianshu.com/p/f0f73fefdd43)
- [与IPC机制相关面试题](http://www.jianshu.com/p/de4793a4c2d0)

### 与登录相关面试题

- [oauth认证协议原理](http://www.jianshu.com/p/2a6ecbf8d49d)
- [token产生的意义](http://www.jianshu.com/p/9b7ce2d6c195)
- [微信扫一扫实现原理](http://www.jianshu.com/p/a9d1f21bd5e0)

### 与开发相关面试题

- [迭代开发的时候如何向前兼容新旧接口](http://www.jianshu.com/p/cbecadec98de)
- [手把手教你如何解决as jar包冲突](http://www.jianshu.com/p/30fdc391289c)
- [context的原理分析](http://www.jianshu.com/p/2706c13a1769)
- [解决ViewPager.setCurrentItem中间很多页面切换方案](http://www.jianshu.com/p/38ab6d856b56)

### 与人事相关面试题

- [人事面试宝典](http://www.jianshu.com/p/d61b553ff8c9)

### 与人事相关面试题

- [人事面试宝典](http://blog.csdn.net/mwq384807683/article/details/71435960)

> 现在三四月份，金三银四最好找工作时间，为方便各位找工作，特意收集100道android各个方面的面试题，并且会一一录制视频分享给大家方便大家找工作，面试题分类如下；

![img](http://upload-images.jianshu.io/upload_images/4037105-4437ab22b7af3cc8.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![img](http://upload-images.jianshu.io/upload_images/4037105-22abf62d3d9f68a5.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![img](http://upload-images.jianshu.io/upload_images/4037105-6838fa267298201a.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![img](http://upload-images.jianshu.io/upload_images/4037105-c8d1161109029383.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 本文配套视频

- [配套视频](https://v.qq.com/x/page/a03916l1n7h.html)
- [配套视频](https://v.qq.com/x/page/m0391pnoyl7.html)
- [配套视频](https://v.qq.com/x/page/t0391b2gjm5.html)
- [配套视频](https://v.qq.com/x/page/v0391vx3ynb.html)
- 欢迎关注微信公众号,长期推荐技术文章和技术视频

![img](http://upload-images.jianshu.io/upload_images/4037105-8f737b5104dd0b5d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 1- Davik进程、linux进程、线程之间的区别？

### Linux进程：

- Linux进程，它有独立的内核堆栈和独立的存储空间，它是操作系统中资源分配和调度的最小单位。
- Linux操作系统会以进程为单位，分配系统资源，给程序进行调度。
- Linux操作系统在执行一个程序时，它会创建一个进程，来执行应用程序，并且伴随着资源的分配和释放。

### Davik进程：

- Dalvik虚拟机运行在Linux操作系统之上。
- Davik进程就是Linux操作系统中的一个进程，属于linux进程
- 每个Android应用程序进程都有一个Dalvik虚拟机实例。这样做得好处是Android应用程序进程之间不会互相影响，也就是说，一个Android应用程序进程的意外终止，不会影响到其他的应用程序进程的正常运行。

### 线程：

- 线程是进程的一个实体，是CPU调度和分派的基本单位,它是比进程更小的能独立运行的基本单位。
- 线程自己基本上不拥有系统资源,在运行时，只需要必不可少的资源(如程序计数器,一组寄存器和栈)。
- 线程与同属一个进程的其他的线程共享进程所拥有的全部资源。

### 三者之间的联系：

- Davik进程就是Linux操作系统的一个进程。
- 线程就是进程的一个实体，线程是进程的一部分。一个进程中可以提供多个线程执行控制。

### 进程和线程的区别：

- 一个程序至少有一个进程,一个进程至少有一个线程.
- 线程的划分尺度小于进程，使得多线程程序的并发性高。
- 进程在执行过程中拥有独立的内存单元，而多个线程共享内存(同属一个进程)，从而极大地提高了程序的运行效率。
- 每个独立的进程有一个程序运行的入口、顺序执行序列和程序的出口。但是线程不能够独立执行，必须依存在应用程序中，由应用程序提供多个线程执行控制。
- 从逻辑角度来看，多线程的意义在于一个应用程序中，有多个执行部分可以同时执行。但操作系统并没有将多个线程看做多个独立的应用，来实现进程的调度和管理以及资源分配。这就是进程和线程的重要区别。

# 2-Android 中进程与进程之间如何通信？

> aidl机制进程间通信
> AIDL: (Android Interface definition language的缩写)它是一种android内部进程通信接口的描述语言，通过它我们可以定义进程间的通信接口

AIDL进程间通讯的原理：
通过编写aidl文件来定义进程间通信接口。
编译后会自动生成响应的java文件
服务器将接口的具体实现写在Stub中，用iBinder对象传递给客户端，
客户端bindService的时候，用asInterface的形式将iBinder还原成接口，再调用其接口中的方法来实现通信。

### 使用Messenger实现进程间通信

> Messenger是基于AIDL实现的。
> AIDL使服务器可以并行处理，而Messenger封装了AIDL之后只能串行运行，所以Messenger一般用作消息传递。

- 需要大家注意：
- 区别Messenger和Message。
  - Message是消息，承载了要传递的数据。
  - Messenger是信使，可以发送消息。并且Messenger对象可以通过getBinder方法获取一个Ibinder对象。

### Messenger实现原理：

> 服务端（被动方）提供一个Service来处理客户端（主动方）连接，维护一个Handler来创建Messenger，在onBind时返回Messenger的binder。
> 双方用Messenger来发送数据，用Handler来处理数据。Messenger处理数据依靠Handler，所以是串行的，也就是说，Handler接到多个message时，就要排队依次处理。

### 使用Messenger实现进程间通信方法如下：

- 首先A应用提供一个Service，创建一个Messenger对象，在onBinder方法里返回messenger.getBinder()生成的IBinder对象；
  然后在B应用绑定该Service，在ServiceConnection的onServiceConnected方法获取到IBinder对象；
- 最后在B应用使用获取到的binder对象构造出一个新的Messenger对象，使用该Messenger对象的send方法发送的Message数据，都将被Service里的Messenger对象handlerMessage方法接收到。

### 内容提供者ContentProvider实现进程间通信

系统四大组件之一，底层也是Binder实现，主要用来为其他APP提供数据。

> 自定义的ContentProvider为外界进程访问的时候，
> 需要在注册时要提供authorities属性，应用需要访问的时候将属性包装成Uri.parse("content://authorities")。

- 然后实现：
  ContentProvider的中query，delete，insert等相关方法，进行数据的操作。
- 欢迎关注微信公众号,长期推荐技术文章和技术视频

微信公众号名称：Android干货程序员

![img](http://upload-images.jianshu.io/upload_images/4037105-8f737b5104dd0b5d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)