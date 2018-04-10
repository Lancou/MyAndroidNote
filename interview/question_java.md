Java面试题大纲为以下内容（绝大部分）： 
- Java各方面基础 
- Java特性 
- 多线程，并发及线程基础 
- 数据类型转换的基本原则 
- 垃圾回收（GC） 
- Java 集合框架 
- 数组 
- 字符串 
- 设计模式 
- SOLID （单一功能、开闭原则、里氏替换、接口隔离以及依赖反转）设计原则 
- 抽象类与接口 
- 泛型与枚举 
- Java IO 与 NIO 
- 常用网络协议 
- Java 中的数据结构和算法 
- 正则表达式 
- JVM 
- Java 最佳实践 
- JDBC 
- Date, Time 与 Calendar 
- Java 处理 XML 
- JUnit

挺多的，但是根据BAT等大厂的面试规律，有很多东西是不会问到的，问到的都是跟Android息息相关的，so我整理了一下范围，如下。

2017-2018 Android-BAT-Java 面试题分类： 
- 1.Java特性 
- 2.字符串String、数组、数据类型转换 
- 3.Java各方面基础 
- 4.抽象类与接口 
- 5.JVM、垃圾回收（GC） 
- 6.Java数据结构和算法 
- 7.设计模式 
- 8.泛型与枚举 
- 9.常用网络协议 
- 10.Java IO 与 NIO 
- 11.多线程，并发及线程基础

1.Java特性 
（1.1）对java多态的理解 
https://www.jianshu.com/p/8cfb92ecaabe 
http://www.cnblogs.com/hupp/p/4854918.html 
此处延伸《动态绑定》： 
http://hxraid.iteye.com/blog/428891 
（1.2）Java中实现多态的机制是什么？ 
https://www.jianshu.com/p/8cfb92ecaabe 
http://www.cnblogs.com/hupp/p/4854918.html

2.字符串String、数组、数据类型转换 
（2.1）Java中String的了解 
https://www.jianshu.com/p/2f209af80f84 
（2.2）String，Stringbuffer，Stringbuilder三者的区别 
http://blog.csdn.net/kingzone_2008/article/details/9220691 
（2.3）String为什么要设计成不可变的？ 
https://www.jianshu.com/p/16480390a847 
https://www.jianshu.com/p/48b011688edc 
（2.4）string 转换成 integer的方式及原理 
http://blog.csdn.net/sinat_20259781/article/details/52024763 
（2.5）int、char、long各占多少字节数 
http://blog.csdn.net/never_cxb/article/details/47204485 
（2.6）int与integer的区别 
https://www.cnblogs.com/liuling/archive/2013/05/05/intAndInteger.html 
https://www.jianshu.com/p/08010144d40f

