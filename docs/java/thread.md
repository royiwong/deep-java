##  JUC包简介
---
J.U.C并发包，即java.util.concurrent包，是JDK的核心工具包，是JDK1.5之后，由 Doug Lea实现并引入。  
整个java.util.concurrent包，按照功能可以大致划分如下：  
- juc-locks 锁框架 
- juc-atomic 原子类框架
- juc-sync 同步器框架
- juc-collections 集合框架
- juc-executors 执行器框架    
本系列将按上述顺序分析J.U.C，分析所基于的源码为Oracle JDK1.8.0_111。
主要参考书籍：  
《Java Concurrency in Practice》 Brian Goetz等  
《JAVA多线程设计模式》 结城浩  
##  juc-locks 锁框架
