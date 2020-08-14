<h1 align="center">Java Android学习/面试指南 Q群：830556582</h1>

<!--| Ⅰ | Ⅱ | Ⅲ | Ⅳ | Ⅴ | Ⅵ | Ⅶ | Ⅷ | Ⅸ | Ⅹ | Ⅹ | Ⅹ |
| :--------: | :---------: | :---------: | :---------: | :---------: | :---------:| :---------: | :-------: | :-------:| :------:|:------:|
| Flutter[:iphone:](#Flutter)| Android[:pencil2:](#Android) | Java[:coffee:](#Java)|Kotlin[:unlock:](#Kotlin) | 面试[:memo:](#面试指南) |网络[:cloud:](#网络协议)| 操作系统 [:computer:](#操作系统)| 系统设计[:bulb:](#系统设计)| 工具[:wrench:](#工具)| 数据库[:floppy_disk:](#数据库)| 算法[:pencil2:](#数据结构与算法) |  TODO学习清单[:page_facing_up:](#TODO学习清单) |-->

| Flutter| Android | Java | Kotlin | &nbsp;面试&nbsp; | 网络 | 系统 | 系统设计 | &nbsp;工具&nbsp; | 数据库 | 算法 |TODO |
| :--------:| :--------: | :---------: | :---------: | :---------: | :---------: | :---------:| :---------: | :-------: | :-------:| :------:|:------:|
| [ :iphone:](#Flutter)| [:pencil2:](#Android) | [:coffee:](#Java)|[:unlock:](#Kotlin) | [:memo:](#面试指南) |[:cloud:](#网络)|  [:computer:](#操作系统)| [:bulb:](#系统设计)| [:wrench:](#工具)| [:floppy_disk:](#数据库)| [:pencil2:](#数据结构与算法) | [:page_facing_up:](#TODO学习清单) |

<br>

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
    - [Android常见设计模式](#Android常见设计模式) 
    - [音视频开发](#音视频开发)    
    - [开源框架](#开源框架)
    - [应用发布](#应用发布)
    - [打包](#打包)  
    - [原生功能讲解](docs/android/AndroidNote/READMENote.md)    
- [Java](#java)
    - [基础](#基础)
    - [容器](#容器)
    - [并发](#并发)
    - [JVM](#jvm)
    - [I/O](#io)
    - [Java 8](#java-8)
    - [编程规范](#编程规范)  
 - [TODO学习清单](#TODO学习清单)      
- [Kotlin学习](#Kotlin)
- [Flutter学习](#Flutter)
- [面试指南](#面试指南)
    - [备战面试](#备战面试)
    - [常见面试题总结](#常见面试题总结)
    - [面经](#面经)
    - [Android面试专场](docs/android/Android-Interview/README.md)
- [网络协议](#网络)
- [操作系统](#操作系统)
    - [Linux相关](#linux相关)
    - [计算机操作系统](#计算机操作系统)   
- [数据结构与算法](#数据结构与算法)
    - [数据结构](#数据结构)
    - [算法](#算法)
- [数据库](#数据库)
    - [MySQL](#mysql)
    - [Redis](#redis)
    - [数据库系统原理](docs/notes/数据库系统原理.md)
    - [SQL](docs/notes/SQL.md)
    - [Leetcode-Database 题解](docs/notes/Leetcode-Database%20题解.md)
- [系统设计](#系统设计)
    - [设计模式](#设计模式)
    - [常用框架](#常用框架)
    - [数据通信](#数据通信)
    - [网站架构](#网站架构)
    - [攻击技术](docs/notes/攻击技术.md)
- [工具](#工具)
    - [Git](#git)
    - [Docker](#Docker)
    - [构建工具](docs/notes/构建工具.md)
    - [正则表达式](docs/notes/正则表达式.md)
- [常见问题](docs/android/interview/README.md)

## Android

### 基础知识

* [Activity详细解析](docs/android/AndroidNote/Android基础/Activity详细解析.md)
* [Service详细解析](docs/android/AndroidNote/Android基础/Service详细解析.md)
* [IntentService详细解析](docs/android/AndroidNote/Android基础/IntentService详细解析.md)
* [IntentService原理解析文章](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=401611665&idx=1&sn=9b6b1f2924d4adfe4e89a322ab53df9c&scene=21#wechat_redirect)
* [ContentProvider实例详解](docs/android/AndroidNote/Android基础/ContentProvider实例详解.md)
* [BroadcastReceiver详细解析](docs/android/AndroidNote/Android基础/BroadcastReceiver详细解析.md)
* [Android异步任务机制之AsycTask](docs/android/AndroidNote/Android基础/Android异步任务机制之AsycTask.md)
* [Handler,Looper,MessageQueue关系](docs/android/AndroidNote/Android基础/Handler,Looper,MessageQueue关系.md)
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
* [Android 中获取控件宽和高的方法（详细解析）](https://blog.csdn.net/CodeIsPoisonous/article/details/54316025)

### 进阶

* [Android 学习笔记核心篇](https://juejin.im/post/5c46db4ae51d4503834d8227)
* [Android内存泄漏性能优化总结](docs/android/AndroidNote/内存性能.md)
* [进程间通信详解](docs/android/AndroidNote/IPC.md)
* [Android中的动画](docs/android/AndroidNote/Android进阶/Android中的动画.md)
* [深入了解MVXX模式](docs/android/AndroidNote/Android进阶/深入了解MVXX模式.md)
* [Android项目总结](docs/android/AndroidNote/Android进阶/Android项目总结.md)
* [Android项目总结2](docs/android/AndroidNote/Android进阶/Android项目总结2.md)
* [自定义RadioGroup](docs/android/AndroidNote/Android进阶/自定义RadioGroup.md)
* [Android导入项目一直在Building的解决方案](docs/android/AndroidNote/Android进阶/AndroidStudio导入工程一直在Building的解决方案.md)
* [基于TOTP的双向认证算法](docs/android/AndroidNote/Android进阶/基于OTP算法的双向认证.md)
* [基于TOTP的双向认证算法](docs/android/AndroidNote/Android进阶/基于OTP算法的双向认证.md)
* [Android 触控事件解析 - Mastering The Android Touch System 笔记](https://www.jianshu.com/p/c65da5e81afd)
* [《Android 高性能编程》—— @IntDef 注解，减缓枚举的使用](https://blog.csdn.net/OneDeveloper/article/details/79973205)
* [Android官网建议代码规范](https://source.android.com/source/code-style#java-language-rules)
* [30多年编码经验总结成10条最佳实践](https://mp.weixin.qq.com/s?__biz=MzIyMjQ0MTU0NA==&mid=2247484524&idx=1&sn=5b2759e6d89f01e61d021545ca7556b9&chksm=e82c3d4bdf5bb45dd77227982931ede8229ee6910829253a57bb905e810c89bd3f0a162786e8&mpshare=1&scene=23&srcid=1023FjKcLWtRlcDpwEeeJnCN#rd)
* [Android中利用异步来优化处理速度](https://mp.weixin.qq.com/s?__biz=MzI0MjE3OTYwMg==&mid=401555104&idx=1&sn=501e6158e6eb26b4e86467be01fd290e&scene=21#wechat_redirect)
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
* [深入理解Android之Gradle Groovy](https://blog.csdn.net/innost/article/details/48228651)
* [Groovy 闭包](https://www.jianshu.com/p/6dc2074480b8)
* [要点提炼| Gradle指南](https://www.jianshu.com/p/1274c1f1b6a4)
* [Gradle专题][39]
* [发布library到Maven仓库][40]

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

## Android常见设计模式
* **Android常见设计模式**
  * [观察者模式](https://blog.csdn.net/chengyuqiang/article/details/79222294)
  * [策略模式](https://github.com/pengMaster/strategyMode)
  * [建造者模式](https://www.jianshu.com/p/154948d5adc6)
  * [适配器模式](https://blog.csdn.net/u012583459/article/details/47079529)
  * [代理模式](https://blog.csdn.net/u012583459/article/details/47079529)
  * [工厂模式](https://blog.csdn.net/u012583459/article/details/47079549)
  * [单例模式](https://blog.csdn.net/u012583459/article/details/47079549)
  * [命令模式](https://blog.csdn.net/u012583459/article/details/47079549)


    
### 音视频开发
- [音视频开发][44]
    - [搭建nginx+rtmp服务器][18]
    - [视频播放相关内容总结][19]
    - [视频解码之软解与硬解][20]
    - [音视频基础知识][21]
    - [Android WebRTC简介][22]
    - [Android音视频开发知识(未完)][23]
    - [DLNA简介][24]
    
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
*[Dagger2][199]        
     - [1.Dagger2简介(一).md][200]
     - [2.Dagger2入门demo(二).md][201]    
     - [3.Dagger2入门demo扩展(三).md][202]
     - [4.Dagger2单例(四).md][203]
     - [5.Dagger2Lay和Provider(五).md][204]
     - [6.Dagger2Android示例代码(六).md][205]
     - [7.Dagger2之dagger-android(七).md][206]            
     - [8.Dagger2与MVP(八).md][207]    
     - [9.Dagger2原理分析(九).md][212]
*  [图片加载][45]
    - [Glide简介(上)][25]
    - [Glide简介(下)][26]
    - [图片加载库比较][27]
* [RxJava][46]
    - [RxJava详解(一)][28]
    - [RxJava详解(二)][29]
    - [RxJava详解(三)][30]
    - [RxJava详解之执行原理(四)][209]
    - [RxJava详解之操作符执行原理(五)][210]
    - [RxJava详解之线程调度原理(六)][211]
    - [RxJava系列全家桶][31]

### 应用发布
- [应用发布][50]
    - [使用Jenkins实现自动化打包][198]
    - [Android应用发布][41]
    - [Zipalign优化][42]
    

### 打包

* [打包jar包或aar包](docs/android/AndroidNote/Android打包相关/Android将library打包成jar文件或aar文件.md)
* [发布sdk到jcenter](docs/android/AndroidNote/Android打包相关/Android发布sdk到jcenter.md)


##### 框架源码分析
- [EventBus源码分析](docs/android/sources/eventbus.md)
- [Bufferknife源码分析](docs/android/sources/butterknife.md)
- [Glide 源码分析](docs/android/sources/glide.md)
- [OKHttp 源码分析](docs/android/sources/okhttp.md)
- [Retrofit 源码分析](docs/android/sources/retrofit.md)
- [ViewModel 源码分析](docs/android/sources/viewmodel.md)
- [自定义View详解][1]
- [Activity界面绘制过程详解][2]
- [Activity启动过程][3]
- [Android Touch事件分发详解][4]
- [AsyncTask详解][5]
- [butterknife源码详解][6]
- [InstantRun详解][7]
- [ListView源码分析][8]
- [VideoView源码分析][9]
 - [View绘制过程详解][10]
 - [网络部分][11]
        - [HttpURLConnection详解][12]
        - [HttpURLConnection与HttpClient][13]
        - [volley-retrofit-okhttp之我们该如何选择网路框架][14]
        - [Volley源码分析][15]
        - [Retrofit详解(上)][16]
        - [Retrofit详解(下)][17]
## Kotlin
- [Kotlin学习][48]
    - [Kotlin学习教程(一)][180]
    - [Kotlin学习教程(二)][181]
    - [Kotlin学习教程(三)][182]
    - [Kotlin学习教程(四)][183]
    - [Kotlin学习教程(五)][184]
    - [Kotlin学习教程(六)][185]
    - [Kotlin学习教程(七)][186]
    - [Kotlin学习教程(八)][187]
    - [Kotlin学习教程(九)][188]
    - [Kotlin学习教程(十)][197]
    - [集合之常用操作符汇总](https://www.cnblogs.com/Jetictors/p/9241867.html)

## Flutter
* **Flutter学习：**
  * [flutter脚手架封装](https://github.com/pengMaster/flutter_app)
  * [flutter中文学习网](https://book.flutterchina.club/chapter2/)
  * [flutter常用库总结](https://www.cnblogs.com/yangyxd/p/9232308.html)
  * [flutter开源项目](https://flutterchina.club/opensource.html)
  * [flutter基础语法](https://www.jianshu.com/p/3d927a7bf020)
  * [Flutter常用工具类](https://juejin.im/post/5d0f4c54f265da1bb31c426c?utm_source=gold_browser_extension)
  * [Flutter-learning](https://github.com/AweiLoveAndroid/Flutter-learning)
  
## TODO学习清单
- [TODO学习清单](docs/android/self.md)  
    
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

### 计算机操作系统
- [计算机操作系统](docs/notes/计算机操作系统%20-%20目录.md)


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

### 数据库系统原理
- [数据库系统原理](docs/notes/数据库系统原理.md)

### SQL
- [SQL](docs/notes/SQL.md)

### Leetcode-Database 题解
- [Leetcode-Database 题解](docs/notes/Leetcode-Database%20题解.md)
    
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

### 攻击技术
- [攻击技术](docs/notes/攻击技术.md)

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

### Android面试专场
- [Android面试专场](docs/android/Android-Interview/README.md)

## 工具

### Git

* [Git入门](docs/tools/Git.md)

### Docker

* [Docker 入门](docs/tools/Docker.md)
* [一文搞懂 Docker 镜像的常用操作！](docs/tools/Docker-Image.md)

### 构建工具
* [构建工具](docs/notes/构建工具.md)

### 正则表达式
* [正则表达式](docs/notes/正则表达式.md)

## 致谢
本文并非原创，通过各位博主综合而得，以便供自己方便学习，在此感谢各位前辈，并在下面注明出处
- [Snailclimb/JavaGuide](https://github.com/Snailclimb/JavaGuide)
- [UCodeUStory/DataStructure](https://github.com/UCodeUStory/DataStructure)
- [JackChan1999/Android-Interview](https://github.com/JackChan1999/Android-Interview)
- [linsir6/AndroidNote](https://github.com/linsir6/AndroidNote)
- [CharonChui/AndroidNote](https://github.com/CharonChui/AndroidNote)
- [CS-Notes](https://github.com/CyC2018/CS-Notes)

<a href="https://github.com/Snailclimb/JavaGuide" >
​    <img src="https://avatars0.githubusercontent.com/u/29880145?s=400&v=4" width="50px">
</a> 
<a href="https://github.com/UCodeUStory/DataStructure">
​    <img src="https://avatars3.githubusercontent.com/u/17451281?s=400&v=4" width="50px">
</a>
<a href="https://github.com/JackChan1999/Android-Interview">
​    <img src="https://avatars0.githubusercontent.com/u/16631168?s=400&v=4" width="50px">
</a>
<a href="https://github.com/linsir6/AndroidNote">
​    <img src="https://avatars2.githubusercontent.com/u/16979367?s=400&v=4" width="50px">
</a>
<a href="https://github.com/CharonChui/AndroidNote">
​    <img src="https://avatars0.githubusercontent.com/u/6140231?s=400&v=4" width="50px">
</a>
<a href="https://github.com/CyC2018/CS-Notes">
​    <img src="https://avatars0.githubusercontent.com/u/36260787?s=400&v=4" width="50px">
</a>

License
===

    MIT License
    
    Copyright (c) 2019 pengMaster
    
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
    
    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.


[1]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/%E8%87%AA%E5%AE%9A%E4%B9%89View%E8%AF%A6%E8%A7%A3.md        "自定义View详解" 
[2]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/Activity%E7%95%8C%E9%9D%A2%E7%BB%98%E5%88%B6%E8%BF%87%E7%A8%8B%E8%AF%A6%E8%A7%A3.md  "Activity界面绘制过程详解" 
[3]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/Activity%E5%90%AF%E5%8A%A8%E8%BF%87%E7%A8%8B.md    "Activity启动过程"
[4]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/Android%20Touch%E4%BA%8B%E4%BB%B6%E5%88%86%E5%8F%91%E8%AF%A6%E8%A7%A3.md    "Android Touch事件分发详解"
[5]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/AsyncTask%E8%AF%A6%E8%A7%A3.md   "AsyncTask详解"
[6]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/butterknife%E6%BA%90%E7%A0%81%E8%AF%A6%E8%A7%A3.md   "butterknife源码详解"
[7]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/InstantRun%E8%AF%A6%E8%A7%A3.md   "InstantRun详解"
[8]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/ListView源码分析.md   "ListView源码分析"
[9]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/VideoView%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90.md   "VideoView源码分析"
[10]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/View%E7%BB%98%E5%88%B6%E8%BF%87%E7%A8%8B%E8%AF%A6%E8%A7%A3.md   "View绘制过程详解"
[11]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//SourceAnalysis/Netowork   "网络部分"
[12]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/Netowork/HttpURLConnection%E8%AF%A6%E8%A7%A3.md   "HttpURLConnection详解"
[13]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/Netowork/HttpURLConnection%E4%B8%8EHttpClient.md   "HttpURLConnection与HttpClient"
[14]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/Netowork/volley-retrofit-okhttp%E4%B9%8B%E6%88%91%E4%BB%AC%E8%AF%A5%E5%A6%82%E4%BD%95%E9%80%89%E6%8B%A9%E7%BD%91%E8%B7%AF%E6%A1%86%E6%9E%B6.md   "volley-retrofit-okhttp之我们该如何选择网路框架"
[15]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/Netowork/Volley%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90.md   "Volley源码分析"
[16]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/Netowork/Retrofit%E8%AF%A6%E8%A7%A3(%E4%B8%8A).md   "Retrofit详解(上)"
[17]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/SourceAnalysis/Netowork/Retrofit%E8%AF%A6%E8%A7%A3(%E4%B8%8B).md   "Retrofit详解(下)"
[18]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/VideoDevelopment/%E6%90%AD%E5%BB%BAnginx%2Brtmp%E6%9C%8D%E5%8A%A1%E5%99%A8.md   "搭建nginx+rtmp服务器"
[19]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/VideoDevelopment/%E8%A7%86%E9%A2%91%E6%92%AD%E6%94%BE%E7%9B%B8%E5%85%B3%E5%86%85%E5%AE%B9%E6%80%BB%E7%BB%93.md   "视频播放相关内容总结"
[20]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/VideoDevelopment/%E8%A7%86%E9%A2%91%E8%A7%A3%E7%A0%81%E4%B9%8B%E8%BD%AF%E8%A7%A3%E4%B8%8E%E7%A1%AC%E8%A7%A3.md   "视频解码之软解与硬解"
[21]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/VideoDevelopment/%E9%9F%B3%E8%A7%86%E9%A2%91%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md   "音视频基础知识"
[22]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/VideoDevelopment/Android%20WebRTC%E7%AE%80%E4%BB%8B.md   "Android WebRTC简介"
[23]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/VideoDevelopment/Android%E9%9F%B3%E8%A7%86%E9%A2%91%E5%BC%80%E5%8F%91.md   "Android音视频开发知识"
[24]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/VideoDevelopment/DLNA%E7%AE%80%E4%BB%8B.md   "DLNA简介"
[25]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/ImageLoaderLibrary/Glide%E7%AE%80%E4%BB%8B(%E4%B8%8A).md   "Glide简介(上)"
[26]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/ImageLoaderLibrary/Glide%E7%AE%80%E4%BB%8B(%E4%B8%8B).md   "Glide简介(下)"
[27]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/ImageLoaderLibrary/%E5%9B%BE%E7%89%87%E5%8A%A0%E8%BD%BD%E5%BA%93%E6%AF%94%E8%BE%83.md   "图片加载库比较"
[28]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/RxJavaPart/1.RxJava%E8%AF%A6%E8%A7%A3(%E4%B8%80).md   "RxJava详解(一)"
[29]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/RxJavaPart/2.RxJava%E8%AF%A6%E8%A7%A3(%E4%BA%8C).md   "RxJava详解(二)"
[30]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/RxJavaPart/3.RxJava%E8%AF%A6%E8%A7%A3(%E4%B8%89).md   "RxJava详解(三)"
[31]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/RxJavaPart/7.RxJava%E7%B3%BB%E5%88%97%E5%85%A8%E5%AE%B6%E6%A1%B6.md   "RxJava系列全家桶"
[32]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Tools%26Library/%E7%9B%AE%E5%89%8D%E6%B5%81%E8%A1%8C%E7%9A%84%E5%BC%80%E5%8F%91%E7%BB%84%E5%90%88.md   "目前流行的开发组合"
[33]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Tools%26Library/%E6%80%A7%E8%83%BD%E4%BC%98%E5%8C%96%E7%9B%B8%E5%85%B3%E5%B7%A5%E5%85%B7.md   "性能优化相关工具"
[34]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Tools%26Library/Android%E5%BC%80%E5%8F%91%E5%B7%A5%E5%85%B7%E5%8F%8A%E7%B1%BB%E5%BA%93.md   "Android开发工具及类库"
[35]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Tools%26Library/Github%E4%B8%AA%E4%BA%BA%E4%B8%BB%E9%A1%B5%E7%BB%91%E5%AE%9A%E5%9F%9F%E5%90%8D.md   "Github个人主页绑定域名"
[36]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Tools%26Library/Markdown%E5%AD%A6%E4%B9%A0%E6%89%8B%E5%86%8C.md   "Markdown学习手册"
[37]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Tools%26Library/MAT%E5%86%85%E5%AD%98%E5%88%86%E6%9E%90.md   "MAT内存分析"
[38]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E4%B8%80).md   "Kotlin学习教程(一)(未完)"
[39]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Gradle%26Maven/Gradle%E4%B8%93%E9%A2%98.md   "Gradle专题"
[40]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Gradle%26Maven/%E5%8F%91%E5%B8%83library%E5%88%B0Maven%E4%BB%93%E5%BA%93.md   "发布library到Maven仓库"
[41]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AppPublish/Android%E5%BA%94%E7%94%A8%E5%8F%91%E5%B8%83.md   "Android应用发布"
[42]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AppPublish/Zipalign%E4%BC%98%E5%8C%96.md   "Zipalign优化"
[43]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//SourceAnalysis   "源码解析"
[44]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//VideoDevelopment   "音视频开发"
[45]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//ImageLoaderLibrary   "图片加载"
[46]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//RxJavaPart   "RxJava"
[47]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//Tools%26Library   "开发工具"
[48]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//KotlinCourse   "Kotlin学习"
[49]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//Gradle%26Maven   "Gradle&Maven"
[50]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//AppPublish   "应用发布"
[51]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//AndroidStudioCourse   "Android Studio使用教程"
[52]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//AdavancedPart   "进阶部分"
[53]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//JavaKnowledge   "Java基础及算法"
[54]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//BasicKnowledge   "基础部分"
[55]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AndroidStudioCourse/AndroidStudio%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B(%E7%AC%AC%E4%B8%80%E5%BC%B9).md   "AndroidStudio使用教程(第一弹)"
[56]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AndroidStudioCourse/AndroidStudio%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B(%E7%AC%AC%E4%BA%8C%E5%BC%B9).md   "AndroidStudio使用教程(第二弹)"
[57]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AndroidStudioCourse/AndroidStudio%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B(%E7%AC%AC%E4%B8%89%E5%BC%B9).md   "AndroidStudio使用教程(第三弹)"
[58]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AndroidStudioCourse/AndroidStudio%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B(%E7%AC%AC%E5%9B%9B%E5%BC%B9).md   "AndroidStudio使用教程(第四弹)"
[59]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AndroidStudioCourse/AndroidStudio%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B(%E7%AC%AC%E4%BA%94%E5%BC%B9).md   "AndroidStudio使用教程(第五弹)"
[60]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AndroidStudioCourse/AndroidStudio%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B(%E7%AC%AC%E5%85%AD%E5%BC%B9).md   "AndroidStudio使用教程(第六弹)"
[61]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AndroidStudioCourse/AndroidStudio%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B(%E7%AC%AC%E4%B8%83%E5%BC%B9).md   "AndroidStudio使用教程(第七弹)"
[62]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AndroidStudioCourse/Android%20Studio%E4%BD%A0%E5%8F%AF%E8%83%BD%E4%B8%8D%E7%9F%A5%E9%81%93%E7%9A%84%E6%93%8D%E4%BD%9C.md   "Android Studio你可能不知道的操作"
[63]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AndroidStudioCourse/AndroidStudio%E6%8F%90%E9%AB%98Build%E9%80%9F%E5%BA%A6.md   "AndroidStudio提高Build速度"
[64]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AndroidStudioCourse/AndroidStudio%E4%B8%AD%E8%BF%9B%E8%A1%8Cndk%E5%BC%80%E5%8F%91.md   "AndroidStudio中进行ndk开发"
[65]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/%E5%B8%83%E5%B1%80%E4%BC%98%E5%8C%96.md   "布局优化"
[66]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/%E5%B1%8F%E5%B9%95%E9%80%82%E9%85%8D%E4%B9%8B%E7%99%BE%E5%88%86%E6%AF%94%E6%96%B9%E6%A1%88%E8%AF%A6%E8%A7%A3.md   "屏幕适配之百分比方案详解"
[67]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/%E7%83%AD%E4%BF%AE%E5%A4%8D%E5%AE%9E%E7%8E%B0.md   "热修复实现"
[68]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/%E5%A6%82%E4%BD%95%E8%AE%A9Service%E5%B8%B8%E9%A9%BB%E5%86%85%E5%AD%98.md   "如何让Service常驻内存"
[69]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/%E9%80%9A%E8%BF%87Hardware%20Layer%E6%8F%90%E9%AB%98%E5%8A%A8%E7%94%BB%E6%80%A7%E8%83%BD.md   "通过Hardware Layer提高动画性能"
[70]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/%E6%80%A7%E8%83%BD%E4%BC%98%E5%8C%96.md   "性能优化"
[71]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/%E6%B3%A8%E8%A7%A3%E4%BD%BF%E7%94%A8.md   "注解使用"
[72]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/Android6.0%E6%9D%83%E9%99%90%E7%B3%BB%E7%BB%9F.md   "Android6.0权限系统"
[73]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/Android%E5%BC%80%E5%8F%91%E4%B8%8D%E7%94%B3%E8%AF%B7%E6%9D%83%E9%99%90%E6%9D%A5%E4%BD%BF%E7%94%A8%E5%AF%B9%E5%BA%94%E5%8A%9F%E8%83%BD.md   "Android开发不申请权限来使用对应功能"
[74]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/Android%E5%BC%80%E5%8F%91%E4%B8%AD%E7%9A%84MVP%E6%A8%A1%E5%BC%8F%E8%AF%A6%E8%A7%A3.md   "Android开发中的MVP模式详解"
[75]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/Android%E5%90%AF%E5%8A%A8%E6%A8%A1%E5%BC%8F%E8%AF%A6%E8%A7%A3.md   "Android启动模式详解"
[76]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/Android%E5%8D%B8%E8%BD%BD%E5%8F%8D%E9%A6%88.md   "Android卸载反馈"
[77]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/ApplicationId%20vs%20PackageName.md   "ApplicationId vs PackageName"
[78]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/ART%E4%B8%8EDalvik.md   "ART与Dalvik"
[79]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/BroadcastReceiver%E5%AE%89%E5%85%A8%E9%97%AE%E9%A2%98.md   "BroadcastReceiver安全问题"
[80]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/Handler%E5%AF%BC%E8%87%B4%E5%86%85%E5%AD%98%E6%B3%84%E9%9C%B2%E5%88%86%E6%9E%90.md   "Handler导致内存泄露分析"
[81]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/Library%E9%A1%B9%E7%9B%AE%E4%B8%AD%E8%B5%84%E6%BA%90id%E4%BD%BF%E7%94%A8case%E6%97%B6%E6%8A%A5%E9%94%99.md   "Library项目中资源id使用case时报错"
[82]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/Mac%E4%B8%8B%E9%85%8D%E7%BD%AEadb%E5%8F%8AAndroid%E5%91%BD%E4%BB%A4.md   "Mac下配置adb及Android命令"
[83]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/MaterialDesign%E4%BD%BF%E7%94%A8.md   "MaterialDesign使用"
[84]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/RecyclerView%E4%B8%93%E9%A2%98.md   "RecyclerView专题"
[85]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E5%B8%B8%E7%94%A8%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%A4%A7%E5%85%A8.md   "常用命令行大全"
[86]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E5%8D%95%E4%BE%8B%E7%9A%84%E6%9C%80%E4%BD%B3%E5%AE%9E%E7%8E%B0%E6%96%B9%E5%BC%8F.md   "单例的最佳实现方式"
[87]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84.md   "数据结构"
[88]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E8%8E%B7%E5%8F%96%E4%BB%8A%E5%90%8E%E5%A4%9A%E5%B0%91%E5%A4%A9%E5%90%8E%E7%9A%84%E6%97%A5%E6%9C%9F.md   "获取今后多少天后的日期"
[89]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E5%89%91%E6%8C%87Offer(%E4%B8%8A).md   "剑指Offer(上)"
[90]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/剑指Offer(下).md   "剑指Offer(下)"
[91]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E5%BC%BA%E5%BC%95%E7%94%A8%E3%80%81%E8%BD%AF%E5%BC%95%E7%94%A8%E3%80%81%E5%BC%B1%E5%BC%95%E7%94%A8%E3%80%81%E8%99%9A%E5%BC%95%E7%94%A8.md   "强引用、软引用、弱引用、虚引用"
[92]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E7%94%9F%E4%BA%A7%E8%80%85%E6%B6%88%E8%B4%B9%E8%80%85.md   "生产者消费者"
[93]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E6%95%B0%E6%8D%AE%E5%8A%A0%E5%AF%86%E5%8F%8A%E8%A7%A3%E5%AF%86.md   "数据加密及解密"
[94]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E6%AD%BB%E9%94%81.md   "死锁"
[95]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E5%B8%B8%E8%A7%81%E7%AE%97%E6%B3%95.md   "算法"
[96]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E7%BD%91%E7%BB%9C%E8%AF%B7%E6%B1%82%E7%9B%B8%E5%85%B3%E5%86%85%E5%AE%B9%E6%80%BB%E7%BB%93.md   "网络请求相关内容总结"
[97]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E7%BA%BF%E7%A8%8B%E6%B1%A0%E7%9A%84%E5%8E%9F%E7%90%86.md   "线程池的原理"
[98]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E5%8E%9F%E5%AD%90%E6%80%A7%E3%80%81%E5%8F%AF%E8%A7%81%E6%80%A7%E4%BB%A5%E5%8F%8A%E6%9C%89%E5%BA%8F%E6%80%A7.md   "原子性、可见性以及有序性"
[99]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/Base64%E5%8A%A0%E5%AF%86.md   "Base64加密"
[100]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/Git%E7%AE%80%E4%BB%8B.md   "Git简介"
[101]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/hashCode%E4%B8%8Eequals.md   "hashCode与equals"
[102]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/HashMap%E5%AE%9E%E7%8E%B0%E5%8E%9F%E7%90%86%E5%88%86%E6%9E%90.md   "HashMap实现原理分析"
[103]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/Java%E5%9F%BA%E7%A1%80%E9%9D%A2%E8%AF%95%E9%A2%98.md   "Java基础面试题"
[104]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/JVM%E5%9E%83%E5%9C%BE%E5%9B%9E%E6%94%B6%E6%9C%BA%E5%88%B6.md   "JVM垃圾回收机制"
[105]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/MD5%E5%8A%A0%E5%AF%86.md   "MD5加密"
[106]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/MVC%E4%B8%8EMVP%E5%8F%8AMVVM.md   "MVC与MVP及MVVM"
[107]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/RMB%E5%A4%A7%E5%B0%8F%E5%86%99%E8%BD%AC%E6%8D%A2.md   "RMB大小写转换"
[108]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/Vim%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B.md   "Vim使用教程"
[109]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/volatile%E5%92%8CSynchronized%E5%8C%BA%E5%88%AB.md   "volatile和Synchronized区别"
[110]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E5%AE%89%E5%85%A8%E9%80%80%E5%87%BA%E5%BA%94%E7%94%A8%E7%A8%8B%E5%BA%8F.md   "安全退出应用程序"
[111]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E7%97%85%E6%AF%92.md   "病毒"
[112]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%B6%85%E7%BA%A7%E7%AE%A1%E7%90%86%E5%91%98(DevicePoliceManager).md   "超级管理员(DevicePoliceManager)"
[113]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E7%A8%8B%E5%BA%8F%E7%9A%84%E5%90%AF%E5%8A%A8%E3%80%81%E5%8D%B8%E8%BD%BD%E5%92%8C%E5%88%86%E4%BA%AB.md   "程序的启动、卸载和分享"
[114]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E4%BB%A3%E7%A0%81%E6%B7%B7%E6%B7%86.md   "代码混淆"
[115]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%AF%BB%E5%8F%96%E7%94%A8%E6%88%B7logcat%E6%97%A5%E5%BF%97.md   "读取用户logcat日志"
[116]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E7%9F%AD%E4%BF%A1%E5%B9%BF%E6%92%AD%E6%8E%A5%E6%94%B6%E8%80%85.md   "短信广播接收者"
[117]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E5%A4%9A%E7%BA%BF%E7%A8%8B%E6%96%AD%E7%82%B9%E4%B8%8B%E8%BD%BD.md   "多线程断点下载"
[118]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E9%BB%91%E5%90%8D%E5%8D%95%E6%8C%82%E6%96%AD%E7%94%B5%E8%AF%9D%E5%8F%8A%E5%88%A0%E9%99%A4%E7%94%B5%E8%AF%9D%E8%AE%B0%E5%BD%95.md   "黑名单挂断电话及删除电话记录"
[119]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E6%A8%AA%E5%90%91ListView.md   "横向ListView"
[120]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E6%BB%91%E5%8A%A8%E5%88%87%E6%8D%A2Activity(GestureDetector).md   "滑动切换Activity(GestureDetector)"
[121]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%8E%B7%E5%8F%96%E8%81%94%E7%B3%BB%E4%BA%BA.md   "获取联系人"
[122]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%8E%B7%E5%8F%96%E6%89%8B%E6%9C%BA%E5%8F%8ASD%E5%8D%A1%E5%8F%AF%E7%94%A8%E5%AD%98%E5%82%A8%E7%A9%BA%E9%97%B4.md   "获取手机及SD卡可用存储空间"
[123]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%8E%B7%E5%8F%96%E6%89%8B%E6%9C%BA%E4%B8%AD%E6%89%80%E6%9C%89%E5%AE%89%E8%A3%85%E7%9A%84%E7%A8%8B%E5%BA%8F.md   "获取手机中所有安装的程序"
[124]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%8E%B7%E5%8F%96%E4%BD%8D%E7%BD%AE(LocationManager).md   "获取位置(LocationManager)"
[125]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%8E%B7%E5%8F%96%E5%BA%94%E7%94%A8%E7%A8%8B%E5%BA%8F%E7%BC%93%E5%AD%98%E5%8F%8A%E4%B8%80%E9%94%AE%E6%B8%85%E7%90%86.md   "获取应用程序缓存及一键清理"
[126]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E5%BC%80%E5%8F%91%E4%B8%AD%E5%BC%82%E5%B8%B8%E7%9A%84%E5%A4%84%E7%90%86.md   "开发中异常的处理"
[127]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E5%BC%80%E5%8F%91%E4%B8%ADLog%E7%9A%84%E7%AE%A1%E7%90%86.md   "开发中Log的管理"
[128]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E5%BF%AB%E6%8D%B7%E6%96%B9%E5%BC%8F%E5%B7%A5%E5%85%B7%E7%B1%BB.md   "快捷方式工具类"
[129]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E6%9D%A5%E7%94%B5%E5%8F%B7%E7%A0%81%E5%BD%92%E5%B1%9E%E5%9C%B0%E6%8F%90%E7%A4%BA%E6%A1%86.md   "来电号码归属地提示框"
[130]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E6%9D%A5%E7%94%B5%E7%9B%91%E5%90%AC%E5%8F%8A%E5%BD%95%E9%9F%B3.md   "来电监听及录音"
[131]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E9%9B%B6%E6%9D%83%E9%99%90%E4%B8%8A%E4%BC%A0%E6%95%B0%E6%8D%AE.md   "零权限上传数据"
[132]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E5%86%85%E5%AD%98%E6%B3%84%E6%BC%8F.md   "内存泄漏"
[133]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E5%B1%8F%E5%B9%95%E9%80%82%E9%85%8D.md   "屏幕适配"
[134]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E4%BB%BB%E5%8A%A1%E7%AE%A1%E7%90%86%E5%99%A8(ActivityManager).md   "任务管理器(ActivityManager)"
[135]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E6%89%8B%E6%9C%BA%E6%91%87%E6%99%83.md   "手机摇晃"
[136]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E7%AB%96%E7%9D%80%E7%9A%84Seekbar.md   "竖着的Seekbar"
[137]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E6%95%B0%E6%8D%AE%E5%AD%98%E5%82%A8.md   "数据存储"
[138]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E6%90%9C%E7%B4%A2%E6%A1%86.md   "搜索框"
[139]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E9%94%81%E5%B1%8F%E4%BB%A5%E5%8F%8A%E8%A7%A3%E9%94%81%E7%9B%91%E5%90%AC.md   "锁屏以及解锁监听"
[140]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E6%96%87%E4%BB%B6%E4%B8%8A%E4%BC%A0.md   "文件上传"
[141]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E4%B8%8B%E6%8B%89%E5%88%B7%E6%96%B0ListView.md   "下拉刷新ListView"
[142]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E4%BF%AE%E6%94%B9%E7%B3%BB%E7%BB%9F%E7%BB%84%E4%BB%B6%E6%A0%B7%E5%BC%8F.md   "修改系统组件样式"
[143]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E9%9F%B3%E9%87%8F%E5%8F%8A%E5%B1%8F%E5%B9%95%E4%BA%AE%E5%BA%A6%E8%B0%83%E8%8A%82.md   "音量及屏幕亮度调节"
[144]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E5%BA%94%E7%94%A8%E5%AE%89%E8%A3%85.md   "应用安装"
[145]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E5%BA%94%E7%94%A8%E5%90%8E%E5%8F%B0%E5%94%A4%E9%86%92%E5%90%8E%E6%95%B0%E6%8D%AE%E7%9A%84%E5%88%B7%E6%96%B0.md   "应用后台唤醒后数据的刷新"
[146]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E7%9F%A5%E8%AF%86%E5%A4%A7%E6%9D%82%E7%83%A9.md   "知识大杂烩"
[147]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%B5%84%E6%BA%90%E6%96%87%E4%BB%B6%E6%8B%B7%E8%B4%9D%E7%9A%84%E4%B8%89%E7%A7%8D%E6%96%B9%E5%BC%8F.md   "资源文件拷贝的三种方式"
[148]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%87%AA%E5%AE%9A%E4%B9%89%E8%83%8C%E6%99%AF.md   "自定义背景"
[149]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%87%AA%E5%AE%9A%E4%B9%89%E6%8E%A7%E4%BB%B6.md   "自定义控件"
[150]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%87%AA%E5%AE%9A%E4%B9%89%E7%8A%B6%E6%80%81%E6%A0%8F%E9%80%9A%E7%9F%A5.md   "自定义状态栏通知"
[151]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/%E8%87%AA%E5%AE%9A%E4%B9%89Toast.md   "自定义Toast"
[152]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/adb%20logcat%E4%BD%BF%E7%94%A8%E7%AE%80%E4%BB%8B.md   "adb logcat使用简介"
[153]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Android%E7%BC%96%E7%A0%81%E8%A7%84%E8%8C%83.md   "Android编码规范"
[154]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Android%E5%8A%A8%E7%94%BB.md   "Android动画"
[155]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Android%E5%9F%BA%E7%A1%80%E9%9D%A2%E8%AF%95%E9%A2%98.md   "Android基础面试题"
[156]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Android%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md   "Android入门介绍"
[157]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Android%E5%9B%9B%E5%A4%A7%E7%BB%84%E4%BB%B6%E4%B9%8BContentProvider.md   "Android四大组件之ContentProvider"
[158]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Android%E5%9B%9B%E5%A4%A7%E7%BB%84%E4%BB%B6%E4%B9%8BService.md   "Android四大组件之Service"
[159]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Ant%E6%89%93%E5%8C%85.md   "Ant打包"
[160]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Bitmap%E4%BC%98%E5%8C%96.md   "Bitmap优化"
[161]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Fragment%E4%B8%93%E9%A2%98.md   "Fragment专题"
[162]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Home%E9%94%AE%E7%9B%91%E5%90%AC.md   "Home键监听"
[163]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/HttpClient%E6%89%A7%E8%A1%8CGet%E5%92%8CPost%E8%AF%B7%E6%B1%82.md   "HttpClient执行Get和Post请求"
[164]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/JNI_C%E8%AF%AD%E8%A8%80%E5%9F%BA%E7%A1%80.md   "JNI_C语言基础"
[165]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/JNI%E5%9F%BA%E7%A1%80.md   "JNI基础"
[166]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/ListView%E4%B8%93%E9%A2%98.md   "ListView专题"
[167]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Parcelable%E5%8F%8ASerializable.md   "Parcelable及Serializable"
[168]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/PopupWindow%E7%BB%86%E8%8A%82.md   "PopupWindow细节"
[169]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Scroller%E7%AE%80%E4%BB%8B.md   "Scroller简介"
[170]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/ScrollingTabs.md   "ScrollingTabs"
[171]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/SDK%20Manager%E6%97%A0%E6%B3%95%E6%9B%B4%E6%96%B0%E7%9A%84%E9%97%AE%E9%A2%98.md   "SDK Manager无法更新的问题"
[172]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Selector%E4%BD%BF%E7%94%A8.md   "Selector使用"
[173]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/SlidingMenu.md   "SlidingMenu"
[174]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/String%E6%A0%BC%E5%BC%8F%E5%8C%96.md   "String格式化"
[175]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/TextView%E8%B7%91%E9%A9%AC%E7%81%AF%E6%95%88%E6%9E%9C.md   "TextView跑马灯效果"
[176]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/WebView%E6%80%BB%E7%BB%93.md   "WebView总结"
[177]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Widget(%E7%AA%97%E5%8F%A3%E5%B0%8F%E9%83%A8%E4%BB%B6).md   "Widget(窗口小部件)"
[178]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/Wifi%E7%8A%B6%E6%80%81%E7%9B%91%E5%90%AC.md   "Wifi状态监听"
[179]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/BasicKnowledge/XmlPullParser.md   "XmlPullParser"


[180]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E4%B8%80).md "Kotlin学习教程(一)"
[181]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E4%BA%8C).md "Kotlin学习教程(二)"
[182]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E4%B8%89).md "Kotlin学习教程(三)"
[183]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E5%9B%9B).md "Kotlin学习教程(四)"
[184]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E4%BA%94).md "Kotlin学习教程(五)"
[185]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E5%85%AD).md "Kotlin学习教程(六)"
[186]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E4%B8%83).md "Kotlin学习教程(七)"
[187]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E5%85%AB).md "Kotlin学习教程(八)"
[188]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E4%B9%9D).md "Kotlin学习教程(九)"
[189]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E5%85%AB%E7%A7%8D%E6%8E%92%E5%BA%8F%E7%AE%97%E6%B3%95.md "八种排序算法"
[190]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E7%BA%BF%E7%A8%8B%E6%B1%A0%E7%AE%80%E4%BB%8B.md "线程池简介"
[191]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F.md "设计模式"
[192]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E7%AE%97%E6%B3%95%E7%9A%84%E5%A4%8D%E6%9D%82%E5%BA%A6.md "算法复杂度"
[193]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/%E5%8A%A8%E6%80%81%E4%BB%A3%E7%90%86.md "动态代理"
[194]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/ConstraintLaayout%E7%AE%80%E4%BB%8B.md "ConstraintLaayout简介"
[195]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/Http%E4%B8%8EHttps%E7%9A%84%E5%8C%BA%E5%88%AB.md "Http与Https的区别"
[196]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/JavaKnowledge/Top-K%E9%97%AE%E9%A2%98.md "Top-K问题"
[197]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/KotlinCourse/Kotlin%E5%AD%A6%E4%B9%A0%E6%95%99%E7%A8%8B(%E5%8D%81).md "Kotlin学习教程(十)"
[198]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AppPublish/%E4%BD%BF%E7%94%A8Jenkins%E5%AE%9E%E7%8E%B0%E8%87%AA%E5%8A%A8%E5%8C%96%E6%89%93%E5%8C%85.md "使用Jenkins实现自动化打包"
[199]: https://github.com/pengMaster/BestNote/tree/master/docs/android/AndroidNote//Dagger2 "Dagger2"
[200]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Dagger2/1.Dagger2%E7%AE%80%E4%BB%8B(%E4%B8%80).md  "1.Dagger2简介(一).md"
[201]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Dagger2/2.Dagger2%E5%85%A5%E9%97%A8demo(%E4%BA%8C).md  "2.Dagger2入门demo(二).md"
[202]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Dagger2/3.Dagger2%E5%85%A5%E9%97%A8demo%E6%89%A9%E5%B1%95(%E4%B8%89).md  "3.Dagger2入门demo扩展(三).md"
[203]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Dagger2/4.Dagger2%E5%8D%95%E4%BE%8B(%E5%9B%9B).md  "4.Dagger2单例(四).md"
[204]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Dagger2/5.Dagger2Lay%E5%92%8CProvider(%E4%BA%94).md  "5.Dagger2Lay和Provider(五).md"
[205]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Dagger2/6.Dagger2Android%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81(%E5%85%AD).md  "6.Dagger2Android示例代码(六).md"
[206]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Dagger2/7.Dagger2%E4%B9%8Bdagger-android(%E4%B8%83).md  "7.Dagger2之dagger-android(七).md"
[207]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Dagger2/8.Dagger2%E4%B8%8EMVP(%E5%85%AB).md  "8.Dagger2与MVP(八).md"
[208]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/AdavancedPart/Android%20WorkManager.md  "Android WorkManager.md"

[209]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/RxJavaPart/4.RxJava%E8%AF%A6%E8%A7%A3%E4%B9%8B%E6%89%A7%E8%A1%8C%E5%8E%9F%E7%90%86(%E5%9B%9B).md  "4.RxJava详解之执行原理(四)"
[210]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/RxJavaPart/5.RxJava%E8%AF%A6%E8%A7%A3%E4%B9%8B%E6%93%8D%E4%BD%9C%E7%AC%A6%E6%89%A7%E8%A1%8C%E5%8E%9F%E7%90%86(%E4%BA%94).md  "5.RxJava详解之操作符执行原理(五)"
[211]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/RxJavaPart/6.RxJava%E8%AF%A6%E8%A7%A3%E4%B9%8B%E7%BA%BF%E7%A8%8B%E8%B0%83%E5%BA%A6%E5%8E%9F%E7%90%86(%E5%85%AD).md  "6.RxJava详解之线程调度原理(六)"
[212]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Dagger2/9.Dagger2%E5%8E%9F%E7%90%86%E5%88%86%E6%9E%90(%E4%B9%9D).md "9.Dagger2原理分析(九)"
[213]: https://github.com/pengMaster/BestNote/blob/master/docs/android/AndroidNote/Tools%26Library/%E8%B0%83%E8%AF%95%E5%B9%B3%E5%8F%B0Sonar.md "调试平台Sonar"
