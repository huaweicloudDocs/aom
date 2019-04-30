# JVM监控<a name="ZH-CN_TOPIC_0148190949"></a>

JVM监控展示基于Java应用的JVM运行环境的内存和线程指标，您可以实时监控指标趋势进行性能分析。

JVM监控功能提供JVM内存和线程指标，您可以单击“内存”和“线程”两个页签，查看内存和线程指标图，快速分析定位内存泄漏、线程异常等问题。

## JVM监控界面说明<a name="section18389174916160"></a>

**图 1**  JVM监控界面<a name="fig332813493411"></a>  
![](figures/JVM监控界面.png "JVM监控界面")

## 内存指标图表<a name="section196041212151912"></a>

如[图2](#fig13224121372113)所示，展示设置的时间段内某个实例的总内存、堆内存、非堆内存等JVM不同内存区域的最大值、分配值和使用情况的趋势，也展示设置的时间段内某个实例的垃圾收集堆的GC时间和GC次数趋势。

**图 2**  内存指标图<a name="fig13224121372113"></a>  
![](figures/内存指标图.png "内存指标图")

**JVM内存介绍**

JVM区域总体分为Heap memory和Non-Heap memory。

-   Heap memory：堆是Java 虚拟机运行时数据区域，分配所有类实例和数组的内存。对象的堆内存由称为垃圾回收器的自动内存管理系统回收。Heap区分为Eden Space、Survivor Space和Tenured Space。
-   Non-Heap memory：Java 虚拟机管理堆之外的内存。Non-Heap区分为Code Cache、Permanent Space或Meta Space。

Java堆是垃圾收集器管理的主要区域，又称为Garbage Collectioned Heap，GC方式包括Full GC和Minor GC。

**表 1**  内存区域说明

<a name="table143811759732"></a>
<table><thead align="left"><tr id="row1038455912310"><th class="cellrowborder" valign="top" width="15.9%" id="mcps1.2.3.1.1"><p id="p153840591632"><a name="p153840591632"></a><a name="p153840591632"></a>区域名称</p>
</th>
<th class="cellrowborder" valign="top" width="84.1%" id="mcps1.2.3.1.2"><p id="p14385165910312"><a name="p14385165910312"></a><a name="p14385165910312"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row138715599316"><td class="cellrowborder" valign="top" width="15.9%" headers="mcps1.2.3.1.1 "><p id="p5389105910310"><a name="p5389105910310"></a><a name="p5389105910310"></a>Eden Space</p>
</td>
<td class="cellrowborder" valign="top" width="84.1%" headers="mcps1.2.3.1.2 "><p id="p1639025913316"><a name="p1639025913316"></a><a name="p1639025913316"></a>用于最初从<span>线程池</span>分配内存<span>给大部分对象</span>。</p>
</td>
</tr>
<tr id="row12391359938"><td class="cellrowborder" valign="top" width="15.9%" headers="mcps1.2.3.1.1 "><p id="p1839314594315"><a name="p1839314594315"></a><a name="p1839314594315"></a>Survivor Space</p>
</td>
<td class="cellrowborder" valign="top" width="84.1%" headers="mcps1.2.3.1.2 "><p id="p123949597316"><a name="p123949597316"></a><a name="p123949597316"></a><span>用于保存在Eden区内存池中经过垃圾回收后没有被回收的对象。</span></p>
</td>
</tr>
<tr id="row3394659339"><td class="cellrowborder" valign="top" width="15.9%" headers="mcps1.2.3.1.1 "><p id="p203951159439"><a name="p203951159439"></a><a name="p203951159439"></a>Tenured Space</p>
</td>
<td class="cellrowborder" valign="top" width="84.1%" headers="mcps1.2.3.1.2 "><p id="p1939615591235"><a name="p1939615591235"></a><a name="p1939615591235"></a><span>用于保持已经在Survivor区内存池中存在了一段时间的对象。</span></p>
</td>
</tr>
<tr id="row2039717591434"><td class="cellrowborder" valign="top" width="15.9%" headers="mcps1.2.3.1.1 "><p id="p439795914318"><a name="p439795914318"></a><a name="p439795914318"></a>Code Cache</p>
</td>
<td class="cellrowborder" valign="top" width="84.1%" headers="mcps1.2.3.1.2 "><p id="p1039714591317"><a name="p1039714591317"></a><a name="p1039714591317"></a><span>用于编译和保存本地代码的内存。</span></p>
</td>
</tr>
<tr id="row3398125912319"><td class="cellrowborder" valign="top" width="15.9%" headers="mcps1.2.3.1.1 "><p id="p04001759433"><a name="p04001759433"></a><a name="p04001759433"></a>Permanent Space</p>
</td>
<td class="cellrowborder" valign="top" width="84.1%" headers="mcps1.2.3.1.2 "><p id="p440112597310"><a name="p440112597310"></a><a name="p440112597310"></a><span>用于保存虚拟机的静态数据，例如，类和方法对象。</span></p>
</td>
</tr>
<tr id="row4401559638"><td class="cellrowborder" valign="top" width="15.9%" headers="mcps1.2.3.1.1 "><p id="p1940218590312"><a name="p1940218590312"></a><a name="p1940218590312"></a>Meta Space</p>
</td>
<td class="cellrowborder" valign="top" width="84.1%" headers="mcps1.2.3.1.2 "><p id="p1140315595310"><a name="p1140315595310"></a><a name="p1140315595310"></a>用于保存本地化内存中类的元数据。Java 8之后Meta Space替代Permanent Space。</p>
</td>
</tr>
<tr id="row104037591238"><td class="cellrowborder" valign="top" width="15.9%" headers="mcps1.2.3.1.1 "><p id="p1140311591237"><a name="p1140311591237"></a><a name="p1140311591237"></a>Full GC</p>
</td>
<td class="cellrowborder" valign="top" width="84.1%" headers="mcps1.2.3.1.2 "><p id="p5403959638"><a name="p5403959638"></a><a name="p5403959638"></a>当内存回收之后仍无法满足内存空间分配需求时， 对整个堆空间（新生代、老年代和永久代）进行垃圾收集。</p>
</td>
</tr>
<tr id="row540695919316"><td class="cellrowborder" valign="top" width="15.9%" headers="mcps1.2.3.1.1 "><p id="p1340711591931"><a name="p1340711591931"></a><a name="p1340711591931"></a>Minor GC</p>
</td>
<td class="cellrowborder" valign="top" width="84.1%" headers="mcps1.2.3.1.2 "><p id="p240713590312"><a name="p240713590312"></a><a name="p240713590312"></a>当分配对象遇到内存不足时，对新生代空间（Eden区和Survivor区）进行垃圾收集。</p>
</td>
</tr>
</tbody>
</table>

JVM采用分代垃圾回收。在JVM的内存空间中把堆空间分为老年代和新生代。将大量（90%以上）创建后短期消亡的对象存储在新生代，而老年代中存放生命周期长久的实例对象。新生代空间分为Eden区和两个Survivor区。新对象首先分配在Eden区，Survivor区作为Eden区和Tenured区的缓冲，在Survivor区的对象经历若干次收集仍然存活的，就会被转移到老年区，如[图3](#fig2089083272713)所示。

**图 3**  内存区域图解<a name="fig2089083272713"></a>  
![](figures/内存区域图解.png "内存区域图解")

>![](public_sys-resources/icon-note.gif) **说明：**   
>新生代共有两个Survivor区，分别用from和to指针指代，其中to指针指向空的Survivor区。  

## 线程指标图表<a name="section188401421102912"></a>

如[图4](#fig176231143319)所示，展示设置的时间段内某个实例的线程数、粘滞线程、专用线程等线程执行情况的趋势。

**图 4**  线程指标图<a name="fig176231143319"></a>  
![](figures/线程指标图.png "线程指标图")

**表 2**  线程说明

<a name="table464495205312"></a>
<table><thead align="left"><tr id="row1564575225319"><th class="cellrowborder" valign="top" width="19.33%" id="mcps1.2.3.1.1"><p id="p1564513524534"><a name="p1564513524534"></a><a name="p1564513524534"></a>线程名称</p>
</th>
<th class="cellrowborder" valign="top" width="80.67%" id="mcps1.2.3.1.2"><p id="p15645175235312"><a name="p15645175235312"></a><a name="p15645175235312"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row657961514468"><td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.3.1.1 "><p id="p175791153464"><a name="p175791153464"></a><a name="p175791153464"></a>总数</p>
</td>
<td class="cellrowborder" valign="top" width="80.67%" headers="mcps1.2.3.1.2 "><p id="p757617227454"><a name="p757617227454"></a><a name="p757617227454"></a>是指总线程数，包含活动线程数和备用线程数。粘滞线程和专用线程在执行完成后变为备用线程。</p>
</td>
</tr>
<tr id="row1257131811414"><td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.3.1.1 "><p id="p11576189415"><a name="p11576189415"></a><a name="p11576189415"></a>死锁</p>
</td>
<td class="cellrowborder" valign="top" width="80.67%" headers="mcps1.2.3.1.2 "><p id="p14571418104111"><a name="p14571418104111"></a><a name="p14571418104111"></a>是指两个或两个以上的进程在执行过程中，由于竞争资源或彼此通信而造成的阻塞现象，导致系统处于死锁状态，此类永远在互相等待的进程称为死锁进程。</p>
</td>
</tr>
<tr id="row16451052125313"><td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.3.1.1 "><p id="p664525216531"><a name="p664525216531"></a><a name="p664525216531"></a>粘滞线程</p>
</td>
<td class="cellrowborder" valign="top" width="80.67%" headers="mcps1.2.3.1.2 "><p id="p85551141155614"><a name="p85551141155614"></a><a name="p85551141155614"></a>如果执行线程处理某个请求的粘滞时间超过配置的粘滞线程<span>最长</span>时间 ，则该线程标记为粘滞线程。</p>
</td>
</tr>
<tr id="row20645125219535"><td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.3.1.1 "><p id="p6645125218535"><a name="p6645125218535"></a><a name="p6645125218535"></a>专用线程</p>
</td>
<td class="cellrowborder" valign="top" width="80.67%" headers="mcps1.2.3.1.2 "><p id="p164555295317"><a name="p164555295317"></a><a name="p164555295317"></a>如果某个请求独占执行线程的时间超过正常执行时间<span>且不超过</span><span>粘滞线程最长时间</span>，则该线程标记为专用线程。</p>
</td>
</tr>
<tr id="row10315203111416"><td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.3.1.1 "><p id="p23172319411"><a name="p23172319411"></a><a name="p23172319411"></a>执行总数</p>
</td>
<td class="cellrowborder" valign="top" width="80.67%" headers="mcps1.2.3.1.2 "><p id="p4575172234511"><a name="p4575172234511"></a><a name="p4575172234511"></a>是指正在执行的线程数，包含粘滞线程数、专用线程数和正常执行的线程数。</p>
</td>
</tr>
<tr id="row123016610457"><td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.3.1.1 "><p id="p73011565452"><a name="p73011565452"></a><a name="p73011565452"></a>活动执行</p>
</td>
<td class="cellrowborder" valign="top" width="80.67%" headers="mcps1.2.3.1.2 "><p id="p03018620455"><a name="p03018620455"></a><a name="p03018620455"></a>是指活动的线程数，包含空闲的线程数和正在执行的线程数。</p>
</td>
</tr>
<tr id="row1784551054511"><td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.3.1.1 "><p id="p15845101014451"><a name="p15845101014451"></a><a name="p15845101014451"></a>空闲执行</p>
</td>
<td class="cellrowborder" valign="top" width="80.67%" headers="mcps1.2.3.1.2 "><p id="p1884571074520"><a name="p1884571074520"></a><a name="p1884571074520"></a>是指处于空闲状态的线程数。 当没有任务时线程处于空闲状态，收到请求时，线程池给此请求分配一个空闲线程，任务完成后回到线程池中等待下次任务。</p>
</td>
</tr>
</tbody>
</table>

