## Union-find  
严格地说，并查集是一种数据结构，它专门用来处理集合的合并操作和查询操作。并查集巧妙地借用了树结构，使得编程复杂度降低到了令人难以置信的地步；用上 一些递归技巧后，各种操作几乎都能用两行代码搞定。而路径压缩的好主意，更是整个数据结构的画龙点睛之笔。并查集的效率极高，单次操作的时间复杂度几乎可 以看作是常数级别；但由于数据结构的实际行为难以预测，精确的时间复杂度分析需要用到不少高深的技巧。  
## Knuth-Morris-Pratt字符串匹配算法  
关于此算法的介绍，请参考此文：[教你从头到尾彻底理解KMP算法](http://mobile.51cto.com/news-455986.htm)。KMP算法曾经落选于二十世纪最伟大的十大算法，但人们显然不能接受，如此漂亮、高效的KMP算法竟然会落选。所以，此次最终投票产出生，KMP算法排到了第二名。  
## BFPRT 算法    
1973 年，Blum、Floyd、Pratt、Rivest、Tarjan集体出动，合写了一篇题为 “Time bounds for selection” 的论文，给出了一种在数组中选出第 k 大元素的算法，俗称"中位数之中位数算法"。依靠一种精心设计的 pivot 选取方法，该算法从理论上保证了最坏情形下的线性时间复杂度，打败了平均线性、最坏 O(n^2) 复杂度的传统算法。一群大牛把递归算法的复杂度分析玩弄于骨掌股掌之间，构造出了一个当之无愧的来自圣经的算法。  
我在这里简单介绍下在数组中选出第k大元素的时间复杂度为O（N）的算法：  
类似快排中的分割算法：    
每次分割后都能返回枢纽点在数组中的位置s,然后比较s与k的大小  
若大的话，则再次递归划分array，小的话，就递归array //s为中间枢纽点元素。否则返回array，就是partition中返回的值。 //就是要找到这个s。找到符合要求的s值后，再遍历输出比s小的那一边的元素。  
我找到了这个 寻找数组中第k小的元素的，平均时间复杂度为O（N）的证明：上述程序的期望运行时间，证明可得O(n)，且假定元素是不同的。  

## Quicksort（快速排序）
快速排序算法几乎涵盖了所有经典算法的所有榜单。它曾获选二十世纪最伟大的十大算法。
## 第五名：Floyd-Warshall all-pairs最短路径算法
关于此算法的介绍，可参考我写的此文：几个最短路径算法比较  （http://blog.csdn.net/v_JULY_v/archive/2011/02/12/6181485.aspx）。  
d: 二维数组. d最小花费、或最短路径的邻边。  
for k from 1 to n:  
for i from 1 to n:   
for j from 1 to n:   
d = min(d, d + d)   
## Gentry's Fully Homomorphic Encryption Scheme（绅士完全同态加密机制）算法 
此算法很漂亮，它允许第三方执行任意加密数据运算得不到私钥（不是很了解）。
## Depth First Search、Breadth First Search（深度、广度优先搜索  
它们是许多其他算法的基础。  
## Miller-Rabin作的类似的试验测试  
这个想法是利用素数的性质(如使用费马大定理)的小概率寻找见证不数素数。如果没有证据是足够的随机检验后发现,这一数字为素数。  
## Binary Search （二分查找）
在一个有序的集合中查找元素，可以使用二分查找算法，也叫二分搜索。二分查找算法先比较位于集合中间位置的元素与键的大小，有三种情况（假设集合是从小到大排列的）：  
1.键小于中间位置的元素，则匹配元素必在左边（如果有的话），于是对左边的区域应用二分搜索。   
2.键等于中间位置的元素，所以元素找到。  
3.键大于中间位置的元素，则匹配元素必在右边（如果有的话），于是对右边的区域应用二分搜索。  
另外，当集合为空，则代表找不到。  
## Huffman coding（霍夫曼编码）  
霍夫曼编码(Huffman Coding)是一种编码方式，是一种用于无损数据压缩的熵编码（权编码）算法。1952年，David A. Huffman在麻省理工攻读博士时所发明的，并发表于《一种构建极小多余编码的方法》（A Method for the Construction of Minimum-Redundancy Codes）一文。  
##  Cooley-Tukey FFT算法。快速傅里叶变换算法  
##  linear programming，线性规划 
##  Dijkstra 算法  
与上第五一样，又一种最短路径算法。  
## Merge Sort
归并排序。  
## Ford–Fulkerson算法

网络***流算法。

##  辗转相除法
在数学中，辗转相除法，又称欧几里得算法，是求***公约数的算法，即求两个正整数之***公因子的算法。此算法作为TAOCP***个算法被阐述，足见此算 法被重视的程度。它是已知最古老的算法, 其可追溯至3000年前。辗转相除法***出现于欧几里得的《几何原本》（第VII卷，命题i和ii）中，而在中国则可以追溯至东汉出现的《九章算术》。扩 展的辗转相除法则构造性地证明了，对任意整数a和b ，存在一对x、y使得 ax + by = gcd(a, b) 。  

## RSA加密演算法
一种加密算法，日后再做详细介绍。
##  遗传算法
##  期望（EM）算法
此算法入选数据挖掘领域十大经典算法。在统计计算中，***期望（EM）算法是在概率（probabilistic）模型中寻找参数***似然估计的算法，其 中概率模型依赖于无法观测的隐藏变量（Latent Variable）。***期望经常用在机器学习和计算机视觉的数据聚类（Data Clustering）领域。***期望算法经过两个步骤交替进行计算，***步是计算期望（E），利用对隐藏变量的现有估计值，计算其***似然估计值；第二步是***化（M），***化在 E 步上求得的***似然值来计算参数的值。M 步上找到的参数估计值被用于下一个 E 步计算中，这个过程不断交替进行。  
## 数据压缩
数据压缩是通过减少计算机中所存储数据或者通信传播中数据的冗余度，达到增大数据密度，最终使数据的存储空间减少的技术。数据压缩在文件存储和分布式系统领域有着十分广泛的应用。数据压缩也代表着尺寸媒介容量的增大和网络带宽的扩展。   
## Hash函数
Hash，一般翻译做“散列”，也有直接音译为“哈希”的，就是把任意长度的输入（又叫做预映射， pre-image），通过散列算法，变换成固定长度的输出，该输出就是散列值。  
## Dynamic Programming（动态规划）
## 堆排序算法
堆排序算法作为一种快速稳定的算法，其平均时间复杂度（最坏也为）O（n*lgn）。当然，在实际应用中，一个实现的好的快速排序算法仍然要优于堆排序算法。不过，堆数据结构还可以作为高效的优先级队列。  
## 递归与回溯算法  
此俩个算法，相信各位比较熟悉，在此不做赘述。 
##  最长公共子序列  
最长公共子序列，英文缩写为LCS（Longest Common Subsequence）。其定义是，一个数列 S ，如果分别是两个或多个已知数列的子序列，且是所有符合此条件序列中最长的，则 S 称为已知序列的最长公共子序列。  
动态规划的一个计算最长公共子序列的方法如下：  
以两个序列 X、Y 为例子：  
设有二维数组 f 表示 X 的 i 位和 Y 的 j 位之前的最长公共子序列的长度，则有：  
   f = same(1,1)  
   f = max{f+same(i,j)，f，f}  
其中，same(a,b)当 X 的第 a 位与 Y 的第 b 位完全相同时为“1”，否则为“0”。  
此时，f中***的数便是 X 和 Y 的最长公共子序列的长度，依据该数组回溯，便可找出最长公共子序列。  
该算法的空间、时间复杂度均为O(n2)，经过优化后，空间复杂度可为O(n)，时间复杂度为O(nlogn)。  
##  红黑树的算法与实现
关于红黑树，linux内核中有实现。
## A\*搜寻算法
相对于BFS、Dijkstra 等算法，A*搜寻算法作为一种高效的最短路径搜索算法，如今，已得到日益广泛的应用。
##  图像特征提取与匹配之SIFT算法
sift，尺度不变特征转换，是一种电脑视觉的算法用来侦测与描述影像中的局部性特征，它在空间尺度中寻找极值点，并提取出其位置、尺度、旋转不变量，此算法由 David Lowe 在1999年所发表，2004年完善总结。