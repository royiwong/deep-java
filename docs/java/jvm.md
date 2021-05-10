https://www.cnblogs.com/crazymakercircle/p/14365820.html        
https://mp.weixin.qq.com/s/oyxKUxdJRLOjdM8a6fCQYA  
https://zhuanlan.zhihu.com/p/25511795   
https://zhuanlan.zhihu.com/p/34426768   

## Java类的加载机制    
https://mp.weixin.qq.com/s?__biz=MzI4NDY5Mjc1Mg==&mid=2247483934&idx=1&sn
=41c46eceb2add54b7cde9eeb01412a90&chksm=ebf6da61dc81537721d36aadb5d20613b
0449762842f9128753e716ce5fefe2b659d8654c4e8&scene=21#wechat_redirect  

## 1、JVM基本概念   
### 1.1、JVM是什么  
JVM 的全称是 「Java Virtual Machine」，也就是我们耳熟能详的 Java 虚拟机。    
JVM具备着计算机的基本运算方式，它主要负责把 Java 程序生成的字节码文件，解释成具体系统平台上的机器指令，让其在各个平台运行。  
JVM是运行在操作系统上的，它与硬件没有直接的交互。  
当然，严格来说JVM也是虚拟机规范，有很多不同的实现，Sun/OracleJDK和OpenJDK中的默认Java虚拟机
是HotSpot虚拟机，是目前使用范围最广的Java虚拟机，一般讲到的JVM默认指的就是HotSpot虚拟机。 
### 1.2、Java程序运行过程  
我们都知道 Java 源文件，通过编译器，能够生产相应的.Class 文件，也就是字节码文件，而字节码文件又通过 Java 虚拟机中的解释
器，编译成特定机器上的机器码 。   
也就是如下：  
![image](/images/jvm/jvm-1.png)     
每一种平台的解释器是不同的，但是实现的虚拟机是相同的，这也就是 Java 为什么能够跨平台的原因了 ，当一个程序从开始运行，这时
虚拟机就开始实例化了，多个程序启动就会存在多个虚拟机实例。程序退出或者关闭，则虚拟机实例消亡，多个虚拟机实例之间数据不能共享。 
### 1.3、JDK、JRE、JVM 
JDK(Java Development Kit Java 开发工具包)，JDK 是提供给 Java 开发人员使用的，其中包含了 Java 的开发工具，也包括了 JRE。其中的开发工具包括编译工具(javac.exe) 打包工具(jar.exe)等。

JRE(Java Runtime Environment Java 运行环境) 是 JDK 的子集，也就是包括 JRE 所有内容，以及开发应用程序所需的编译器和调试器等工具。JRE 提供了库、Java 虚拟机（JVM）和其他组件，用于运行 Java 编程语言、小程序、应用程序。

JVM(Java Virtual Machine Java 虚拟机)，JVM 可以理解为是一个虚拟出来的计算机，具备着计算机的基本运算方式，它主要负责把 Java 程序生成的字节码文件，

解释成具体系统平台上的机器指令，让其在各个平台运行。

JDK中包含JRE，也包括JDK，而JRE也包括JDK。

范围关系：JDK>JRE>JVM。