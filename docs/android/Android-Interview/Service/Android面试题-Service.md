**Android面试题-Service是否在main thread中执行, service里面是否能执行耗时的操作?**

Service不是独立的进程，也不是独立的线程，它是依赖于应用程序的主线程的，也就是说，在更多时候不建议在Service中编写耗时的逻辑和操作（比如:网络请求，拷贝数据库，大文件），否则会引起ANR。

如果想在服务中执行耗时的任务。有以下解决方案：

1） 在service中开启一个子线程

```
new Thread(){}.start();
```

2） 可以使用IntentService异步管理服务
参考文章IntentService的使用：
[http://blog.csdn.net/mwq384807683/article/details/72549222](http://blog.csdn.net/mwq384807683/article/details/72549222)

Service 和 Activity 在同一个线程，对于同一 app 来说默认情况下是在同一个线程中的 main Thread (UI Thread)