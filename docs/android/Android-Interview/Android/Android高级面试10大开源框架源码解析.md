## Android高级面试，10大开源框架源码解析

编程最好的学习方法是阅读顶尖工程师的源码！本课程将带你深度剖析Android主流开源框架的源码，让你全面掌握框架的使用场景、内部机制、构造原理、核心类、架构与设计思想等，提升你的代码阅读与分析能力、提高代码设计能力及改造能力，快速突破技术瓶颈，轻松应对Android高级面试与技术难题！ 

<!--more-->

## 课程章节

### 第1章 课程介绍

编程最好的学习方法是阅读顶级工程师的源码！本课程将带你深度剖析Android主流开源框架的源码，让你全面掌握框架的使用场景、内部机制、构造原理、核心类、架构与设计思想等，提升你的代码阅读与分析能力、提高代码设计能力及改造能力，快速突破技术瓶颈，轻松应对Android高级面试与技术难题！ ...

- 1-1 课程导学

### 第2章 Okhttp网络库深入解析和相关面试题分析

本章主要先通过分析OKhttp的简单使用，对于OKhttp的调度器、拦截器、缓存策略、连接池等进行了相应的源码和原理分析，并对于socket、websocket、http缓存、多线程下载、文件下载、https等经典Android面试题进行分析。

- 2-1 okhttp框架流程分析
- 2-2 okhttp同步请求方法
- 2-3 okhttp异步请求方法
- 2-4 okhttp同步请求流程和源码分析
- 2-5 okhttp异步请求流程和源码分析-1
- 2-6 okhttp异步请求流程和源码分析-2
- 2-7 okhttp任务调度核心类dispatcher解析-1
- 2-8 okhttp任务调度核心类dispatcher解析-2
- 2-9 okhttp拦截器流程
- 2-10 okhttp拦截器链介绍
- 2-11 okhttp之RetryAndFollowUpInterceptor解析
- 2-12 okhttp之BridgeInterceptor解析
- 2-13 okhttp缓存策略源码分析：put方法
- 2-14 okhttp缓存策略源码分析：get方法
- 2-15 okhttp拦截器之CacheInterceptor解析
- 2-16 okhttp拦截器之ConnectInterceptor解析-1
- 2-17 okhttp拦截器之ConnectInterceptor解析-2
- 2-18 okhttp连接池：put,get方法
- 2-19 okhttp连接池：connection回收
- 2-20 okhttp拦截器之CallServerInterceptor解析
- 2-21 okhttp面试: Socket-1
- 2-22 okhttp面试: Socket-2
- 2-23 okhttp面试: HttpClient&HttpUrlConnection
- 2-24 okhttp面试: OkHttp来实现WebSocket连接
- 2-25 okhttp面试: WebSocket&轮询相关
- 2-26 okhttp面试: Http缓存、Etag等标示作用
- 2-27 okhttp面试: 断点续传原理&Okhttp如何实现
- 2-28 okhttp面试：多线程下载
- 2-29 okhttp面试：文件上传&Okhttp如何处理文件上传
- 2-30 okhttp面试：如何解析Json类型数据
- 2-31 okhttp面试：Https／对称加密&不对称加密

### 第3章 Retrofit网络库深入解析和相关面试题分析

本章主要先通过分析retrofit的使用，对于retrofit的接口、动态代理、适配工厂、数据转换等进行相应的源码和原理分析，并对于retrofit的设计模式、线程切换、Hook、MVC和MVP架构、SP跨进程问题等经典Android面试题进行分析。

- 3-1 retrofit流程分析
- 3-2 retrofit概述
- 3-3 retrofit官网例子解析
- 3-4 retrofit请求过程7步骤详解
- 3-5 静态代理模式讲解
- 3-6 动态代理模式讲解
- 3-7 retrofit网络通信流程8步骤&7个关键成员变量解析
- 3-8 retrofit中builder构建者模式&builder内部类解析
- 3-9 retrofit中baseurl／converter／calladapter解析
- 3-10 retrofit中build方法完成retrofit对象创建流程解析
- 3-11 retrofit中RxjavaCallAdapterFactory内部构造与工作原理解析
- 3-12 retrofit中网络请求接口实例解析
- 3-13 retrofit中serviceMethod对象解析
- 3-14 retrofit中okHttpCall对象和adapt返回对象解析
- 3-15 retrofit中同步请求&重要参数解析
- 3-16 retrofit中异步请求解析
- 3-17 retrofit设计模式解析-1：构建者模式
- 3-18 retrofit设计模式解析-2：工厂模式
- 3-19 retrofit设计模式解析-3：外观模式
- 3-20 retrofit设计模式解析-4：策略模式
- 3-21 retrofit设计模式解析-5：适配器模式
- 3-22 retrofit设计模式解析-6：动态代理模式／观察者
- 3-23 retrofit面试题：retfrofit线程切换（异步机制Looper)
- 3-24 retrofit面试题：rxjava和retrofit如何结合进行网络请求
- 3-25 retrofit面试题：Hook与动态代理
- 3-26 retrofit面试题：Android MVC架构优势和缺点
- 3-27 retrofit面试题：MVP优点和缺点
- 3-28 retrofit面试题：sp跨进程&apply和commit方法

