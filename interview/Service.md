
<!DOCTYPE html>
<!--[if IE 6]><html class="ie lt-ie8"><![endif]-->
<!--[if IE 7]><html class="ie lt-ie8"><![endif]-->
<!--[if IE 8]><html class="ie ie8"><![endif]-->
<!--[if IE 9]><html class="ie ie9"><![endif]-->
<!--[if !IE]><!--> <html> <!--<![endif]-->

<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=Edge">
<script type="text/javascript">window.NREUM||(NREUM={});NREUM.info={"beacon":"bam.nr-data.net","errorBeacon":"bam.nr-data.net","licenseKey":"1255494d3a","applicationID":"15702971","transactionName":"e1daR0JWVV9RER9ZWkxdRxxDUVZE","queueTime":19,"applicationTime":37,"agent":""}</script>
<script type="text/javascript">window.NREUM||(NREUM={}),__nr_require=function(e,n,t){function r(t){if(!n[t]){var o=n[t]={exports:{}};e[t][0].call(o.exports,function(n){var o=e[t][1][n];return r(o||n)},o,o.exports)}return n[t].exports}if("function"==typeof __nr_require)return __nr_require;for(var o=0;o<t.length;o++)r(t[o]);return r}({1:[function(e,n,t){function r(){}function o(e,n,t){return function(){return i(e,[c.now()].concat(u(arguments)),n?null:this,t),n?void 0:this}}var i=e("handle"),a=e(2),u=e(3),f=e("ee").get("tracer"),c=e("loader"),s=NREUM;"undefined"==typeof window.newrelic&&(newrelic=s);var p=["setPageViewName","setCustomAttribute","setErrorHandler","finished","addToTrace","inlineHit","addRelease"],d="api-",l=d+"ixn-";a(p,function(e,n){s[n]=o(d+n,!0,"api")}),s.addPageAction=o(d+"addPageAction",!0),s.setCurrentRouteName=o(d+"routeName",!0),n.exports=newrelic,s.interaction=function(){return(new r).get()};var m=r.prototype={createTracer:function(e,n){var t={},r=this,o="function"==typeof n;return i(l+"tracer",[c.now(),e,t],r),function(){if(f.emit((o?"":"no-")+"fn-start",[c.now(),r,o],t),o)try{return n.apply(this,arguments)}finally{f.emit("fn-end",[c.now()],t)}}}};a("setName,setAttribute,save,ignore,onEnd,getContext,end,get".split(","),function(e,n){m[n]=o(l+n)}),newrelic.noticeError=function(e){"string"==typeof e&&(e=new Error(e)),i("err",[e,c.now()])}},{}],2:[function(e,n,t){function r(e,n){var t=[],r="",i=0;for(r in e)o.call(e,r)&&(t[i]=n(r,e[r]),i+=1);return t}var o=Object.prototype.hasOwnProperty;n.exports=r},{}],3:[function(e,n,t){function r(e,n,t){n||(n=0),"undefined"==typeof t&&(t=e?e.length:0);for(var r=-1,o=t-n||0,i=Array(o<0?0:o);++r<o;)i[r]=e[n+r];return i}n.exports=r},{}],4:[function(e,n,t){n.exports={exists:"undefined"!=typeof window.performance&&window.performance.timing&&"undefined"!=typeof window.performance.timing.navigationStart}},{}],ee:[function(e,n,t){function r(){}function o(e){function n(e){return e&&e instanceof r?e:e?f(e,u,i):i()}function t(t,r,o,i){if(!d.aborted||i){e&&e(t,r,o);for(var a=n(o),u=m(t),f=u.length,c=0;c<f;c++)u[c].apply(a,r);var p=s[y[t]];return p&&p.push([b,t,r,a]),a}}function l(e,n){v[e]=m(e).concat(n)}function m(e){return v[e]||[]}function w(e){return p[e]=p[e]||o(t)}function g(e,n){c(e,function(e,t){n=n||"feature",y[t]=n,n in s||(s[n]=[])})}var v={},y={},b={on:l,emit:t,get:w,listeners:m,context:n,buffer:g,abort:a,aborted:!1};return b}function i(){return new r}function a(){(s.api||s.feature)&&(d.aborted=!0,s=d.backlog={})}var u="nr@context",f=e("gos"),c=e(2),s={},p={},d=n.exports=o();d.backlog=s},{}],gos:[function(e,n,t){function r(e,n,t){if(o.call(e,n))return e[n];var r=t();if(Object.defineProperty&&Object.keys)try{return Object.defineProperty(e,n,{value:r,writable:!0,enumerable:!1}),r}catch(i){}return e[n]=r,r}var o=Object.prototype.hasOwnProperty;n.exports=r},{}],handle:[function(e,n,t){function r(e,n,t,r){o.buffer([e],r),o.emit(e,n,t)}var o=e("ee").get("handle");n.exports=r,r.ee=o},{}],id:[function(e,n,t){function r(e){var n=typeof e;return!e||"object"!==n&&"function"!==n?-1:e===window?0:a(e,i,function(){return o++})}var o=1,i="nr@id",a=e("gos");n.exports=r},{}],loader:[function(e,n,t){function r(){if(!x++){var e=h.info=NREUM.info,n=d.getElementsByTagName("script")[0];if(setTimeout(s.abort,3e4),!(e&&e.licenseKey&&e.applicationID&&n))return s.abort();c(y,function(n,t){e[n]||(e[n]=t)}),f("mark",["onload",a()+h.offset],null,"api");var t=d.createElement("script");t.src="https://"+e.agent,n.parentNode.insertBefore(t,n)}}function o(){"complete"===d.readyState&&i()}function i(){f("mark",["domContent",a()+h.offset],null,"api")}function a(){return E.exists&&performance.now?Math.round(performance.now()):(u=Math.max((new Date).getTime(),u))-h.offset}var u=(new Date).getTime(),f=e("handle"),c=e(2),s=e("ee"),p=window,d=p.document,l="addEventListener",m="attachEvent",w=p.XMLHttpRequest,g=w&&w.prototype;NREUM.o={ST:setTimeout,CT:clearTimeout,XHR:w,REQ:p.Request,EV:p.Event,PR:p.Promise,MO:p.MutationObserver};var v=""+location,y={beacon:"bam.nr-data.net",errorBeacon:"bam.nr-data.net",agent:"js-agent.newrelic.com/nr-1026.min.js"},b=w&&g&&g[l]&&!/CriOS/.test(navigator.userAgent),h=n.exports={offset:u,now:a,origin:v,features:{},xhrWrappable:b};e(1),d[l]?(d[l]("DOMContentLoaded",i,!1),p[l]("load",r,!1)):(d[m]("onreadystatechange",o),p[m]("onload",r)),f("mark",["firstbyte",u],null,"api");var x=0,E=e(4)},{}]},{},["loader"]);</script>
  <meta name="viewport" content="width=device-width, initial-scale=1.0,user-scalable=no">
  <meta http-equiv="Cache-Control" content="no-siteapp" />
    <meta name="description"  content="前言我从2009年开始接触Android开发（SDK1.6），然后一直在Android这条路上痛并快乐地颠簸顽抗至今。一算也有6年光景了，6年中参加过不同公司的面试，也同样面试过不同公司跳槽来的人，想想自己也算Android开发中骨灰级的面霸了。仿佛已老，老是开始回忆一些以前的面试经历，所以干脆写下来，用自己经历给大家展示一下面试者和面试官两个人会怎么对待同一个问题的。面试题：知道Servi...">
  <meta property="wb:webmaster" content="294ec9de89e7fadb" />
  <meta property="qc:admins" content="104102651453316562112116375" />
  <meta property="qc:admins" content="11635613706305617" />
  <meta property="qc:admins" content="1163561616621163056375" />
  <meta name="google-site-verification" content="cV4-qkUJZR6gmFeajx_UyPe47GW9vY6cnCrYtCHYNh4" />
  <meta name="google-site-verification" content="HF7lfF8YEGs1qtCE-kPml8Z469e2RHhGajy6JPVy5XI" />
  <meta http-equiv="mobile-agent" content="format=html5; url=http://www.jianshu.com/p/7a7db9f8692d">

  <!-- Apple -->
  <meta name="apple-mobile-web-app-title" content="简书">

    <!--  Meta for Smart App Banner -->
  <meta name="apple-itunes-app" content="app-id=888237539, app-argument=jianshu://notes/3958460">
  <!-- End -->

  <!--  Meta for Twitter Card -->
  <meta content="summary" property="twitter:card">
  <meta content="@jianshucom" property="twitter:site">
  <meta content="Android面试一天一题（1 Day）" property="twitter:title">
  <meta content="前言我从2009年开始接触Android开发（SDK1.6），然后一直在Android这条路上痛并快乐地颠簸顽抗至今。一算也有6年光景了，6年中参加过不同公司的面试，也同样面试过不同公司跳槽来的人，想想自己也算Android开发中骨灰级的面霸了。仿佛已老，老是开始回忆一些以前的面试经历，所以干脆写下来，用自己经历给大家展示一下面试者和面试官两个人会怎么对待同一个问题的。面试题：知道Service吗，它有几种启动方式？这是我印象深刻的一道题，很明显它是我的第一次，那时我去一家公司（暂时叫它T公司吧）面试外派到韩国三星的工作机会。T公司的面试官是一个叫Bely架构师，显然那..." property="twitter:description">
  <meta content="http://www.jianshu.com/p/7a7db9f8692d" property="twitter:url">
  <!-- End -->

  <!--  Meta for OpenGraph -->
  <meta property="fb:app_id" content="865829053512461">
  <meta property="og:site_name" content="简书">
  <meta property="og:title" content="Android面试一天一题（1 Day）">
  <meta property="og:type" content="article">
  <meta property="og:url" content="http://www.jianshu.com/p/7a7db9f8692d">
  <meta property="og:description" content="前言我从2009年开始接触Android开发（SDK1.6），然后一直在Android这条路上痛并快乐地颠簸顽抗至今。一算也有6年光景了，6年中参加过不同公司的面试，也同样面试过不同公司跳槽来的...">
  <!-- End -->

  <!--  Meta for Facebook Applinks -->
  <meta property="al:ios:url" content="jianshu://notes/3958460" />
  <meta property="al:ios:app_store_id" content="888237539" />
  <meta property="al:ios:app_name" content="简书" />

  <meta property="al:android:url" content="jianshu://notes/3958460" />
  <meta property="al:android:package" content="com.jianshu.haruki" />
  <meta property="al:android:app_name" content="简书" />
  <!-- End -->


    <title>Android面试一天一题（1 Day） - 简书</title>

  <meta name="csrf-param" content="authenticity_token" />
