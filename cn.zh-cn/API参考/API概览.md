# API概览<a name="aom_04_0056"></a>

应用运维管理服务API为开发者、合作伙伴提供监控、弹性伸缩、日志、APM的开放接口，帮助您快速、低成本地实现应用运维。

**表 1**  API概览

<a name="table1253219238421"></a>
<table><thead align="left"><tr id="row196808238421"><th class="cellrowborder" valign="top" width="26.25%" id="mcps1.2.3.1.1"><p id="p7680192364214"><a name="p7680192364214"></a><a name="p7680192364214"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="73.75%" id="mcps1.2.3.1.2"><p id="p176806238423"><a name="p176806238423"></a><a name="p176806238423"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1368052315426"><td class="cellrowborder" valign="top" width="26.25%" headers="mcps1.2.3.1.1 "><p id="p156800230426"><a name="p156800230426"></a><a name="p156800230426"></a><a href="#section448552316427">监控</a></p>
</td>
<td class="cellrowborder" valign="top" width="73.75%" headers="mcps1.2.3.1.2 "><p id="p9472442161611"><a name="p9472442161611"></a><a name="p9472442161611"></a>监控相关的接口，包括查询指标，查询、添加监控数据，添加、修改、查询、删除阈值规则，添加、修改、查询、删除服务发现规则接口。</p>
</td>
</tr>
<tr id="row9681142311428"><td class="cellrowborder" valign="top" width="26.25%" headers="mcps1.2.3.1.1 "><p id="p16681172320424"><a name="p16681172320424"></a><a name="p16681172320424"></a><a href="#section39811452171413">弹性伸缩</a></p>
</td>
<td class="cellrowborder" valign="top" width="73.75%" headers="mcps1.2.3.1.2 "><p id="p8449134215165"><a name="p8449134215165"></a><a name="p8449134215165"></a>弹性伸缩相关的接口，包括创建、删除、更新策略，查看单个和所有策略，更新、查询策略组属性接口。</p>
</td>
</tr>
<tr id="row1156911421614"><td class="cellrowborder" valign="top" width="26.25%" headers="mcps1.2.3.1.1 "><p id="p10570181441610"><a name="p10570181441610"></a><a name="p10570181441610"></a><a href="#section180071091515">日志</a></p>
</td>
<td class="cellrowborder" valign="top" width="73.75%" headers="mcps1.2.3.1.2 "><p id="p2570141413166"><a name="p2570141413166"></a><a name="p2570141413166"></a>日志相关的接口，包括查询日志接口。</p>
</td>
</tr>
<tr id="row165701512101613"><td class="cellrowborder" valign="top" width="26.25%" headers="mcps1.2.3.1.1 "><p id="p8571111212166"><a name="p8571111212166"></a><a name="p8571111212166"></a><a href="#section9610102610152">APM</a></p>
</td>
<td class="cellrowborder" valign="top" width="73.75%" headers="mcps1.2.3.1.2 "><p id="p858019925810"><a name="p858019925810"></a><a name="p858019925810"></a>APM相关的接口，包括查询应用列表、服务列表、服务实例列表、服务事务列表、调用链、调用链详情接口。</p>
</td>
</tr>
</tbody>
</table>

## 监控<a name="section448552316427"></a>