### 第4章 Glide图片库深入解析和相关面试题分析

本章主要先通过分析Glide的使用，对于glide的内存和硬盘缓存、加载策略、如何进行图片网络请求等方面，并将重点放在梳理整个Glide请求的流程，最后对于bitmap、性能优化OOM和三级缓存、Lrucache等Android面试题进行分析。

- 4-1 glide框架流程分析
- 4-2 glide框架介绍-1
- 4-3 glide框架介绍-2
- 4-4 glide图片加载流程和源码分析-1：with方法（requestManager获取)
- 4-5 glide图片加载流程和源码分析-2：with方法（requestManagerRetriever的get方法)
- 4-6 glide图片加载流程和源码分析-3：load方法
- 4-7 glide图片加载流程和源码分析-4：into方法（buildTarget）
- 4-8 glide图片加载流程和源码分析-5：into方法（request建立和begin方法）
- 4-9 glide图片加载流程和源码分析-6：into方法（Loadprovider）
- 4-10 glide图片加载流程和源码分析-7：into方法（硬盘缓存／内存缓存)
- 4-11 glide图片加载流程和源码分析-8：into方法（内存缓存的读取）
- 4-12 glide图片加载流程和源码分析-9：into方法（内存缓存的写入）
- 4-13 Glide面试一：bitmap&oom&优化bitmap
- 4-14 Glide面试二：三级缓存&lrucache

### 第5章 LeakCanary内存泄漏框架解析和相关面试题分析

本章主要先通过leakcanary使用，然后分析内存泄漏产生原因，并对于Leakcanary如何进行泄漏Activity收集策略、转换内存快照、定位内存泄漏位置等分析，最后对于现在业界比较关心的UI流畅度和性能数据上报等进行对应分析。

- 5-1 leakcanary预备知识：android性能优化&Gcroots
- 5-2 leakcanary内存框架：内存泄漏基础&为什么需要leakcanary
- 5-3 android常见内存泄漏分析-1：单例VS非静态内部类
- 5-4 android常见内存泄漏分析-2：handler&解决办法
- 5-5 android常见内存泄漏分析-3：线程&WebView
- 5-6 leakcanary原理分析-1：Leakcanary原理概述和弱引用／引用队列
- 5-7 leakcanary原理分析-2：ActivityRefWatcher如何监视Activity
- 5-8 leakcanary原理分析-3：.hprof转换snapshot
- 5-9 leakcanary原理分析-4：查找内存泄漏引用和最短泄漏路径
- 5-10 leakcanary面试题：Application&内存
- 5-11 leakcanary面试题：性能数据上报：网络流量和冷启动
- 5-12 leakcanary面试题：性能数据上报：UI卡顿和内存占用

### 第6章 butterknife依赖注入框架源码解析

本章从butterknife的基本使用讲起，首先会介绍框架相关注解和APT知识点，然后开始逐步分析butterknife源码，并逐步理清butterknife注入框架的原理，最后提炼butterknife中有关android面试相关问题。

- 6-1 butterknife的引言和基本使用
- 6-2 butterknife原理必备知识点1：注解
- 6-3 butterknife原理必备知识点2：APT工作原理
- 6-4 butterknife原理必备知识点3：反射+运行时注解举例
- 6-5 butterknife原理分析-1：注解处理器如何处理注解和保存注解
- 6-6 butterknife原理分析-2：如何生成findviewByID代码

### 第7章 blockcanary UI卡顿优化框架源码解析

本章会从blockcanary基本使用讲起，首先会简单介绍ActivityThread／handler／looper相关框架知识点，然后通过分析blockcanary源码，逐步理清blockcanary如何解决UI卡顿的原理，最后会提炼blockcanary中有关android面试相关问题,并总结android性能优化相关问题。...

- 7-1 blockcanary背景／UI卡顿原理／UI卡顿常见原因
- 7-2 blockcanary使用／阀值参数
- 7-3 blockcanary核心原理实现和流程图简述
- 7-4 blockcanary源码解析-1：框架初始化
- 7-5 blockcanary源码解析-2：stacksampler／cpusampler／start方法
- 7-6 blockcanary面试一：anr场景／原因／解决
- 7-7 blockcanary面试二：watchdog-anr 如何检测anr
- 7-8 blockcanary面试三：new Thread开启线程的4点弊端
- 7-9 blockcanary面试四：线程间通信：子线程--UI线程
- 7-10 blockcanary面试五：主线程--子线程(handlerThread-IntentService)
- 7-11 blockcanary面试六：多进程的4点好处与问题／voliate关键字
- 7-12 blockcanary面试七：voliate关键字和单例的写法

