# APP端汇总<a name="ZH-CN_TOPIC_0129033179"></a>

## Mobile简介<a name="section1344432144616"></a>

华为云应用性能管理-Mobile致力于为您提供清晰直观的移动APP性能监控数据，通过用户体验、吞吐量、错误数、Crash、ANR（Application Not Response）等多项指标，为您展现不同维度的移动APP性能数据，助您快速定位性能瓶颈，完成移动APP性能优化。

在用户体验至上的互联网时代，移动APP的用户体验至关重要，成为移动APP是否成功的关键因素之一，然而移动APP通常安装在用户手机上，企业往往无法感知到真实的用户体验，只能依靠调研随访、用户反馈等方式收集用户意见，从而对移动APP进行优化。可想而知，这种方式并不高效，甚至并没有效果。

华为云应用性能管理Mobile端侧监控采用非侵入式埋点技术，只需简单的一个命令行即可完成业务代码埋点。使用华为云应用性能管理-Mobile您将瞬间和您在全球各地的用户建立联系，实时感知他们的用户体验。海内存知己，天涯若比邻，即使相隔千里，用户的使用体验也将即刻在您的APP汇总页面上呈现，快速发现性能瓶颈，完成性能优化，助您实现商业成功。

## 监控指标说明<a name="zh-cn_topic_0127936422_section66421051185312"></a>

**用户体验**

华为云应用性能管理服务使用Apdex（Application Performance Index）度量用户体验，根据用户等待响应的时间将每次网络请求评估为满意、可容忍、不满意三个等级，并根据公式进行计算，量化用户体验，帮助您了解应用基本情况。

**吞吐量**

吞吐量指的是指定时间内用户进行网络请求的总次数。

**时延（TP99时延）**

时延（TP99时延）是指满足百分之九十九的网络请求所需要的最低耗时。例如，有四次请求耗时分别为：10ms、100ms、500ms、20ms，那么时延（TP99时延）则是这么计算的：4次请求中，99%的请求数为4\*99%，进位取整得4。也就是99%的请求次数为4次。而满足这4次请求的最低耗时为500ms，那么TP99时延为500ms。

**错误数**

错误数是指用户进行网络请求失败的次数。

**移动应用Crash个数**

应用的Crash个数指标图可以直观的展示您当前应用Crash频率，未来华为移动APP会提供更多Crash统计指标和展示Crash详情的能力，能让您更加全面的掌握APP的Crash问题。

**地域分布**

基于地理位置的移动应用的统计信息能够帮您直观的展示全球各地的人们使用APP的情况，为您优化移动APP提供最直观、最精准的信息。

**拓扑**

华为云移动APP性能检测提供了端到端展示应用拓扑的能力。即使您只购买了移动端的探针我们也能为您展示移动APP和所有外部应用的交互信息。如果您同时购买了移动端和云服务的探针，我们将为您展示端到端的全景应用拓扑。

## APP端汇总界面操作<a name="zh-cn_topic_0127936422_section16744158919"></a>

通过单击APP端汇总页左侧的![](figures/zh-cn_image_0129033304.png)解锁按钮，您可对汇总页面中的控件进行如下表操作。