3.Java各方面基础 
（3.1）java中==和equals和hashCode的区别 
http://blog.csdn.net/hla199106/article/details/46907725 
（3.2）Object类的equal和hashCode方法重写，为什么？ 
https://www.jianshu.com/p/f9cc84047bd6 
（3.3）修改对象A的equals方法的签名，那么使用HashMap存放这个对象实例的时候，会调用哪个equals方法？ 
https://www.jianshu.com/p/7d3feb156be4 
（3.4）线程sleep和wait有什么区别 
http://blog.csdn.net/liuzhenwen/article/details/4202967 
（3.5）闭包和局部内部类的区别 
https://www.jianshu.com/p/f55b11a4cec2 
https://www.jianshu.com/p/367b138fe909 
（3.6）进程和线程的区别 
https://www.jianshu.com/p/a4fa4edbeb8a 
（3.7）序列化的方式 
https://www.jianshu.com/p/ff770511a097 
（3.8）Serializable 和Parcelable 的区别 
https://www.jianshu.com/p/a60b609ec7e7 
（3.9）静态属性和静态方法是否可以被继承？是否可以被重写？以及原因？ 
http://blog.csdn.net/liuconey/article/details/51555362 
http://blog.csdn.net/carmelo_z/article/details/67086140 
（3.10）静态内部类的设计意图 
http://blog.csdn.net/blessed24/article/details/78077134 
https://www.cnblogs.com/aademeng/articles/6192954.html 
（3.11）成员内部类、静态内部类、局部内部类和匿名内部类的理解，以及项目中的应用 
https://www.jianshu.com/p/5c5fa1377c79 
https://www.jianshu.com/p/e385ce41ca5b 
（3.12）什么是内部类？内部类的作用 
https://www.jianshu.com/p/e385ce41ca5b 
（3.13）讲一下常见编码方式？ 
https://www.cnblogs.com/liujinhong/p/5995946.html 
（3.14）utf-8编码中的中文占几个字节；int型几个字节？ 
https://www.jianshu.com/p/c34d3e5790a4 
（3.15）Java的异常体系 
https://www.jianshu.com/p/93aa1cf26b97 
（3.16）如何将一个Java对象序列化到文件里？ 
http://blog.csdn.net/it_wangxiangpan/article/details/5781941 
（3.17）final，finally，finalize的区别 
https://www.jianshu.com/p/59b77edd3319 
（3.18）说说你对Java反射的理解 
https://www.jianshu.com/p/6277c1f9f48d 
https://www.jianshu.com/p/1a21a9cb5bea 
（3.19）说说你对Java注解的理解 
https://www.jianshu.com/p/0b1af95c1335 
https://www.jianshu.com/p/4068da3c8d3d 
（3.20）说说你对依赖注入的理解 
https://www.jianshu.com/p/506dcd94d4f9 
（3.21）静态代理和动态代理的区别，什么场景使用？ 
https://www.jianshu.com/p/2f518a4a4c2b 
https://www.jianshu.com/p/861223789d53

4.抽象类与接口 
（4.1）抽象类和接口区别 
https://www.jianshu.com/p/038f0b356e9a 
https://www.jianshu.com/p/612e2d2a8a78 
（4.2）抽象类的意义 
http://blog.csdn.net/wei_zhi/article/details/52736350 
（4.3）抽象类与接口的应用场景 
http://blog.csdn.net/xcbeyond/article/details/7667733 
（4.4）抽象类是否可以没有方法和属性？ 
当然可以。。 
（4.5）接口的意义 
http://blog.csdn.net/oreo_go/article/details/52102514 
PS：（4.1）-（4.4）都是一类东西，基本上过一遍详细的文章，都能解决。 
（4.6）父类的静态方法能否被子类重写 
https://www.jianshu.com/p/df43f5500ea3

5.JVM、垃圾回收（GC） 
（5.1）java虚拟机的工作原理 
https://www.cnblogs.com/lishun1005/p/6019678.html 
（5.2）java虚拟机和Dalvik虚拟机的区别 
http://www.jianshu.com/p/923aebd31b65 
（5.3）哪些情况下的对象会被垃圾回收机制处理掉？ 
https://www.jianshu.com/p/5261a62e4d29 
https://www.jianshu.com/p/778dd3848196 
（5.4）谈谈你对解析与分派的认识。 
这个已经有点深入了，建议从虚拟机入手，先了解清楚。 
https://www.jianshu.com/p/355ae3bcec41