<a name="table8491823134216"></a>
<table><thead align="left"><tr id="row768292312429"><th class="cellrowborder" valign="top" width="30%" id="mcps1.1.3.1.1"><p id="p968219233420"><a name="p968219233420"></a><a name="p968219233420"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="70%" id="mcps1.1.3.1.2"><p id="p16682923204217"><a name="p16682923204217"></a><a name="p16682923204217"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row176821123134213"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p14905134011415"><a name="p14905134011415"></a><a name="p14905134011415"></a><a href="查询指标.md">查询指标</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p176476311242"><a name="p176476311242"></a><a name="p176476311242"></a>查询当前可监控的指标列表，可以指定指标命名空间、指标名称、维度、所属资源的编号（格式为：resType_resId），分页查询的起始位置和返回的最大记录条数。</p>
</td>
</tr>
<tr id="row968242304216"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p5902104091418"><a name="p5902104091418"></a><a name="p5902104091418"></a><a href="查询监控数据.md">查询监控数据</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p1974651011252"><a name="p1974651011252"></a><a name="p1974651011252"></a>查询指定时间范围内的监控数据，可以通过参数指定需要查询的数据维度，数据周期等。</p>
</td>
</tr>
<tr id="row20682122310428"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p2901184015141"><a name="p2901184015141"></a><a name="p2901184015141"></a><a href="添加监控数据.md">添加监控数据</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p770718181002"><a name="p770718181002"></a><a name="p770718181002"></a>添加单条或多条监控数据。</p>
</td>
</tr>
<tr id="row66831323144219"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p189818406141"><a name="p189818406141"></a><a name="p189818406141"></a><a href="添加阈值规则.md">添加阈值规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p1249611498254"><a name="p1249611498254"></a><a name="p1249611498254"></a>添加单条阈值规则。</p>
</td>
</tr>
<tr id="row56830238421"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p58953404141"><a name="p58953404141"></a><a name="p58953404141"></a><a href="修改阈值规则.md">修改阈值规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p109843214012"><a name="p109843214012"></a><a name="p109843214012"></a>修改单条阈值规则。</p>
</td>
</tr>
<tr id="row268352313427"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p11892154012145"><a name="p11892154012145"></a><a name="p11892154012145"></a><a href="查询阈值规则列表.md">查询阈值规则列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p75082615265"><a name="p75082615265"></a><a name="p75082615265"></a>查询所有阈值规则。</p>
</td>
</tr>
<tr id="row6683162318424"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p289016401143"><a name="p289016401143"></a><a name="p289016401143"></a><a href="查询单条阈值规则.md">查询单条阈值规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p1988944015140"><a name="p1988944015140"></a><a name="p1988944015140"></a>查询单条阈值规则。</p>
</td>
</tr>
<tr id="row17683202310427"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p15888340101419"><a name="p15888340101419"></a><a name="p15888340101419"></a><a href="删除阈值规则.md">删除阈值规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p6887164051412"><a name="p6887164051412"></a><a name="p6887164051412"></a>删除单条阈值规则。</p>
</td>
</tr>
<tr id="row76838237426"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p18865407143"><a name="p18865407143"></a><a name="p18865407143"></a><a href="添加或修改服务发现规则.md">添加或修改服务发现规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p20885240111415"><a name="p20885240111415"></a><a name="p20885240111415"></a>添加、修改单条或多条服务发现规则。</p>
</td>
</tr>
<tr id="row11683423114213"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p138841740161411"><a name="p138841740161411"></a><a name="p138841740161411"></a><a href="查询服务发现规则.md">查询服务发现规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0135040578_p975712814512"><a name="zh-cn_topic_0135040578_p975712814512"></a><a name="zh-cn_topic_0135040578_p975712814512"></a>查询当前已存在的服务发现规则。</p>
</td>
</tr>
<tr id="row1560445111413"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p3535745191414"><a name="p3535745191414"></a><a name="p3535745191414"></a><a href="删除服务发现规则.md">删除服务发现规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p45351145171410"><a name="p45351145171410"></a><a name="p45351145171410"></a>删除单条或多条服务发现规则。</p>
</td>
</tr>
</tbody>
</table>

## 弹性伸缩<a name="section39811452171413"></a>

<a name="table1498116526144"></a>
<table><thead align="left"><tr id="row598255221420"><th class="cellrowborder" valign="top" width="30%" id="mcps1.1.3.1.1"><p id="p20982195219145"><a name="p20982195219145"></a><a name="p20982195219145"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="70%" id="mcps1.1.3.1.2"><p id="p20982452191415"><a name="p20982452191415"></a><a name="p20982452191415"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1198210528141"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p7983135221411"><a name="p7983135221411"></a><a name="p7983135221411"></a><a href="创建策略.md">创建策略</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p12983185219143"><a name="p12983185219143"></a><a name="p12983185219143"></a>创建策略。</p>
</td>
</tr>
<tr id="row69831452141410"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p99831352121419"><a name="p99831352121419"></a><a name="p99831352121419"></a><a href="删除策略.md">删除策略</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p836112257213"><a name="p836112257213"></a><a name="p836112257213"></a>删除指定策略。</p>
</td>
</tr>
<tr id="row4983752111416"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p1984552111419"><a name="p1984552111419"></a><a name="p1984552111419"></a><a href="更新策略.md">更新策略</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p139843520149"><a name="p139843520149"></a><a name="p139843520149"></a>更新策略。</p>
</td>
</tr>
<tr id="row19984185281418"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p209841652121415"><a name="p209841652121415"></a><a name="p209841652121415"></a><a href="查看策略列表.md">查看策略列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p9148144326"><a name="p9148144326"></a><a name="p9148144326"></a>查询指定项目下所有策略的详细信息。</p>
</td>
</tr>
<tr id="row1298411522146"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p1098413529148"><a name="p1098413529148"></a><a name="p1098413529148"></a><a href="查看单个策略.md">查看单个策略</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0130935561_p18110355195615"><a name="zh-cn_topic_0130935561_p18110355195615"></a><a name="zh-cn_topic_0130935561_p18110355195615"></a>查询指定项目下单个策略的详细信息。</p>
</td>
</tr>
<tr id="row7984105261414"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p1198495221413"><a name="p1198495221413"></a><a name="p1198495221413"></a><a href="更新策略组属性.md">更新策略组属性</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p1445725711212"><a name="p1445725711212"></a><a name="p1445725711212"></a>更新策略组属性。</p>
</td>
</tr>
<tr id="row1298475251417"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p1398435211142"><a name="p1398435211142"></a><a name="p1398435211142"></a><a href="查询策略组属性.md">查询策略组属性</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p199841520141"><a name="p199841520141"></a><a name="p199841520141"></a>查询策略组属性。</p>
</td>
</tr>
</tbody>
</table>

