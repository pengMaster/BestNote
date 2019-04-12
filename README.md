<h1 align="center">Java Android学习/面试指南</h1>

本文并非原创，通过各位博主综合而得，以便供自己方便学习，在此感谢各位前辈，并在下面注明出处

## 目录

- [Android](#Android)
    - [基础](#基础知识)
    - [进阶](#进阶)
    - [Gradle相关](#Gradle相关)
    - [自定义View](#自定义View)
    - [插件化相关](#插件化相关)
    - [热修复相关](#热修复相关)
    - [编译器相关](#编译器相关)
    - [框架源码分析](#框架源码分析)
    - [性能优化](#性能优化)
    - [开源框架](#开源框架)
    - [打包](#打包)    
- [Java](#java)
    - [基础](#基础)
    - [容器](#容器)
    - [并发](#并发)
    - [JVM](#jvm)
    - [I/O](#io)
    - [Java 8](#java-8)
    - [编程规范](#编程规范)   
- [面试指南](#面试指南)
    - [备战面试](#备战面试)
    - [常见面试题总结](#常见面试题总结)
    - [面经](#面经)
    - [Android面试专场](docs/android/AndroidNote/Android-Interview/README.md)
- [网络协议](#网络)
- [操作系统](#操作系统)
    - [Linux相关](#linux相关)
- [数据结构与算法](#数据结构与算法)
    - [数据结构](#数据结构)
    - [算法](#算法)
- [数据库](#数据库)
    - [MySQL](#mysql)
    - [Redis](#redis)
- [系统设计](#系统设计)
    - [设计模式](#设计模式)
    - [常用框架](#常用框架)
    - [数据通信](#数据通信)
    - [网站架构](#网站架构)

- [工具](#工具)
    - [Git](#git)
    - [Docker](#Docker)

- [常见问题](docs/android/README.md)

## Android

### 基础知识

* [Activity详细解析](docs/android/AndroidNote/Android基础/Activity详细解析.md)
* [Service详细解析](docs/android/AndroidNote/Android基础/Service详细解析.md)
* [IntentService详细解析](docs/android/AndroidNote/Android基础/IntentService详细解析.md)
* [IntentService原理解析文章](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=401611665&idx=1&sn=9b6b1f2924d4adfe4e89a322ab53df9c&scene=21#wechat_redirect)
* [ContentProvider实例详解](docs/android/AndroidNote/Android基础/ContentProvider实例详解.md)
* [BroadcastReceiver详细解析](docs/android/AndroidNote/Android基础/BroadcastReceiver详细解析.md)
* [Android异步任务机制之AsycTask](docs/android/AndroidNote/Android基础/Handler,Looper,MessageQueue关系.md)
* [Handler,Looper,MessageQueue关系](docs/android/AndroidNote/Android基础/Activity详细解析.md)
* [Android-SQLite的基本使用](docs/android/AndroidNote/Android基础/Android-SQLite的基本使用.md)
* [Android系统相机与相册的使用](docs/android/AndroidNote/Android基础/Android中相机与相册的详细使用.md)
* [图片缓存原理](docs/android/AndroidNote/Android基础/图片缓存原理.md)
* [Android数据存储的五种方式](docs/android/AndroidNote/Android基础/Android数据存储的五种方式.md)
* [Android跟随手指移动的View](docs/android/AndroidNote/Android基础/Android跟随手指移动的view.md)
* [RecyclerView的使用](docs/android/AndroidNote/Android基础/RecyclerView的简介.md)
* [Android获取SHA1](docs/android/AndroidNote/Android基础/Android获取SHA1.md)
* [Recyclerview和Listview的异同.md](docs/android/AndroidNote/Android进阶/Recyclerview和Listview的异同.md)
* [初识ConstraintLayout](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=2649548068&idx=1&sn=f750ae79c9458f89c3cf85f7573ba579&scene=21#wechat_redirect)
* [TabLayout记录](docs/android/AndroidNote/Android基础/tablayout记录.md)
* [用SpannableString打造绚丽多彩的文本显示效果](http://www.jianshu.com/p/84067ad289d2)
* [解析ConstraintLayout的性能优势](https://mp.weixin.qq.com/s/gGR2itbY7hh9fo61SxaMQQ)
* [Android新特性介绍，ConstraintLayout完全解析](https://blog.csdn.net/guolin_blog/article/details/53122387)
* [Android新特性介绍，ConstraintLayout完全解析](https://blog.csdn.net/guolin_blog/article/details/53122387)
* [Android 一个无限循环滚动的卡片式ViewPager](https://blog.csdn.net/qq_30552993/article/details/76208535)

### 进阶

* [Android 触控事件解析 - Mastering The Android Touch System 笔记](https://www.jianshu.com/p/c65da5e81afd)
* [Android 多进程使用场景](http://blog.csdn.net/qq_27489007/article/details/54377655)
* [Android官网建议代码规范](https://source.android.com/source/code-style#java-language-rules)
* [30多年编码经验总结成10条最佳实践](https://mp.weixin.qq.com/s?__biz=MzIyMjQ0MTU0NA==&mid=2247484524&idx=1&sn=5b2759e6d89f01e61d021545ca7556b9&chksm=e82c3d4bdf5bb45dd77227982931ede8229ee6910829253a57bb905e810c89bd3f0a162786e8&mpshare=1&scene=23&srcid=1023FjKcLWtRlcDpwEeeJnCN#rd)
* [Android中的动画](docs/android/AndroidNote/Android进阶/Android中的动画.md)
* [深入了解MVXX模式](docs/android/AndroidNote/Android进阶/深入了解MVXX模式.md)
* [Android项目总结](docs/android/AndroidNote/Android进阶/Android项目总结.md)
* [Android项目总结2](docs/android/AndroidNote/Android进阶/Android项目总结2.md)
* [自定义RadioGroup](docs/android/AndroidNote/Android进阶/自定义RadioGroup.md)
* [Android导入项目一直在Building的解决方案](docs/android/AndroidNote/Android进阶/AndroidStudio导入工程一直在Building的解决方案.md)
* [基于TOTP的双向认证算法](docs/android/AndroidNote/Android进阶/基于OTP算法的双向认证.md)
* [Android内存泄漏总结.md](docs/android/AndroidNote/Android进阶/Android内存泄漏总结.md)
* [Handler引起的内存泄漏的案例与分析](docs/android/AndroidNote/Android进阶/Handler引起的内存泄漏以及分析.md)
* [Android性能优化.md](docs/android/AndroidNote/Android进阶/Android性能优化.md)
* [LeakCanary的工作过程以及原理](docs/androidAndroidNote/Android性能优化相关/LeakCanary工作过程以及原理.md)
* [AIDL的具体实现流程](http://bbs.51cto.com/thread-1086040-1.html)
* [Android中利用异步来优化处理速度](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=401555104&idx=1&sn=501e6158e6eb26b4e86467be01fd290e&scene=21#wechat_redirect)
* [为什么选择Binder实现Android中跨进程通信](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=2649548116&idx=1&sn=d11a131871623110c74e3676d4fcf785&chksm=f1180e29c66f873f9cac5dc104f97fae319c1831219a9fd9458a4429f16562f6712cc7f65a4c&scene=21#wechat_redirect)
* [三大图片缓存框架的对比](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=2649547344&idx=2&sn=e3fa99b52055a37202634fe61a62d439&scene=21#wechat_redirect)
* [SVG图片在Android中的应用](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=2649548366&idx=1&sn=6cbdf8652ec139859d9be01444e1ad3b&chksm=f1180d33c66f8425a286de4fd5f03aa89308add3593529a91356439cb8c2f8542305561034c8&scene=21#wechat_redirect)
* [携程App的网络性能优化实践](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=2649547359&idx=1&sn=9f069a28f5dbe73fb6c241cfa1049571&scene=21#wechat_redirect)
* [途牛插件化原理](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=2649547401&idx=1&sn=e615735d600f987a7f769f7e278d0840&scene=21#wechat_redirect)
* [Android分包原理](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=2649547390&idx=1&sn=1fae14b1753e437a032640be81c475b8&scene=21#wechat_redirect)
* [插件化实现的思想](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=2649547660&idx=1&sn=d2764b282fdf1c1fdb629f9c2ca9b10f&scene=21#wechat_redirect)
* [Android 7.0新特性总结](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=2649548427&idx=1&sn=df9956d131a6da5f29292cd05a61b16e&chksm=f1180df6c66f84e0097eea33bba6abb125b6bcd6847720a7c481a85001a52ae2e4b1941690eb&scene=21#wechat_redirect)
* [RecyclerView局部刷新的坑](http://blog.csdn.net/jdsjlzx/article/details/52893469)
* [Android单元测试](https://tech.meituan.com/Android_unit_test.html)
* [gradle 详解——你真的了解Gradle吗？](http://blog.csdn.net/u013132758/article/details/52355915)
* [AndroidStudio-Gradle多渠道打包](http://stormzhang.com/devtools/2015/01/15/android-studio-tutorial6/)
* [Android基础入门教程——8.1.1 Android中的13种Drawable小结 Part 1](http://blog.csdn.net/coder_pig/article/details/49006217)
* [Android基础入门教程——8.1.2 Android中的13种Drawable小结 Part 2](http://blog.csdn.net/coder_pig/article/details/49008397)
* [Android-Drawable高级用法](http://blog.csdn.net/lmj623565791/article/details/43752383)
* [安卓开踩过的坑：你的 Bitmap 究竟占多大内存？](http://dev.qq.com/topic/591d61f56793d26660901b4e)
* [Android 4.4 中 WebView 使用注意事项](https://github.com/cundong/blog/blob/master/Android%204.4%20%E4%B8%AD%20WebView%20%E4%BD%BF%E7%94%A8%E6%B3%A8%E6%84%8F%E4%BA%8B%E9%A1%B9.md)
* [Android图像处理 - 高斯模糊的原理及实现](https://mp.weixin.qq.com/s?__biz=MzI2MTU3MTE4NQ==&mid=2247483896&idx=1&sn=50c61e2c78aa610a1944be6a89bd75e5&chksm=ea5916e6dd2e9ff0a62af64c7f345ffb5c6dafdb65847b757b99afcc6fed8e1270e915dbcb25&mpshare=1&scene=23&srcid=1001DxwdQpiMwea74mczpSw8#rd)
* [Android实战——GreenDao3.2的使用，爱不释手](https://mp.weixin.qq.com/s/4Nx2DacsK65O5LanPZUszA)
* [Realm for Android详细教程](http://www.jianshu.com/p/28912c2f31db#)
* [给 Android 开发者的 RxJava 详解](http://gank.io/post/560e15be2dca930e00da1083)
* [Android 谈谈自动化测试](https://mp.weixin.qq.com/s/-0e1wd2iveQPMWgGFcmOwQ)
* [检查app是否具有通知栏权限](docs/android/AndroidNote/Android进阶/检查app是否有推送权限.md)
* [Android中图片压缩分析（上）](https://mp.weixin.qq.com/s/QZ-XTsO7WnNvpnbr3DWQmg)
* [Android Studio3.0更新之路（遇坑必入）](http://www.jianshu.com/p/15afb8234d19)
* [Android Studio3.0正式版填坑路](http://www.jianshu.com/p/9b25087a5d7d)
* [Android混合编程：WebView实践](https://juejin.im/post/59f17a7051882546d71e91a7)
* [runOnUiThread 、Handler.post、View.post之间的区别](https://blog.csdn.net/dengpeng_/article/details/78804404)
* [理解 Activity.runOnUiThread](https://www.jianshu.com/p/e39449026f21)
* [说说 getMainLooper](http://www.icodeyou.com/2015/10/11/2015-10-11-getMainLooper/)
* [Android 探究 LayoutInflater setFactory](https://blog.csdn.net/lmj623565791/article/details/51503977)
* [巧用ViewPager 打造不一样的广告轮播切换效果](https://blog.csdn.net/lmj623565791/article/details/51339751)
* [为RecyclerView打造通用Adapter 让RecyclerView更加好用](https://blog.csdn.net/lmj623565791/article/details/51118836)
* [MNCrashMonitor 监听程序崩溃日志,直接页面展示崩溃日志列表](http://www.wanandroid.com/blog/show/2207)
* [『进阶之路』—— 线程池](http://www.wanandroid.com/blog/show/2264)
* [从json文件到炫酷动画-Lottie实现思路和源码分析](https://www.jianshu.com/p/81be1bf9600c)
* [Lottie动画库 Android 端源码浅析](http://chenhaohui.com/2017/03/13/sd/)

### Gradle相关

* [如何理解 Transform API](https://juejin.im/entry/59776f2bf265da6c4741db2b)
* [Gradle自定义插件详解](https://www.jianshu.com/p/03eb55536298)
* [Android 突破 DEX 文件的 64k方法数限制](http://yifeng.studio/2016/10/26/android-64k-methods-count/)
* [Android Dex分包之旅](http://yydcdut.com/2016/03/20/split-dex/)
* [美团Android DEX自动拆包及动态加载简介](https://tech.meituan.com/mt-android-auto-split-dex.html)
* [gradle简单入门系列](http://www.cnblogs.com/davenkin/p/gradle-learning-1.html)
* [Gradle简单配置](https://mp.weixin.qq.com/s/1UHcYOudViMhpUYeREZzGA)
* [Android 如何编写基于编译时注解的项目](https://blog.csdn.net/lmj623565791/article/details/51931859)
* [Gradle 完整指南（Android）](https://www.jianshu.com/p/9df3c3b6067a)
* [NDK-JNI开发入门教程项目](https://github.com/pengMaster/NDKJniDemo)


### 自定义View

* [自定义View入门](docs/android/AndroidNote/Android自定义View/自定义View入门.md)
* [自定义view详细教程](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=2649547668&idx=1&sn=b2667c46188c6674c90aa72c2fba4719&scene=21#wechat_redirect)
* [自定义ViewGroup入门](docs/android/AndroidNote/Android自定义View/自定义ViewGroup入门.md)
* [Android事件分发机制](docs/android/AndroidNote/Android自定义View/Android事件分发机制.md)
* [CameraView](docs/android/AndroidNote/Android自定义View/自定义View——CameraView.md)
* [CheckView](docs/android/AndroidNote/Android自定义View/自定义View——CheckView.md)
* [CircleView](docs/android/AndroidNote/Android自定义View/自定义View——CircleView.md)
* [FlowLayout](docs/android/AndroidNote/Android自定义View/自定义View——FlowLayout.md)
* [PieView](docs/android/AndroidNote/Android自定义View/自定义View——PieView.md)
* [SlideslipListView](docs/android/AndroidNote/Android自定义View/自定义view——sideslipListView.md)
* [二阶贝塞尔曲线](docs/android/AndroidNote/Android自定义View/二阶贝塞尔曲线.md)
* [三阶贝塞尔曲线](docs/android/AndroidNote/Android自定义View/三阶贝塞尔曲线.md)
* [贝塞尔曲线Demo](https://github.com/linsir6/mCustomView/tree/master/BezierDemo)
* [具有弹性的小球](https://github.com/linsir6/mCustomView/tree/master/MagicCircle)
* [PathMeasure](docs/android/AndroidNote/Android自定义View/PathMeasure.md)


### 热修复相关

* [Android 热修复 Tinker Gradle Plugin解析](https://blog.csdn.net/lmj623565791/article/details/72667669)
* [Android 热修复 Tinker接入及源码浅析](https://blog.csdn.net/lmj623565791/article/details/54882693)
* [Android 热修复 Tinker 源码分析之DexDiff / DexPatch](https://blog.csdn.net/lmj623565791/article/details/60874334)

### 插件化相关

* [滴滴插件化方案 VirtualApk 源码解析](https://blog.csdn.net/lmj623565791/article/details/75000580)


### 编译器相关

* [Android Studio 3.0 新功能解析和旧项目适配](https://mp.weixin.qq.com/s/met0fke7rKumb7Nlb5hxpA)
* [Android-studio使用教程1](docs/android/AndroidNote/Android编译器相关/AndroidStudio使用教程(第一弹).md)
* [Android-studio使用教程2](docs/android/AndroidNote/Android编译器相关/AndroidStudio使用教程(第二弹).md)
* [Android-studio使用教程3](docs/android/AndroidNote/Android编译器相关/AndroidStudio使用教程(第三弹).md)
* [Android-studio使用教程4](docs/android/AndroidNote/Android编译器相关/AndroidStudio使用教程(第四弹).md)
* [Android-studio使用教程5](docs/android/AndroidNote/Android编译器相关/AndroidStudio使用教程(第五弹).md)
* [Android-studio使用教程6](docs/android/AndroidNote/Android编译器相关/AndroidStudio使用教程(第六弹).md)
* [Android-studio使用教程7](docs/android/AndroidNote/Android编译器相关/AndroidStudio使用教程(第七弹).md)


### 性能优化

* [Android开发性能优化总结(一)](http://blog.csdn.net/gs12software/article/details/51173392)
* [Android开发性能优化总结(二)](http://blog.csdn.net/gs12software/article/details/51234454)


### 开源框架

* [当下流行开源框架总览](docs/android/AndroidNote/Android开源框架相关/Android当下最流行的开源框架总结.md)
* [easypermission](docs/android/AndroidNote/Android开源框架相关/动态申请权限库：easypermissions使用与源码解析.md)
* [ButterKnifeZelezny](docs/android/AndroidNote/Android开源框架相关/Android黑科技——ButterKnifeZelezny.md)
* [RxJava+retrofit2](docs/android/AndroidNote/Android开源框架相关/RxJava+retrofit2实现安卓中网络操作.md)
* [LinLog](docs/android/AndroidNote/Android开源框架相关/一款Android的Log、Toast的库.md)
* [Retrofit 2.0 使用教程](http://www.jianshu.com/p/a3e162261ab6)
* [retrofit 2.0 源码解析](http://www.jianshu.com/p/0c055ad46b6c)
* [关于 RxJava 背压](https://juejin.im/entry/58e704cbac502e4957b230eb)
* [RxJava 2.0中backpressure(背压)概念的理解](https://blog.csdn.net/jdsjlzx/article/details/52717636)
* [Retrofit2 完全解析 探索与okhttp之间的关系](https://blog.csdn.net/lmj623565791/article/details/51304204)


### 打包

* [打包jar包或aar包](docs/android/AndroidNote/Android打包相关/Android将library打包成jar文件或aar文件.md)
* [发布sdk到jcenter](docs/android/AndroidNote/Android打包相关/Android发布sdk到jcenter.md)


##### 框架源码分析
1. [EventBus源码分析](docs/android/AndroidNote/sources/eventbus.md)
2. [Bufferknife源码分析](docs/android/AndroidNote/sources/butterknife.md)
3. [Glide 源码分析](docs/android/AndroidNote/sources/glide.md)
4. [OKHttp 源码分析](docs/android/AndroidNote/sources/okhttp.md)
5. [Retrofit 源码分析](docs/android/AndroidNote/sources/retrofit.md)
6. [ViewModel 源码分析](docs/android/AndroidNote/sources/viewmodel.md)

## Java

### 基础

* [Java 基础知识回顾](docs/java/Java基础知识.md)
* [J2EE 基础知识回顾](docs/java/J2EE基础知识.md)
* [Collections 工具类和 Arrays 工具类常见方法](docs/java/Basis/Arrays%2CCollectionsCommonMethods.md)
* [Java常见关键字总结：static、final、this、super](docs/java/Basis/final、static、this、super.md) 
* [Java常见关键字总结：static、final、this、super](docs/java/Basis/final、static、this、super.md) 

### 容器

* **常见问题总结：**
  * [这几道Java集合框架面试题几乎必问](docs/java/这几道Java集合框架面试题几乎必问.md)
  * [Java 集合框架常见面试题总结](docs/java/Java集合框架常见面试题总结.md)
* **源码分析：**
  * [ArrayList 源码学习](docs/java/ArrayList.md) 
  * [【面试必备】透过源码角度一步一步带你分析 ArrayList 扩容机制](docs/java/ArrayList-Grow.md)    
  * [LinkedList 源码学习](docs/java/LinkedList.md)   
  * [HashMap(JDK1.8)源码学习](docs/java/HashMap.md)  

### 并发

* [并发编程面试必备：synchronized 关键字使用、底层原理、JDK1.6 之后的底层优化以及 和ReenTrantLock 的对比](docs/java/synchronized.md)
* [并发编程面试必备：乐观锁与悲观锁](docs/essential-content-for-interview/面试必备之乐观锁与悲观锁.md)
* [并发编程面试必备：JUC 中的 Atomic 原子类总结](docs/java/Multithread/Atomic.md)
* [并发编程面试必备：AQS 原理以及 AQS 同步组件总结](docs/java/Multithread/AQS.md)
* [BATJ都爱问的多线程面试题](docs/java/Multithread/BATJ都爱问的多线程面试题.md)
* [并发容器总结](docs/java/Multithread/并发容器总结.md)

### JVM

* [可能是把Java内存区域讲的最清楚的一篇文章](docs/java/可能是把Java内存区域讲的最清楚的一篇文章.md)
* [搞定JVM垃圾回收就是这么简单](docs/java/搞定JVM垃圾回收就是这么简单.md)
* [《深入理解Java虚拟机》第2版学习笔记](docs/java/Java虚拟机（jvm）.md)

### I/O

* [BIO,NIO,AIO 总结 ](docs/java/BIO-NIO-AIO.md)
* [Java IO 与 NIO系列文章](docs/java/Java%20IO与NIO.md)

### Java 8 

* [Java 8 新特性总结](docs/java/What's%20New%20in%20JDK8/Java8Tutorial.md)
* [Java 8 学习资源推荐](docs/java/What's%20New%20in%20JDK8/Java8教程推荐.md)

### 编程规范

- [Java 编程规范](docs/java/Java编程规范.md)

## 网络
* [浅析socket](docs/android/AndroidNote/网络协议/浅析socket.md)
* [浅析Hessian](docs/android/AndroidNote/网络协议/浅析Hessian协议.md)
* [浅析RPC协议](docs/android/AndroidNote/网络协议/浅析RPC协议.md)
* [浅析dubbo服务](docs/android/AndroidNote/网络协议/浅析dubbo服务.md)
* [SSH原理与应用](docs/android/AndroidNote/网络协议/SSH原理与应用.md)
* [理解OAuth 2.0](http://www.ruanyifeng.com/blog/2014/05/oauth_2_0.html)
* [OAuth 2和JWT - 如何设计安全的API？](http://blog.csdn.net/ljinddlj/article/details/53108261)
* [计算机网络常见面试题](docs/network/计算机网络.md)
* [计算机网络基础知识总结](docs/network/干货：计算机网络知识总结.md)
* [HTTPS中的TLS](docs/network/HTTPS中的TLS.md)

## 操作系统

### Linux相关

* [后端程序员必备的 Linux 基础知识](docs/operating-system/后端程序员必备的Linux基础知识.md)  
* [Shell 编程入门](docs/operating-system/Shell.md)  

## 数据结构与算法

### 数据结构

- [数据结构知识学习与面试](docs/dataStructures-algorithms/数据结构.md)

### 算法

- [算法学习资源推荐](docs/dataStructures-algorithms/算法学习资源推荐.md)  
- [算法总结——几道常见的子符串算法题 ](docs/dataStructures-algorithms/几道常见的子符串算法题.md)
- [算法总结——几道常见的链表算法题 ](docs/dataStructures-algorithms/几道常见的链表算法题.md)   
- [剑指offer部分编程题](docs/dataStructures-algorithms/剑指offer部分编程题.md)
- [公司真题](docs/dataStructures-algorithms/公司真题.md)
- [回溯算法经典案例之N皇后问题](docs/dataStructures-algorithms/Backtracking-NQueens.md)
- [算法设计常用思想](docs/dataStructures-algorithms/Backtracking-NQueens.md)

## 数据库

### MySQL

* [MySQL 学习与面试](docs/database/MySQL.md)
* [一千行MySQL学习笔记](docs/database/一千行MySQL命令.md)
* [MySQL高性能优化规范建议](docs/database/MySQL高性能优化规范建议.md)
* [搞定数据库索引就是这么简单](docs/database/MySQL%20Index.md)
* [事务隔离级别(图文详解)](docs/database/事务隔离级别(图文详解).md)
* [一条SQL语句在MySQL中如何执行的](docs/database/一条sql语句在mysql中如何执行的.md)
* [linux下安装MySQL](docs/android/AndroidNote/WebNote/MySQL相关/云服务器linux下安装MySQL.md)
* [MySQL基础操作](docs/android/AndroidNote/WebNote/MySQL相关/mysql基础操作.md)
* [MySQL导出数据库、表](docs/android/AndroidNote/WebNote/MySQL相关/Mysql导出数据库、表(有无数据).md)
* [Error-ER_TRUNCATED_WRONG_VALUE_FOR_FIELD](docs/android/AndroidNote/WebNote/MySQL相关/Error--ER_TRUNCATED_WRONG_VALUE_FOR_FIELD.md)
* [ERROR-1045-(28000)--Access-denied-for-user-'debian-sys-maint'@'localhost](docs/android/AndroidNote/WebNote/MySQL相关/ERROR-1045-(28000)--Access-denied-for-user-'debian-sys-maint'@'localho.md)
* [mysql设置远程链接权限](https://www.cnblogs.com/gdsblog/p/7349551.html)
* [关于初次安装mysql8.01遇到的问题解决](https://blog.csdn.net/l569746927/article/details/80025364)

### Redis

* [Redis 总结](docs/database/Redis/Redis.md)
* [Redlock分布式锁](docs/database/Redis/Redlock分布式锁.md)
* [如何做可靠的分布式锁，Redlock真的可行么](docs/database/Redis/如何做可靠的分布式锁，Redlock真的可行么.md)

## 系统设计

### 设计模式

- [设计模式系列文章](docs/system-design/设计模式.md)

### 常用框架

#### Spring

- [Spring 学习与面试](docs/system-design/framework/Spring学习与面试.md)
- [Spring中bean的作用域与生命周期](docs/system-design/framework/SpringBean.md)
- [SpringMVC 工作原理详解](docs/system-design/framework/SpringMVC%20%E5%B7%A5%E4%BD%9C%E5%8E%9F%E7%90%86%E8%AF%A6%E8%A7%A3.md)

#### ZooKeeper

- [可能是把 ZooKeeper 概念讲的最清楚的一篇文章](docs/system-design/framework/ZooKeeper.md)
- [ZooKeeper 数据模型和常见命令了解一下，速度收藏！](docs/system-design/framework/ZooKeeper数据模型和常见命令.md)

### 数据通信

- [数据通信(RESTful、RPC、消息队列)相关知识点总结](docs/system-design/data-communication/数据通信(RESTful、RPC、消息队列).md)
- [Dubbo 总结：关于 Dubbo 的重要知识点](docs/system-design/data-communication/dubbo.md)
- [消息队列总结：新手也能看懂，消息队列其实很简单](docs/system-design/data-communication/message-queue.md)
- [一文搞懂 RabbitMQ 的重要概念以及安装](docs/system-design/data-communication/rabbitmq.md)

### 网站架构

- [一文读懂分布式应该学什么](docs/system-design/website-architecture/分布式.md)
- [8 张图读懂大型网站技术架构](docs/system-design/website-architecture/8%20张图读懂大型网站技术架构.md)
- [【面试精选】关于大型网站系统架构你不得不懂的10个问题](docs/system-design/website-architecture/【面试精选】关于大型网站系统架构你不得不懂的10个问题.md)

## 面试指南

### 备战面试

* [【备战面试1】程序员的简历就该这样写](docs/essential-content-for-interview/PreparingForInterview/程序员的简历之道.md)
* [【备战面试2】初出茅庐的程序员该如何准备面试？](docs/essential-content-for-interview/PreparingForInterview/interviewPrepare.md)
* [【备战面试3】7个大部分程序员在面试前很关心的问题](docs/essential-content-for-interview/PreparingForInterview/JavaProgrammerNeedKnow.md)
* [【备战面试4】Github上开源的Java面试/学习相关的仓库推荐](docs/essential-content-for-interview/PreparingForInterview/JavaInterviewLibrary.md)
* [【备战面试5】如果面试官问你“你有什么问题问我吗？”时，你该如何回答](docs/essential-content-for-interview/PreparingForInterview/如果面试官问你“你有什么问题问我吗？”时，你该如何回答.md)
* [【备战面试6】美团面试常见问题总结（附详解答案）](docs/essential-content-for-interview/PreparingForInterview/美团面试常见问题总结.md)

### 常见面试题总结

* [第一周（2018-8-7）](docs/essential-content-for-interview/MostCommonJavaInterviewQuestions/第一周（2018-8-7）.md) (为什么 Java 中只有值传递、==与equals、 hashCode与equals)
* [第二周（2018-8-13）](docs/essential-content-for-interview/MostCommonJavaInterviewQuestions/第二周(2018-8-13).md)(String和StringBuffer、StringBuilder的区别是什么？String为什么是不可变的？、什么是反射机制？反射机制的应用场景有哪些？......)
* [第三周（2018-08-22）](docs/java/这几道Java集合框架面试题几乎必问.md) （Arraylist 与 LinkedList 异同、ArrayList 与 Vector 区别、HashMap的底层实现、HashMap 和 Hashtable 的区别、HashMap 的长度为什么是2的幂次方、HashSet 和 HashMap 区别、ConcurrentHashMap 和 Hashtable 的区别、ConcurrentHashMap线程安全的具体实现方式/底层具体实现、集合框架底层数据结构总结）
* [第四周(2018-8-30).md](docs/essential-content-for-interview/MostCommonJavaInterviewQuestions/第四周(2018-8-30).md) （主要内容是几道面试常问的多线程基础题。）

### 面经

- [5面阿里,终获offer(2018年秋招)](docs/essential-content-for-interview/BATJrealInterviewExperience/5面阿里,终获offer.md)

## 工具

### Git

* [Git入门](docs/tools/Git.md)

### Docker

* [Docker 入门](docs/tools/Docker.md)
* [一文搞懂 Docker 镜像的常用操作！](docs/tools/Docker-Image.md)

## 说明
本文并非原创，通过各位博主综合而得，以便供自己方便学习，在此感谢各位前辈，并在下面注明出处
- [Snailclimb/JavaGuide](https://github.com/Snailclimb/JavaGuide)
- [UCodeUStory/DataStructure](https://github.com/UCodeUStory/DataStructure)
- [JackChan1999/Android-Interview](https://github.com/JackChan1999/Android-Interview)
- [linsir6/AndroidNote](https://github.com/linsir6/AndroidNote)