<meta name="csrf-token" content="eJHMf5J2/xVnkaBZ8q4Ae1tJW83iME2T6ch2ZCt5YyzxxIUU0dofCNJgjUC1N+JmdthIkoAMbPz/K/jw9Qxn0w==" />

  <link rel="stylesheet" media="all" href="//cdn2.jianshu.io/assets/web-b5a90e7297a723b82f9e.css" />
  
  <link rel="stylesheet" media="all" href="//cdn2.jianshu.io/assets/web/pages/notes/show/entry-b5a90e7297a723b82f9e.css" />

  <link href="//cdn2.jianshu.io/assets/favicons/favicon-783beb88ed621ceab614de960376ac0c.ico" rel="icon">
      <link rel="apple-touch-icon-precomposed" href="//cdn2.jianshu.io/assets/apple-touch-icons/57-47624b2e2161e8eb144462c85db0a5ff.png" sizes="57x57" />
      <link rel="apple-touch-icon-precomposed" href="//cdn2.jianshu.io/assets/apple-touch-icons/72-c00cde7cf98fc49e50cbb3ee1dcd5804.png" sizes="72x72" />
      <link rel="apple-touch-icon-precomposed" href="//cdn2.jianshu.io/assets/apple-touch-icons/76-e8af0bdeaf1ba31e303b1fde8b5e66c4.png" sizes="76x76" />
      <link rel="apple-touch-icon-precomposed" href="//cdn2.jianshu.io/assets/apple-touch-icons/114-f4c78569bbf1977e8382a5fd90c9237a.png" sizes="114x114" />
      <link rel="apple-touch-icon-precomposed" href="//cdn2.jianshu.io/assets/apple-touch-icons/120-cf10c3711dba269522743729efe66bbc.png" sizes="120x120" />
      <link rel="apple-touch-icon-precomposed" href="//cdn2.jianshu.io/assets/apple-touch-icons/152-7bd60457b5f3ecbf1343f0e6241be4f8.png" sizes="152x152" />