<a name="zh-cn_topic_0127936422_table16941192520152"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127936422_row6826364"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0127936422_p16064575"><a name="zh-cn_topic_0127936422_p16064575"></a><a name="zh-cn_topic_0127936422_p16064575"></a>操作对象</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0127936422_p26162236"><a name="zh-cn_topic_0127936422_p26162236"></a><a name="zh-cn_topic_0127936422_p26162236"></a>操作</p>
</th>
<th class="cellrowborder" valign="top" width="70%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0127936422_p38766361"><a name="zh-cn_topic_0127936422_p38766361"></a><a name="zh-cn_topic_0127936422_p38766361"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127936422_row53067518"><td class="cellrowborder" rowspan="4" valign="top" width="15%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0127936422_p3501716"><a name="zh-cn_topic_0127936422_p3501716"></a><a name="zh-cn_topic_0127936422_p3501716"></a>汇总界面</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0127936422_p15203586"><a name="zh-cn_topic_0127936422_p15203586"></a><a name="zh-cn_topic_0127936422_p15203586"></a>锁定</p>
</td>
<td class="cellrowborder" rowspan="4" valign="top" width="70%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0127936422_p23530993"><a name="zh-cn_topic_0127936422_p23530993"></a><a name="zh-cn_topic_0127936422_p23530993"></a>通过单击APP端汇总页左侧的<a name="zh-cn_topic_0127936422_image12241115217359"></a><a name="zh-cn_topic_0127936422_image12241115217359"></a><span><img id="zh-cn_topic_0127936422_image12241115217359" src="figures/zh-cn_image_0129033307.png"></span>解锁按钮，可添加、删除、重置汇总页面的控件。</p>
<p id="zh-cn_topic_0127936422_p10452353"><a name="zh-cn_topic_0127936422_p10452353"></a><a name="zh-cn_topic_0127936422_p10452353"></a><a name="zh-cn_topic_0127936422_image050623012318"></a><a name="zh-cn_topic_0127936422_image050623012318"></a><span><img id="zh-cn_topic_0127936422_image050623012318" src="figures/zh-cn_image_0129033310.png"></span></p>
</td>
</tr>
<tr id="zh-cn_topic_0127936422_row41334227"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0127936422_p59738106"><a name="zh-cn_topic_0127936422_p59738106"></a><a name="zh-cn_topic_0127936422_p59738106"></a>添加</p>
</td>
</tr>
<tr id="zh-cn_topic_0127936422_row7957714175513"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0127936422_p4958314135514"><a name="zh-cn_topic_0127936422_p4958314135514"></a><a name="zh-cn_topic_0127936422_p4958314135514"></a>删除</p>
</td>
</tr>
<tr id="zh-cn_topic_0127936422_row772049"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0127936422_p62536018"><a name="zh-cn_topic_0127936422_p62536018"></a><a name="zh-cn_topic_0127936422_p62536018"></a>重置</p>
</td>
</tr>
<tr id="zh-cn_topic_0127936422_row15716008"><td class="cellrowborder" rowspan="2" valign="top" width="15%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0127936422_p65037115"><a name="zh-cn_topic_0127936422_p65037115"></a><a name="zh-cn_topic_0127936422_p65037115"></a>控件</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0127936422_p33514934"><a name="zh-cn_topic_0127936422_p33514934"></a><a name="zh-cn_topic_0127936422_p33514934"></a>删除</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="70%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0127936422_p30355138"><a name="zh-cn_topic_0127936422_p30355138"></a><a name="zh-cn_topic_0127936422_p30355138"></a>通过单击APP端汇总页左侧的<a name="zh-cn_topic_0127936422_image7220105553514"></a><a name="zh-cn_topic_0127936422_image7220105553514"></a><span><img id="zh-cn_topic_0127936422_image7220105553514" src="figures/zh-cn_image_0129033313.png"></span>解锁按钮，在每个控件可进行对控件的“删除”，对控件视图“放大”的操作。</p>
<p id="zh-cn_topic_0127936422_p17540145514296"><a name="zh-cn_topic_0127936422_p17540145514296"></a><a name="zh-cn_topic_0127936422_p17540145514296"></a><a name="zh-cn_topic_0127936422_image49371858193614"></a><a name="zh-cn_topic_0127936422_image49371858193614"></a><span><img id="zh-cn_topic_0127936422_image49371858193614" src="figures/zh-cn_image_0129033316.png"></span></p>
</td>
</tr>
<tr id="zh-cn_topic_0127936422_row4760790"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0127936422_p50079677"><a name="zh-cn_topic_0127936422_p50079677"></a><a name="zh-cn_topic_0127936422_p50079677"></a>放大</p>
</td>
</tr>
</tbody>
</table>