### 第8章 eventbus异步框架源码解析

本章会从eventbus的基本用法开始讲起，主要包括Event、Subscriber、Publisher、ThreadMode几大部分，并结合handler、组件间传递等消息知识点深入分析，然后对比分析eventbus3.0和2.0的区别，并结合eventbus在android面试中遇到的高频问题，对eventbus框架进行总结。...

- 8-1 eventbus框架核心概念：事件传递／EventBus的优点／传统handler通信的两种方式
- 8-2 eventbus框架基本用法
- 8-3 eventbus框架源码解析-1：EventBus对象构建／如何进行线程调度
- 8-4 eventbus框架源码解析-2 subscribe注解／threadMode
- 8-5 eventbus框架源码解析-3：register订阅(上)
- 8-6 eventbus框架源码解析-4：register订阅（中）
- 8-7 eventbus框架源码解析-5：register订阅（下）
- 8-8 eventbus框架源码解析-6：subscribe方法完成订阅（上）
- 8-9 eventbus框架源码解析-7：subscribe方法完成订阅（下）
- 8-10 eventbus框架源码解析-8：发送事件post

### 第9章 dagger2依赖注入框架源码解析

本章从dagger2的基本使用讲起，首先会介绍框架相关依赖注入的知识点，然后逐步分析dagger2源码，并逐步理清dagger2注入框架原理，并对比分析dagger2与dagger的区别，最后会根据android面试相关问题，给大家总结dagger2的相关知识点。

- 9-1 dagger2引言：依赖注入和使用场景
- 9-2 dagger2四种注入方式和依赖注入总结
- 9-3 dagger2的四种基本注解：@inject注解
- 9-4 dagger2的四种基本注解：@component注解
- 9-5 dagger2的inject和component注解实例和源码分析
- 9-6 dagger2的@Module和@Provides注解
- 9-7 dagger2的@Module和@Provides注解实例和代码分析

### 第10章 rxjava异步框架源码解析

本章会从rxjava的基本使用讲起：主要包括观察者模式、操作符、线程控制等，然后逐步分析rxjava中的响应式编程原理，最后会结合rxjava在android面试中遇到的高频面试问题，给大家总结rxjava相关知识。

- 10-1 rxjava基本用法和观察者模式：01-传统观察者模式
- 10-2 rxjava观察者模式和基本用法
- 10-3 rxjava如何创建Observable&observer／subscriber
- 10-4 rxjava如何创建subscriber以及如何完成订阅
- 10-5 rxjava操作符之map基本使用
- 10-6 rxjava操作符之map源码探究：lift
- 10-7 rxjava操作符之flatmap
- 10-8 rxjava线程控制：多线程编程准则&Rxjava如何处理多线程&&Schedulers
- 10-9 rxjava线程控制：两个小例子&observeOn和SubscribeOn
- 10-10 rxjava线程控制：SubscribeOn源码剖析
- 10-11 rxjava线程控制：ObserveOn源码剖析&&subscribeOn可以调用几次

### 第11章 picasso图片框架源码解析

本章从picasso基本用法和配置讲起，逐步分析picasso的源码，并从DownLoader，Dispatcher,service线程池等核心类进行分析，最后根据picasso流程图进行总结，并给大家提炼android面试中有关picasso框架的问题。

- 11-1 picasso框架基本使用API
- 11-2 picasso源码with方法：内存缓存Lrucache和线程池的调度
- 11-3 piacsso源码with：dispatcher如何完成线程切换
- 11-4 picasso源码with：NetworkRequestHandler处理图片请求和回调
- 11-5 picasso源码load方法
- 11-6 picasso源码into方法：Action&BitmapHunter
- 11-7 picasso源码into方法：线程池&PicassoFutureTask
- 11-8 picasso源码into：线程开启如何执行图片加载请求？
- 11-9 picasso源码into：Okhttp和UrlConnectionDownloader下载图片
- 11-10 picasso源码into方法：完成加载

### 第12章 课程总结

本章将通过对Android面试技巧的梳理，帮助大家整体的认知和提高Android面试能力以及需要做的面试准备等，希望能对大家的面试有所帮助！最后非常感谢大家对课程的认可和支持，祝愿你们都能找到好工作。收到你们的Offer消息，是做好这门课程最大的动力。...

- 12-1 Android面试技巧梳理