</head>

  <body lang="zh-CN" class="reader-black-font">
    <!-- 全局顶部导航栏 -->
<nav class="navbar navbar-default navbar-fixed-top" role="navigation">
  <div class="width-limit">
    <!-- 左上方 Logo -->
    <a class="logo" href="/"><img src="//cdn2.jianshu.io/assets/web/logo-58fd04f6f0de908401aa561cda6a0688.png" alt="Logo" /></a>

    <!-- 右上角 -->
      <!-- 未登录显示登录/注册/写文章 -->
      <a class="btn write-btn" target="_blank" href="/writer#/">
        <i class="iconfont ic-write"></i>写文章
</a>      <a class="btn sign-up" href="/sign_up">注册</a>
      <a class="btn log-in" href="/sign_in">登录</a>

    <!-- 如果用户登录，显示下拉菜单 -->

    <div id="view-mode-ctrl">
    </div>
    <div class="container">
      <div class="navbar-header">
        <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#menu" aria-expanded="false">
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
        </button>
      </div>
      <div class="collapse navbar-collapse" id="menu">
        <ul class="nav navbar-nav">
            <li class="">
              <a href="/">
                <span class="menu-text">首页</span><i class="iconfont ic-navigation-discover menu-icon"></i>
</a>            </li>
            <li class="">
              <a class="app-download-btn" href="/apps"><span class="menu-text">下载App</span><i class="iconfont ic-navigation-download menu-icon"></i></a>
            </li>
          <li class="search">
            <form target="_blank" action="/search" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="&#x2713;" />
              <input type="text" name="q" id="q" value="" placeholder="搜索" class="search-input" />
              <a class="search-btn" href="javascript:void(null)"><i class="iconfont ic-search"></i></a>
              <!-- <div id="navbar-trending-search"></div> -->
