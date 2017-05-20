### 关于Service
* [知道Service吗，它有几种启动方式？](http://www.jianshu.com/p/7a7db9f8692d)
* Service是一个专门在后台处理长时间任务的Android组件，它没有UI。它有两种启动方式，startService和bindService。
* 这两种启动方式的区别:</br>
startService只是启动Service，启动它的组件（如Activity）和Service并没有关联，只有当Service调用stopSelf或者其他组件调用stopService服务才会终止。</br>
bindService方法启动Service，其他组件可以通过回调获取Service的代理对象和Service交互，而这两方也进行了绑定，当启动方销毁时，Service也会自动进行unBind操作，当发现所有绑定都进行了unBind时才会销毁Service。
	
![](http://upload-images.jianshu.io/upload_images/1685558-5b9c3263c0af2ea2.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* Service的onCreate是在主线程（ActivityThread）中调用的，耗时操作会阻塞UI
* 如果需要做耗时的操作，你会怎么做？
Handler
* 场景：如果一个应用要从网络上下载MP3文件，并在Activity上展示进度条，这个Activity要求是可以转屏的。那么在转屏时Actvitiy会重启，如何保证下载的进度条能正确展示进度呢？
* IntentService
* Activity（UI）和Service的交互
