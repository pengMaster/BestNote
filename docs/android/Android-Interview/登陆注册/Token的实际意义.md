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

今天文章比较简单，主要是为了录制面试题系列，保证文章的完整性来帮助那些想找工作的哥们，各位高级程序员请勿拍砖,不过把下面三段视频都看完，多多少少会有些收获。。。

### 本文配套视频：

- [为什么需要token配套视频](https://v.qq.com/x/page/c0395s3jd4f.html)
- [一分钟登录配套视频](https://v.qq.com/x/page/p0395khlfdz.html)
- [一分钟解析登录配套视频](https://v.qq.com/x/page/r03959jvnjm.html)

## 在android开发中，用户登录时，客户端会接收到token值，请描述一下对token的理解？

### Token的引入：

Token是在客户端频繁向服务端请求数据，服务端频繁的去数据库查询用户名和密码并进行对比，判断用户名和密码正确与否，并作出相应提示，在这样的背景下，Token便应运而生。

### Token的定义：

Token是服务端生成的一串字符串，以作客户端进行请求的一个令牌，当第一次登录后，服务器生成一个Token便将此Token返回给客户端，以后客户端只需带上这个Token前来请求数据即可，无需再次带上用户名和密码。

使用Token的目的：
Token的目的是为了验证用户登录情况以及减轻服务器的压力，减少频繁的查询数据库，使服务器更加健壮。

### Token的应用：

1. 当用户首次登录成功之后, 服务器端就会生成一个 token 值，这个值，会在服务器保存token值(保存在数据库中)，再将这个token值返回给客户端
2. 客户端拿到 token 值之后,使用sp进行保存
3. 以后客户端再次发送网络请求(一般不是登录请求)的时候,就会将这个 token 值附带到参数中发送给服务器
4. 服务器接收到客户端的请求之后,会取出token值与保存在本地(数据库)中的token值做对比
5. 如果两个 token 值相同， 说明用户登录成功过!当前用户处于登录状态
6. 如果没有这个 token 值, 没有登录成功
7. 如果 token 值不同: 说明原来的登录信息已经失效,让用户重新登录

### 使用一分钟利用开源中国接口获取登录token

### 利用一分钟时间解析服务器返回的token数据

懒得写文字了，直接看视频吧，看完会有不小的收获哦

## 登录和注销 (Cookie, Session)


* 登陆过程
 1. 先把用户名和密码传给服务器(请求头中没有Cookie)
 2. 服务器验证用户名和密码
 3. 验证通过->响应头中返回(Cookies)一个或多个key=value;key1=value1
 4. 客户端保存这些Cookies到本地文件.

* 请求数据过程
 1. 如果没有Cookie, 只能获取到公共信息.
 2. 把Cookie放到请求头中, 可以获取到Cookie对应的账号的隐私数据.
 3. 如果Cookie超时了(一小时, 一周, 一个月), 服务器同样不返回隐私数据.

* 注销过程
 1. 删除本地的Cookie
 2. 以后的请求头中都没有Cookie
 3. 服务器不会再知道客户端是谁, 会话结束.

- 欢迎关注微信公众号,长期推荐技术文章和技术视频

微信公众号名称：Android干货程序员

![img](http://upload-images.jianshu.io/upload_images/4037105-8f737b5104dd0b5d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)