</form>          </li>
        </ul>
      </div>
    </div>
  </div>
</nav>

    
<div class="note">
  <div class="post">
    <div class="article">
        <h1 class="title">Android面试一天一题（1 Day）</h1>

        <!-- 作者区域 -->
        <div class="author">
          <a class="avatar" href="/u/f9fbc7a39b36">
            <img src="//upload.jianshu.io/users/upload_avatars/1685558/55985a8c0e1f.jpg?imageMogr2/auto-orient/strip|imageView2/1/w/144/h/144" alt="144" />
</a>          <div class="info">
            <span class="tag">作者</span>
            <span class="name"><a href="/u/f9fbc7a39b36">goeasyway</a></span>
            <!-- 关注用户按钮 -->
            <div data-author-follow-button></div>
            <!-- 文章数据信息 -->
            <div class="meta">
              <!-- 如果文章更新时间大于发布时间，那么使用 tooltip 显示更新时间 -->
                <span class="publish-time" data-toggle="tooltip" data-placement="bottom" title="最后编辑于 2016.05.16 20:50">2016.05.16 20:32*</span>
              <span class="wordage">字数 1456</span>
            </div>
          </div>
          <!-- 如果是当前作者，加入编辑按钮 -->
        </div>
        <!-- -->

        <!-- 文章内容 -->
        <div class="show-content">
          <h3>前言</h3>
