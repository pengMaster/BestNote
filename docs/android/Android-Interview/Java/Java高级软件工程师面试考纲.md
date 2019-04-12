如果要应聘高级开发工程师职务，仅仅懂得Java的基础知识是远远不够的，还必须懂得常用数据结构、算法、网络、操作系统等知识。因此本文不会讲解具体的技术，笔者综合自己应聘各大公司的经历，整理了一份大公司对Java高级开发工程师职位的考核纲要，希望可以帮助到需要的人。

当前，市面上有《Java XX宝典》类似的图书，而且图书中的内容都着重在讲解Java最为基础的部分，最严重的是，里面有着大量错误的内容，极具误导性。另外，网上也有各种各样的[Java面试题](http://www.codeceo.com/article/tag/java%E9%9D%A2%E8%AF%95%E9%A2%98)，很多也是着重在Java语言基础上。实际上，如果要应聘高级开发工程师职务，仅仅懂得Java的基础知识是远远不够的，还必须懂得常用数据结构、算法、网络、操作系统等知识。因此本文不会讲解具体的技术，笔者综合自己应聘各大公司的经历，整理了一份大公司对Java高级开发工程师职位的考核纲要，希望可以帮助到需要的人。

## 1 Java基础

**1.1 Collection和Map**

(1)掌握Collection和Map的继承体系。

(2)掌握ArrayList、LinkedList、Vector、Stack、PriorityQueue、HashSet、LinkedHashSet、TreeSet、HashMap、LinkedHashMap、TreeMap、[WeakHashMap](http://www.codeceo.com/article/java-weakhashmap-source.html)、EnumMap、TreeMap、HashTable的特点和实现原理。

(3)掌握CopyOnWriteArrayList、CopyOnWriteArraySet、ConcurrentHashMap的实现原理和适用场景。

**1.2 IO**

(1)掌握InputStream、OutputStream、Reader、Writer的继承体系。

(2)掌握字节流(FileInputStream、DataInputStream、BufferedInputStream、FileOutputSteam、DataOutputStream、BufferedOutputStream)和字符流(BufferedReader、InputStreamReader、FileReader、BufferedWriter、OutputStreamWriter、PrintWriter、FileWriter)，并熟练运用。

(3)掌握NIO实现原理及使用方法。

**1.3 异常**

(1)掌握Throwable继承体系。

(2)掌握异常工作原理。

(3)了解常见受检异常(比如FileNotFoundException)、非受检异常(比如NullPointerException)和错误(比如IOError)。

**1.4 多线程**

(1)掌握[Executor](http://www.codeceo.com/article/java-executor-learning.html)s可以创建的三种(JAVA8增加了一种，共四种)线程池的特点及适用范围。

(2)掌握多线程同步机制，并熟练运用。

**1.5 Socket**

(1)掌握Socket通信原理。

(2)熟练使用多线程结合Socket进行编程。

## 2 Java虚拟机

**2.1 JVM内存区域划分**

(1)掌握程序计数器、堆、虚拟机栈、本地方法栈、方法区（JAVA8已移除）、元空间（JAVA8新增）的作用及基本原理。

(2)掌握堆的划分：新生代（Eden、Survivor1、Survivor2）和老年代的作用及工作原理。

(3)掌握JVM内存参数设置及调优。

**2.2 类加载**

(1)掌握类的加载阶段：加载、链接（验证、准备、解析）、初始化、使用、卸载。

(2)掌握类加载器分类及其应用：启动类加载器、扩展类加载器、应用程序类加载器、自定义加载器。

## 3 J2EE

(1) 掌握JSP内置对象、动作及相关特点和工作原理。

(2) 掌握Servlet的特点和工作原理。

(3) 掌握Spring框架的IOC和AOP实现原理（反射和动态代理）。

(4) 至少掌握一个[MVC框架](http://www.codeceo.com/article/mvc-framework-mvc-design.html)（Spring MVC，Struts等）的工作原理，并熟练运用。

(5) 至少掌握一个ORM框架(Hibernate，MyBatis等)的工作原理，并熟练运用。

## 4 数据结构与算法

(1)掌握线性表和树的特点并熟练运用。

(2)掌握常用排序和查找算法：插入排序(直接插入排序、希尔排序)、选择排序(直接选择排序、堆排序)、交换排序(冒泡排序、快速排序)、归并排序，顺序查找、[二分查找](http://www.codeceo.com/article/binary-search.html)、哈希查找。

(3) 熟练运用常见排序和查找算法思想解决编程问题。

(4)了解几大基本算法：[贪心算法](http://www.codeceo.com/article/greedy-algorithm.html)、分治策略、动态规划。

## 5 计算机网络

(1)掌握网络的分层结构，及每层的功能特点。

(2)掌握TCP/IP的通信原理(三次握手、四次挥手)

## 6 数据库

(1)掌握复杂的SQL语句编写。

(2)掌握数据库的优化（SQL层面和表设计层面）。

(3)至少掌握一款数据库产品。

(4)熟悉高并发、大数据情况下的数据库开发。

## 7 Web技术

(1)掌握AJAX的工作原理。

(2)至少熟悉一款JS框架(比如JQuery)。

## 8 [设计模式](http://www.codeceo.com/article/category/develop/design-patterns)

(1)熟悉常见的设计模式。

(2)会将设计模式理论应用到实际开发中。

## 9 Linux

(1)熟练运用Linux常见命令。

(2)熟悉Linux操作系统基本概念及特点。

(3)熟悉Shell脚本。

## 10 操作系统

(1)掌握操作系统的进程管理。

(2)了解操作系统的I/O。

## 11 正则表达式

(1)掌握常见正则表达式符号。

(2)熟练运用正则表达式解决实际问题(比如匹配电话号码、邮箱、域名等)。