## 日志<a name="section180071091515"></a>

<a name="table280031081519"></a>
<table><thead align="left"><tr id="row1980031015154"><th class="cellrowborder" valign="top" width="30%" id="mcps1.1.3.1.1"><p id="p1280010109154"><a name="p1280010109154"></a><a name="p1280010109154"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="70%" id="mcps1.1.3.1.2"><p id="p16800410191512"><a name="p16800410191512"></a><a name="p16800410191512"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1280118103156"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p6801151051516"><a name="p6801151051516"></a><a name="p6801151051516"></a><a href="查询日志.md">查询日志</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p1380111081514"><a name="p1380111081514"></a><a name="p1380111081514"></a>查询不同维度（例如，集群、IP、应用等）下的日志内容。</p>
</td>
</tr>
</tbody>
</table>

## APM<a name="section9610102610152"></a>

<a name="table4610326201516"></a>
<table><thead align="left"><tr id="row46108260157"><th class="cellrowborder" valign="top" width="30%" id="mcps1.1.3.1.1"><p id="p1161102671518"><a name="p1161102671518"></a><a name="p1161102671518"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="70%" id="mcps1.1.3.1.2"><p id="p46111226121517"><a name="p46111226121517"></a><a name="p46111226121517"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row6611926151515"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p1861112262155"><a name="p1861112262155"></a><a name="p1861112262155"></a><a href="查询应用列表.md">查询应用列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p161112641510"><a name="p161112641510"></a><a name="p161112641510"></a>查询应用列表。</p>
</td>
</tr>
<tr id="row1861114266150"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p261152611159"><a name="p261152611159"></a><a name="p261152611159"></a><a href="查询服务列表.md">查询服务列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p1161142619157"><a name="p1161142619157"></a><a name="p1161142619157"></a>查询服务列表。</p>
</td>
</tr>
<tr id="row2061119263156"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p15611162614158"><a name="p15611162614158"></a><a name="p15611162614158"></a><a href="查询服务实例列表.md">查询服务实例列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p938531814296"><a name="p938531814296"></a><a name="p938531814296"></a>查询指定服务下的实例列表。</p>
</td>
</tr>
<tr id="row196111026171520"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p8611112681514"><a name="p8611112681514"></a><a name="p8611112681514"></a><a href="查询服务事务列表.md">查询服务事务列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="p1561242631510"><a name="p1561242631510"></a><a name="p1561242631510"></a>查询指定服务下的事务列表。</p>
</td>
</tr>
<tr id="row15612202611513"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p12612192613158"><a name="p12612192613158"></a><a name="p12612192613158"></a><a href="查询调用链.md">查询调用链</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0154976251_zh-cn_topic_0095238331_zh-cn_topic_0082840623_p152651981568"><a name="zh-cn_topic_0154976251_zh-cn_topic_0095238331_zh-cn_topic_0082840623_p152651981568"></a><a name="zh-cn_topic_0154976251_zh-cn_topic_0095238331_zh-cn_topic_0082840623_p152651981568"></a>根据查询条件查询调用链数据。</p>
</td>
</tr>
<tr id="row17612142618157"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.3.1.1 "><p id="p86121826141515"><a name="p86121826141515"></a><a name="p86121826141515"></a><a href="查询调用链详情.md">查询调用链详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0154976252_zh-cn_topic_0095238332_zh-cn_topic_0082840624_p109011744205612"><a name="zh-cn_topic_0154976252_zh-cn_topic_0095238332_zh-cn_topic_0082840624_p109011744205612"></a><a name="zh-cn_topic_0154976252_zh-cn_topic_0095238332_zh-cn_topic_0082840624_p109011744205612"></a>根据调用链的traceId信息查询调用链详情。</p>
</td>
</tr>
</tbody>
</table>