<p>我从2009年开始接触Android开发（SDK1.6），然后一直在Android这条路上痛并快乐地颠簸顽抗至今。一算也有6年光景了，6年中参加过不同公司的面试，也同样面试过不同公司跳槽来的人，想想自己也算Android开发中骨灰级的面霸了。仿佛已老，老是开始回忆一些以前的面试经历，所以干脆写下来，用自己经历给大家展示一下面试者和面试官两个人会怎么对待同一个问题的。</p>
<h2>面试题：知道Service吗，它有几种启动方式？</h2>
<p>这是我印象深刻的一道题，很明显它是我的第一次，那时我去一家公司（暂时叫它T公司吧）面试外派到韩国三星的工作机会。T公司的面试官是一个叫Bely架构师，显然那个时候Android开发是稀缺资源，知道Service那都不得了了，当然Bely也没打算为难我（必竟也工作4年多了，人长得也不错），我轻松对答：</p>
<blockquote><p>Service是一个专门在后台处理长时间任务的Android组件，它没有UI。它有两种启动方式，startService和bindService。</p></blockquote>
<p>你猜得没错，Bely紧接着问我：这两种启动方式的区别。</p>
<blockquote><p><strong>startService</strong>只是启动Service，启动它的组件（如Activity）和Service并没有关联，只有当Service调用stopSelf或者其他组件调用stopService服务才会终止。<br><strong>bindService</strong>方法启动Service，其他组件可以通过回调获取Service的代理对象和Service交互，而这两方也进行了绑定，当启动方销毁时，Service也会自动进行unBind操作，当发现所有绑定都进行了unBind时才会销毁Service。</p></blockquote>
<p>这应该是比较关键的区别了，在面试前我刚刚用Serivce做过一个音乐播放器。几年后，我在深圳面试过很多人，他们中有60-70%的人没有使用Service的经验，让我一度感觉得深圳这座城市做Android开发的比较浮躁。因为这儿工作机会太多了，初级的开发者都比较急功近利，不需要在自己身上下太多的功夫也可以找到工作（当然这是片面的认识）。</p>
<p>当然还有其他的区别，如两种调用对Service生命周期函数影响，面试官也可以就这个问题展开一下。<br></p><div class="image-package">
<img src="http://upload-images.jianshu.io/upload_images/1685558-5b9c3263c0af2ea2.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240" data-original-src="http://upload-images.jianshu.io/upload_images/1685558-5b9c3263c0af2ea2.png?imageMogr2/auto-orient/strip%7CimageView2/2"><br><div class="image-caption"></div>
</div>
<p>当我遇到面试者知道怎么使用Service，也如多年前的我可以自如的答出startService和bindService的区别时，我一般会多问一句：</p>
<blockquote><p>Service的onCreate回调函数可以做耗时的操作吗？</p></blockquote>
<p>很多人都会说：可以。</p>
<p>原形毕露，他前面的回答只是在面试前预习了一下面试题而已。如果知道Service的onCreate是在主线程（ActivityThread）中调用的，耗时操作会阻塞UI，我一般再接着问：</p>
<blockquote><p>如果需要做耗时的操作，你会怎么做？</p></blockquote>
<p>问题便这样展开了，一个人是否真正懂得原理会灵活运用，一下子便能看出来。 当面试者回答到线程和Handler方式时，我会再问一下对方:</p>
<blockquote><p>是否知道IntentService，在什么场景下使用IntentService？</p></blockquote>
<p>这也是面试官要看的点，真正的项目需要一个开发人员对某个问题有一定的深度，也需要对整个Android的知识点有一定的广度。深度代表这个人对问题认真对待有钻研的精神，广度代表这个人在面对同一个问题时，会更容易从多种可行的方案中选出最合适的一种。</p>
<p>Service的实际项目中一直被很多人忽略，为什么我一再强调Service很重要，我们来看看，如果对Service完全无知会在工作中遇到什么问题。</p>
<blockquote><p>场景：如果一个应用要从网络上下载MP3文件，并在Activity上展示进度条，这个Activity要求是可以转屏的。那么在转屏时Actvitiy会重启，如何保证下载的进度条能正确展示进度呢？</p></blockquote>
<p>没有Service概念的人，一般想出来的方案如下：</p>
<ol>
<li>在转屏前将进度缓存，转屏后再读出来。</li>
<li>使用android:configChanges设置，让转屏时Activity不销毁和重建。</li>
</ol>
<p>针对第1个方案，我会继续问他将进度值存在哪里？ 转屏的过程中，我们知道Activity的重建算是比较耗时的，会可能会有几百毫秒以上，那么这时候下载线程仍然在工作，进度肯定和保存时的进度不一致了，如何处理这个问题呢？</p>
<p>第2个方案，大家可以自己展开思考，实际的项目中可能会需要额外做一些事情来处理ContentView的横竖布局的问题。</p>
<p>如果使用Service来解决这个问题，看似是比较完美的，不过就会涉及Activity（UI）和Service的交互问题，这个我们以后再讨论。</p>
<h2>小结</h2>
<p>当我们知道了Service的用途，心中有一个Service相关的概念时，针对实际的场景还是要做具体的分析再决定是否使用Service。因为Service仍然是在主线程中调用，还是要开线程才能处理长时间的工作，Service和UI的交互也让这个方式变得不那么简便。如果你只需要在当前界面去做一些耗时操作，界面退出或改变时，工作也要停止，那么这时直接使用Thread（或者AsyncTask, ThreadHandler）会更合适你。</p>

        </div>
        <!--  -->

        <div class="show-foot">
          <a class="notebook" href="/nb/3450453">
            <i class="iconfont ic-search-notebook"></i> <span>Android面试</span>