6.Java数据结构和算法 
算法在这里就没必要收集面试题了，这个不是一下子能掌握的东西，需要题目的自己百度去背简单的几个算法。 
掌握算法需要一个过程，我建议可以去leetcode、lintcode等刷提网站练习。 
（6.1）常用数据结构简介 
https://www.jianshu.com/p/44a1e5bc077a 
（6.2）并发集合了解哪些？ 
http://youyu4.iteye.com/blog/2352846 
（6.3）列举java的集合以及集合之间的继承关系 
https://www.jianshu.com/p/63e76826e852 
（6.4）集合类以及集合框架 
https://www.jianshu.com/p/63e76826e852 
（6.5）容器类介绍以及之间的区别（容器类估计很多人没听这个词，Java容器主要可以划分为4个部分：List列表、Set集合、Map映射、工具类（Iterator迭代器、Enumeration枚举类、Arrays和Collections） 
https://www.jianshu.com/p/c70989bd5f29 
（6.6）List,Set,Map的区别 
https://www.jianshu.com/p/047e33fdefd2 
（6.7）List和Map的实现方式以及存储方式 
https://www.jianshu.com/p/047e33fdefd2 
（6.8）HashMap的实现原理 
https://www.jianshu.com/p/8b372f3a195d/ 
（6.9）HashMap数据结构？ 
https://www.jianshu.com/p/8b372f3a195d/ 
（6.10）HashMap源码理解 
https://www.jianshu.com/p/8b372f3a195d/ 
（6.11）HashMap如何put数据（从HashMap源码角度讲解）？ 
https://www.jianshu.com/p/8b372f3a195d/ 
（6.12）HashMap怎么手写实现？ 
自己去写哈，几种遍历方式。 
（6.13）ConcurrentHashMap的实现原理 
https://www.jianshu.com/p/c0642afe03e0 
（6.14）ArrayMap和HashMap的对比 
https://www.jianshu.com/p/7b9a1b386265 
（6.15）HashTable实现原理 
https://www.jianshu.com/p/dbe7a1ea5928 
（6.16）TreeMap具体实现 
https://www.jianshu.com/p/d9ad7f6d75a0 
（6.17）HashMap和HashTable的区别 
https://www.jianshu.com/p/7456a339e4aa 
（6.18）HashMap与HashSet的区别 
https://www.jianshu.com/p/749e6ce12d98 
（6.19）HashSet与HashMap怎么判断集合元素重复？ 
http://f543711700.iteye.com/blog/800929 
http://blog.csdn.net/ning109314/article/details/17354839 
（6.20）集合Set实现Hash怎么防止碰撞 
http://blog.csdn.net/zeb_perfect/article/details/52574915 
http://blog.csdn.net/u010698072/article/details/52802179 
（6.21）ArrayList和LinkedList的区别，以及应用场景 
https://www.cnblogs.com/soundcode/p/6294174.html 
https://www.jianshu.com/p/e591690afacb 
（6.22）数组和链表的区别 
https://www.jianshu.com/p/26fa29a3d669 
（6.23）二叉树的深度优先遍历和广度优先遍历的具体实现 
http://blog.csdn.net/fantasy_lin_/article/details/52751559 
（6.24）堆的结构 
http://blog.csdn.net/l294265421/article/details/50927538 
（6.25）堆和树的区别 
https://www.zhihu.com/question/36134980/answer/66080662 
（6.26）堆和栈在内存中的区别是什么(解答提示：可以从数据结构方面以及实际实现方面两个方面去回答)？ 
https://www.jianshu.com/p/947a76e2ddbc 
（6.27）什么是深拷贝和浅拷贝 
http://blog.csdn.net/u014727260/article/details/55003402 
（6.28）手写链表逆序代码 
http://blog.csdn.net/u012571415/article/details/46955535 
（6.29）讲一下对树，B+树的理解 
https://www.jianshu.com/p/6f68d3c118d6 
（6.30）判断单链表成环与否？ 
http://blog.csdn.net/njr465167967/article/details/52634352 
算法题，去leetcode、lintcode多刷刷题，这些都不是什么问题 
（6.31）链表翻转（即：翻转一个单项链表） 
http://blog.csdn.net/guyuealian/article/details/51119499 
算法题，去leetcode、lintcode多刷刷题，这些都不是什么问题 
（6.32）合并多个单有序链表（假设都是递增的） 
https://www.jianshu.com/p/a3d5cd6c3ae2

