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

第一：当出现这个错误就是jar包冲突。

![img](http://upload-images.jianshu.io/upload_images/4037105-9147f9c33825f794.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

第二：解决办法，双击Shift搜索，会发现如下图片：

![img](http://upload-images.jianshu.io/upload_images/4037105-01ec162adcd79502.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

搜索你会发现我的项目里面添加了okhttp3.6，bomb里面也添加了okhttp3.3.1，这时候系统就不知道该用哪个jar冲突了。

第三：打开项目的扩展库，如下图展示：

![img](http://upload-images.jianshu.io/upload_images/4037105-d952e4f45f66ce3d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

会发现bomb自带了okhttp的jar包，如图片展示。

![img](http://upload-images.jianshu.io/upload_images/4037105-cee4021279d743d6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

我的项目也再带okhttp的jar包，如图片展示。

![img](http://upload-images.jianshu.io/upload_images/4037105-c05678f43cb13f4d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

第四：找到我的build.gradle文件，去掉刚刚冲突的jar包，如下展示：

```gradle
 //bmob-sdk：Bmob的android sdk包，包含了Bmob的数据存储、文件等服务，以下是最新的bmob-sdk:
   compile ('cn.bmob.android:bmob-sdk:3.5.5'){ // gson-2.6.2
        exclude group: 'com.squareup.okhttp3'
        exclude group: 'com.squareup.okio'
        exclude group: 'com.google.code.gson'
//        exclude(module: 'gson')      // 防止版本冲突
    }

 // 网络加载
    compile ('com.squareup.okhttp3:okhttp:3.6.0'){
        exclude group: 'com.squareup.okhttp3'
        exclude group: 'com.squareup.okio'
    }
```

至此解决冲突。

- 欢迎关注微信公众号,长期推荐技术文章和技术视频
- 微信公众号名称：Android干货程序员

![img](http://upload-images.jianshu.io/upload_images/4037105-8f737b5104dd0b5d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)