</a>          <div class="copyright" data-toggle="tooltip" data-html="true" data-original-title="转载请联系作者获得授权，并标注“简书作者”。">
            © 著作权归作者所有
          </div>
          <div class="modal-wrap" data-report-note>
            <a id="report-modal">举报文章</a>
          </div>
        </div>
    </div>

    <!-- 文章底部作者信息 -->
      <div class="follow-detail">
        <div class="info">
          <a class="avatar" href="/u/f9fbc7a39b36">
            <img src="//upload.jianshu.io/users/upload_avatars/1685558/55985a8c0e1f.jpg?imageMogr2/auto-orient/strip|imageView2/1/w/144/h/144" alt="144" />
</a>          <div data-author-follow-button></div>
          <a class="title" href="/u/f9fbc7a39b36">goeasyway</a>
        </div>
          <div class="signature">
            <span>Even的移动开发博客，专注于Android和React Native开发。欢迎关注微信公众号...</span>
          </div>
      </div>

      <div class="support-author"></div>

    <div class="meta-bottom">
      <div class="btn like-group"></div>
      <div class="share-group">
        <a class="share-circle" data-action="weixin-share" data-toggle="tooltip" data-original-title="分享到微信">
          <i class="iconfont ic-wechat"></i>
        </a>
        <a class="share-circle" data-toggle="tooltip" href="javascript:void((function(s,d,e,r,l,p,t,z,c){var%20f=&#39;http://v.t.sina.com.cn/share/share.php?appkey=1881139527&#39;,u=z||d.location,p=[&#39;&amp;url=&#39;,e(u),&#39;&amp;title=&#39;,e(t||d.title),&#39;&amp;source=&#39;,e(r),&#39;&amp;sourceUrl=&#39;,e(l),&#39;&amp;content=&#39;,c||&#39;gb2312&#39;,&#39;&amp;pic=&#39;,e(p||&#39;&#39;)].join(&#39;&#39;);function%20a(){if(!window.open([f,p].join(&#39;&#39;),&#39;mb&#39;,[&#39;toolbar=0,status=0,resizable=1,width=440,height=430,left=&#39;,(s.width-440)/2,&#39;,top=&#39;,(s.height-430)/2].join(&#39;&#39;)))u.href=[f,p].join(&#39;&#39;);};if(/Firefox/.test(navigator.userAgent))setTimeout(a,0);else%20a();})(screen,document,encodeURIComponent,&#39;&#39;,&#39;&#39;,&#39;http://cwb.assets.jianshu.io/notes/images/3958460/weibo/image_73c5e58e9aac.jpg&#39;, &#39;推荐 @Android面试启示录 的文章《Android面试一天一题（1 Day）》（ 分享自 @简书 ）&#39;,&#39;http://www.jianshu.com/p/7a7db9f8692d?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=weibo&#39;,&#39;页面编码gb2312|utf-8默认gb2312&#39;));" data-original-title="分享到微博">
          <i class="iconfont ic-weibo"></i>
        </a>
          <a class="share-circle" data-toggle="tooltip" href="http://cwb.assets.jianshu.io/notes/images/3958460/weibo/image_73c5e58e9aac.jpg" target="_blank" data-original-title="下载长微博图片">
            <i class="iconfont ic-picture"></i>
          </a>
        <a class="share-circle more-share" tabindex="0" data-toggle="popover" data-placement="top" data-html="true" data-trigger="focus" href="javascript:void(0);" data-content='
          <ul class="share-list">
            <li><a href="javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;http://sns.qzone.qq.com/cgi-bin/qzshare/cgi_qzshare_onekey?url=&#39;+e(&#39;http://www.jianshu.com/p/7a7db9f8692d?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=qzone&#39;)+&#39;&amp;title=&#39;+e(&#39;推荐 goeasyway 的文章《Android面试一天一题（1 Day）》&#39;),x=function(){if(!window.open(r,&#39;qzone&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=600,height=600&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();"><i class="social-icon-sprite social-icon-zone"></i><span>分享到QQ空间</span></a></li>
            <li><a href="javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;https://twitter.com/share?url=&#39;+e(&#39;http://www.jianshu.com/p/7a7db9f8692d?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=twitter&#39;)+&#39;&amp;text=&#39;+e(&#39;推荐 goeasyway 的文章《Android面试一天一题（1 Day）》（ 分享自 @jianshucom ）&#39;)+&#39;&amp;related=&#39;+e(&#39;jianshucom&#39;),x=function(){if(!window.open(r,&#39;twitter&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=600,height=600&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();"><i class="social-icon-sprite social-icon-twitter"></i><span>分享到Twitter</span></a></li>
            <li><a href="javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;https://www.facebook.com/dialog/share?app_id=483126645039390&amp;display=popup&amp;href=http://www.jianshu.com/p/7a7db9f8692d?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=facebook&#39;,x=function(){if(!window.open(r,&#39;facebook&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=450,height=330&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();"><i class="social-icon-sprite social-icon-facebook"></i><span>分享到Facebook</span></a></li>
            <li><a href="javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;https://plus.google.com/share?url=&#39;+e(&#39;http://www.jianshu.com/p/7a7db9f8692d?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=google_plus&#39;),x=function(){if(!window.open(r,&#39;google_plus&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=450,height=330&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();"><i class="social-icon-sprite social-icon-google"></i><span>分享到Google+</span></a></li>
            <li><a href="javascript:void(function(){var d=document,e=encodeURIComponent,s1=window.getSelection,s2=d.getSelection,s3=d.selection,s=s1?s1():s2?s2():s3?s3.createRange().text:&#39;&#39;,r=&#39;http://www.douban.com/recommend/?url=&#39;+e(&#39;http://www.jianshu.com/p/7a7db9f8692d?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=douban&#39;)+&#39;&amp;title=&#39;+e(&#39;Android面试一天一题（1 Day）&#39;)+&#39;&amp;sel=&#39;+e(s)+&#39;&amp;v=1&#39;,x=function(){if(!window.open(r,&#39;douban&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=450,height=330&#39;))location.href=r+&#39;&amp;r=1&#39;};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})()"><i class="social-icon-sprite social-icon-douban"></i><span>分享到豆瓣</span></a></li>
          </ul>
        '>更多分享</a>
      </div>
    </div>
    <div id="vue_comment"></div>
  </div>

  <div class="vue-side-tool"></div>