7.设计模式 
（7.1）在Java中，什么时候用重载，什么时候用重写？ 
http://blog.csdn.net/qq_33642117/article/details/51920354 
（7.2）Java中什么是单例设计模式？用Java写出线程安全的单例 
https://www.cnblogs.com/garryfu/p/7976546.html 
http://blog.csdn.net/cselmu9/article/details/51366946 
（7.3）使用工厂模式最主要的好处是什么？你在哪里使用？ 
http://blog.csdn.net/lee576/article/details/1549910

8.泛型与枚举 
（8.1）说一下泛型原理，并举例说明 
https://www.jianshu.com/p/ddbe1db509da 
（8.2）泛型中extends和super的区别 
https://www.zhihu.com/question/20400700 
（8.3）什么是泛型中的限定通配符和非限定通配符 
https://www.jianshu.com/p/ccdfc9bba821 
https://www.cnblogs.com/fengmingyue/p/6087031.html

9.常用网络协议 
（9.1）HTTP响应的结构是怎么样的？ 
http://liuwangshu.cn/application/network/1-http.html 
（9.2）什么是cookie？session和cookie有什么区别 
http://blog.csdn.net/duan1078774504/article/details/51912868 
（9.3）TCP/IP在连接时有几次握手？释放时有几次握手？ 
http://blog.csdn.net/guyuealian/article/details/52535294 
（9.4）什么是TCP协议？UDP协议？区别？ 
http://blog.csdn.net/qq_18425655/article/details/51955674

10.Java IO 与 NIO 
（10.1）说说io和nio的理解，区别？ 
这个作者写了12篇NIO的文章： 
http://www.importnew.com/18763.html

