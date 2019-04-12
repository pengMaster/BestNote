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

### 本文配套视频

- [什么是XMPP配套视频](https://v.qq.com/x/page/t0394w3zhoa.html)

## 3-简单阐述一下对XMPP协议理解以及优缺点？

### 定义：

> XMPP（可扩展消息处理现场协议）的前身是Jabber，由一个开源组织产生的即时通信协议，基于可扩展标记语言（XML）的一种协议，是由IETF(国际互联网小组)通过的网络标准。

- 及时通讯:发送一则消息，对方账号马上即时接收到消息。中间没有出现延时。
  底层使用 socket实现/java对tcp/ip协议的实现

### 基本网络结构

XMPP中定义了三个角色，客户端，服务器，网关。通信能够在这三者的任意两个之间双向发生。服务器同时承担了客户端信息记录，连接管理和信息的路由功能。网关承担着与异构即时通信系统的互联互通，异构系统可以包括SMS（短信），
MSN，ICQ等。基本的网络形式是单客户端通过TCP/IP连接到单服务器，然后在之上传输XML。

- 举个例子看看所谓的XML（标准通用标记语言的子集）流是什么样子的？

客户端：

```xml
<?xmlversion='1.0'?>
<stream:stream
	to='example_com'
	xmlns='jabber:client'
	xmlns:stream='http_etherx_jabber_org/streams'
	version='1.0'>
```

服务器：

```xml
<?xmlversion='1.0'?>
<stream:stream
	from='example_com'
	id='someid'
	xmlns='jabber:client'
	xmlns:stream='http_etherx_jabber_org/streams'
	version='1.0'>
```

其他通信
客户端：

```xml
<messagefrom='juliet_example_com'
	to='romeo_example_net'
	xml:lang='zh-cn'>
    	<body>Art thou not Romeo, and a Montague?</body>
</message>
```

服务器：

```xml
<message from='romeo_example_net'
	to='juliet_example_com'
	xml:lang='zh-cn'>
    <body>Neither, fair saint, if either thee dislike.</body>
</message>
```

客户端：

```xml
</stream:stream>
```

服务器：

```xml
</stream:stream>
```

- 以文档的观点来看，客户端或服务器发送的所有XML文本连缀在一起，从&lt;stream>到&lt;/stream>构成了一个完整的XML文档。其中的stream标签就是所谓的XML Stream。在&lt;stream>与&lt;/stream>中间的那些&lt;message>...&lt;/message>这样的XML元素就是所谓的XML Stanza（XML节）。 XMPP核心协议通信的基本模式就是先建立一个stream，然后协商一堆安全之类的东西，中间通信过程就是客户端发送XML Stanza，一个接一个的。服务器根据客户端发送的信息以及程序的逻辑，发送XML Stanza给客户端。但是这个过程并不是一问一答的，
  任何时候都有可能从一方发信给另外一方。通信的最后阶段是&lt;/stream>关闭流，关闭TCP/IP连接。

> XMPP 的消息格式。
> XMPP 协议的所有消息都是 XML 格式的，在 XMPP 中定义了 3 个顶层消息：

- 2.1 Presence

  用于确定用户的状态。消息结构举例如下（每个 XML 的 node 还会有很多其他 attribute，为了简单起见这里省略，下同）：

  ```
  <presence from="abc@jabber.org/contact"  to="def@jabber.org/contact"> 
    <status>online</status> 
  </presence>
  ```

- 2.2 Message

  用于在两个用户之间发送消息。消息结构举例如下：

  ```
  <message from="abc@jabber.org/contact" to="def@jabber.org/contact" type=“chat”> 
    <body>hello</body> 
  </message>
  ```

- 2.3 IQ​

  信息/请求，是一个请求－响应机制，管理XMPP服务器上两个用户的转换，允许他们通过相应的XML格式进行查询和响应。

  ```
  <iq from="abc@jabber.org/contact" id=“id11” type=“result”> 
  </iq>
  ```

![img](http://upload-images.jianshu.io/upload_images/4037105-e929a077d630d27e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

[及时聊天的展示形式](https://v.qq.com/x/page/k0394y5jo6d.html)

![img](http://upload-images.jianshu.io/upload_images/4037105-66c1ec0e265257de.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![img](http://upload-images.jianshu.io/upload_images/4037105-9d4319f3ac184fa5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

> 面向连接：三次握手

![img](http://upload-images.jianshu.io/upload_images/4037105-45c525c855b6e407.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 欢迎关注微信公众号,长期推荐技术文章和技术视频

微信公众号名称：Android干货程序员

![img](http://upload-images.jianshu.io/upload_images/4037105-8f737b5104dd0b5d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)