</div>
<div class="js-included-collections"></div>

    <script type="application/json" data-name="page-data">{"user_signed_in":false,"locale":"zh-CN","os":"windows","read_mode":"day","read_font":"font2","note_show":{"is_author":false,"is_following_author":false,"is_liked_note":false,"uuid":"a5aa9c1e-46a4-4dde-b37b-e5d93d28ecd1"},"note":{"id":3958460,"slug":"7a7db9f8692d","user_id":1685558,"notebook_id":3450453,"commentable":true,"likes_count":183,"views_count":7267,"public_wordage":1456,"comments_count":56,"author":{"total_wordage":129652,"followers_count":3881,"total_likes_count":4260}}}</script>
    
    <script src="//cdn2.jianshu.io/assets/babel-polyfill-b5a90e7297a723b82f9e.js"></script>
    <script src="//cdn2.jianshu.io/assets/web-base-b5a90e7297a723b82f9e.js"></script>
<script src="//cdn2.jianshu.io/assets/web-b5a90e7297a723b82f9e.js"></script>
    
    <script src="//cdn2.jianshu.io/assets/web/pages/notes/show/entry-b5a90e7297a723b82f9e.js"></script>
    <script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-35169517-1', 'auto');
  ga('send', 'pageview');
</script>

<script>
  var _hmt = _hmt || [];
  (function() {
    var hm = document.createElement("script");
    hm.src = "//hm.baidu.com/hm.js?0c0e9d9b1e7d617b3e6842e85b9fb068";
    var s = document.getElementsByTagName("script")[0];
    s.parentNode.insertBefore(hm, s);
  })();
</script>

<script>
  (function(){
      var bp = document.createElement('script');
      var curProtocol = window.location.protocol.split(':')[0];
      if (curProtocol === 'https') {
          bp.src = 'https://zz.bdstatic.com/linksubmit/push.js';
      }
      else {
          bp.src = 'http://push.zhanzhang.baidu.com/push.js';
      }
      var s = document.getElementsByTagName("script")[0];
      s.parentNode.insertBefore(bp, s);
  })();
</script>

  </body>
</html>