11.多线程，并发及线程基础 
关于多线程请先过一遍这篇文章： 
https://www.jianshu.com/p/40d4c7aebd66 
（11.1）开启线程的三种方式？ 
http://blog.csdn.net/longshengguoji/article/details/41126119 
（11.2）谈谈你对多线程同步机制的理解？ 
一般问你怎么理解，就是说要怎么用，用在什么场景。 
https://www.jianshu.com/p/592ef5642513 
（11.3）为什么要有线程，而不是仅仅用进程？ 
http://blog.csdn.net/tongxinhaonan/article/details/42558561 
（11.4）run()和start()方法区别 
http://blog.csdn.net/dada360778512/article/details/6965790 
（11.5）如何控制某个方法允许并发访问线程的个数？ 
http://blog.csdn.net/zuoanyinxiang/article/details/50448564 
http://blog.csdn.net/anhenzhufeng/article/details/70225415 
（11.6）在Java中wait和seelp方法的不同 
https://www.jianshu.com/p/a67ad7ba89a5 
（11.7）谈谈wait/notify关键字的理解 
https://www.jianshu.com/p/f3d472c21c0e 
（11.8）什么导致线程阻塞？ 
http://blog.csdn.net/sinat_22013331/article/details/45740641 
http://blog.csdn.net/he3527/article/details/77618691 
（11.9）线程如何关闭？ 
https://www.jianshu.com/p/536b0df1fd55 
（11.10）讲一下java中的同步的方法 
https://www.jianshu.com/p/6542c8a96392 
（11.11）数据一致性如何保证？ 
https://www.cnblogs.com/jiumao/p/7136631.html 
从数据库下手去了解，道理差不多。重点是同步和线程安全。 
（11.12）如何保证线程安全？ 
https://www.jianshu.com/p/fe7ed5b50933 
http://blog.csdn.net/xiangxianghehe/article/details/51135299 
（11.13）如何实现线程同步？ 
https://www.jianshu.com/p/6542c8a96392 
（11.14）谈谈对多线程的理解 
https://www.jianshu.com/p/40d4c7aebd66 
（11.15）线程间操作List 
不知道想问啥，并发操作？ 
（11.16）Java中对象的生命周期 
http://blog.csdn.net/sodino/article/details/38387049 
延伸：如何判断对象“无用” 
https://www.jianshu.com/p/73d8d6c54515 
（11.17）Synchronized用法 
https://www.jianshu.com/p/19f861ab749e 
（11.18）Synchronize的原理 
https://www.jianshu.com/p/19f861ab749e 
（11.19）谈谈对Synchronized关键字，类锁，方法锁，重入锁的理解 
http://blog.csdn.net/le_le_name/article/details/52348314 
https://www.jianshu.com/p/007bd7029faf 
（11.20）static synchronized 方法的多线程访问和作用 
http://blog.csdn.net/wangtaomtk/article/details/52318634 
（11.21）同一个类里面两个synchronized方法，两个线程同时访问的问题 
http://blog.csdn.net/aiyawalie/article/details/53261823 
（11.22）谈谈volatile关键字的用法 
https://www.jianshu.com/p/7798161d7472 
（11.23）谈谈volatile关键字的作用 
https://www.jianshu.com/p/7798161d7472 
（11.24）volatile的原理 
https://www.jianshu.com/p/7c614ac4dd92 
http://ifeve.com/volatile/ 
（11.26）Synchronized 和volatile 关键字的区别 
http://blog.csdn.net/suifeng3051/article/details/52611233 
https://www.cnblogs.com/tf-Y/p/5266710.html 
（11.27）Synchronized与Lock的区别 
http://blog.csdn.net/u012403290/article/details/64910926?locationNum=11&fps=1 
https://www.jianshu.com/p/2344a3e68ca9 
（11.28）ReentrantLock 、synchronized和volatile比较 
http://heaven-arch.iteye.com/blog/1738212 
https://www.cnblogs.com/dennyzhangdd/p/6020566.html 
（11.29）ReentrantLock的内部实现 
http://blog.csdn.net/yanyan19880509/article/details/52345422 
（11.30）lock原理 
http://blog.csdn.net/endlu/article/details/51249156 
（11.31）死锁的四个必要条件？ 
http://blog.csdn.net/ysdaniel/article/details/6644418 
（11.32）怎么避免死锁？ 
http://blog.csdn.net/ls5718/article/details/51896159 
（11.33）对象锁和类锁是否会互相影响？ 
http://blog.csdn.net/u013142781/article/details/51697672 
http://blog.csdn.net/codeharvest/article/details/70649375 
先了解它们是啥，自己动手试一下就知道了。 
（11.34）什么是线程池，如何使用? 
https://www.jianshu.com/p/210eab345423 
（11.35）Java的并发、多线程、线程模型 
并发模型：https://www.jianshu.com/p/067702fbf256 
http://ifeve.com/%E5%B9%B6%E5%8F%91%E7%BC%96%E7%A8%8B%E6%A8%A1%E5%9E%8B/ 
线程模型： 
https://www.cnblogs.com/tian830937/p/5277459.html 
（11.36）多线程有什么要注意的问题？ 
并发问题，安全问题，效率问题。 
（11.37）谈谈你对并发编程的理解并举例说明 
https://www.jianshu.com/p/053943a425c3 
http://blog.csdn.net/songxinjianqwe/article/details/72789899?locationNum=15&fps=1 
有本书叫：java并发编程实战，买下来。 
（11.38）如何保证多线程读写文件的安全？ 
换个说法就是你怎么保证多线程安全，怎么样保证多线程安全做一件事，这件事是啥不重要。。 
关于写文件这里有篇文章： 
http://blog.csdn.net/baple/article/details/23857485 
（11.39）多线程断点续传原理 
http://blog.csdn.net/ghost_Programmer/article/details/51923895 
（11.40）断点续传的实现 
http://blog.csdn.net/ghost_Programmer/article/details/51923895 
关于断点续传这个，我自己以前有做过，我建议可以从android的开源框架里面直接看源码，这样懂的比较快。断点续传的框架有很多。
