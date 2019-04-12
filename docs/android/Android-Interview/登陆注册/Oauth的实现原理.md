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

- [配套视频](https://v.qq.com/x/page/p03953hoam3.html)

## 腾讯QQ第三方登录的实现原理？

> Oauth当中的角色：

1. Service Provider（服务提供方）

服务提供方通常是网站，在这些网站当中存储着一些受限制的资源，如照片、视频、联系人列表等。这些网站通常使用用户名和密码来确认用户的身份。比如新浪微博的开放平台就是Service Provider。

2. User（用户）

存放在服务提供方的受保护的资源的所有者。用户持有可以登录服务提供者网站的用户名和密码。用户不希望把自己的资源公开，但是用户却需要将这些资源共享给其他网站或应用程序（如用户希望使用第三方开发的新浪微博客户端来访问自己的资源，但又不希望第三方应用知道自己的用户名和密码）。

3. 客户端（Client）

要访问服务提供方资源的第三方应用，可以是web应用程序、桌面应用程序或者是手机应用程序。客户端需要得到授权之后才能访问相应的资源。

> Oauth的认证和授权过程：

1. 用户使用第三方的客户端（如访问第三方的网站，或使用第三方的应用），想对存放在服务提供者的某些资源进行操作
2. 第三方网站或应用向服务提供方请求一个临时令牌（Request Token）
3. 服务提供方验证第三方的身份后，授予其一个临时令牌
4. 第三方获得临时令牌后，将用户引导至服务提供方的授权页面请求用户授权。在这个过程中将临时令牌和客户端的回调连接发送给服务提供者
5. 用户在服务提供者的授权页面上输入自己的用户名和密码，然后授权该客户端访问相应的资源
6. 授权成功后，服务提供方引导用户返回第三方网站的的网页
7. 客户端根据临时令牌从服务提供方那里获取访问令牌（Access Token）
8. 服务提供方根据临时令牌和用户的授权情况授予客户端访问令牌
9. 客户端使用获取的访问令牌访问存放在服务提供方上的相应的资源

Oauth简单示意图

![img](http://upload-images.jianshu.io/upload_images/4037105-b1e90838ef009145.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

Oauth全面的示意图

![img](http://upload-images.jianshu.io/upload_images/4037105-7931074dfb4fa188.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 欢迎关注微信公众号,长期推荐技术文章和技术视频

微信公众号名称：Android干货程序员

![img](http://upload-images.jianshu.io/upload_images/4037105-8f737b5104dd0b5d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)