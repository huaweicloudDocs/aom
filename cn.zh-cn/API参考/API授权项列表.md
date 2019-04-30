# API授权项列表<a name="ZH-CN_TOPIC_0130753547"></a>

此功能目前仅对华北-北京一区域、华东-上海二区域和华南-广州区域开放。

**表 1**  API授权项列表

<a name="table181863315109"></a>
<table><thead align="left"><tr id="row418623110104"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p6186143119106"><a name="p6186143119106"></a><a name="p6186143119106"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p818683117109"><a name="p818683117109"></a><a name="p818683117109"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p81861631141012"><a name="p81861631141012"></a><a name="p81861631141012"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="35%" id="mcps1.2.5.1.4"><p id="p94971820113617"><a name="p94971820113617"></a><a name="p94971820113617"></a>授权作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row14186531161010"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p181371562148"><a name="p181371562148"></a><a name="p181371562148"></a>POST /v1/{project_id}/ams/metrics</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p13186131101014"><a name="p13186131101014"></a><a name="p13186131101014"></a>查询指标</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p118613311100"><a name="p118613311100"></a><a name="p118613311100"></a>aom:metric:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul697925564613"></a><a name="ul697925564613"></a><ul id="ul697925564613"><li>支持：项目(Project)</li></ul>
<a name="ul17982455204616"></a><a name="ul17982455204616"></a><ul id="ul17982455204616"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row018615312107"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p0186173191012"><a name="p0186173191012"></a><a name="p0186173191012"></a>POST /v1/{project_id}/ams/metricdata</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p10186163171015"><a name="p10186163171015"></a><a name="p10186163171015"></a>查询监控数据</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p111861331181018"><a name="p111861331181018"></a><a name="p111861331181018"></a>aom:metric:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul1821541793719"></a><a name="ul1821541793719"></a><ul id="ul1821541793719"><li>支持：项目(Project)</li></ul>
<a name="ul3218111713372"></a><a name="ul3218111713372"></a><ul id="ul3218111713372"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row91861431191014"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p38367706"><a name="p38367706"></a><a name="p38367706"></a>POST /v1/{project_id}/ams/alarms</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1818813110105"><a name="p1818813110105"></a><a name="p1818813110105"></a>添加阈值规则</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1018815312100"><a name="p1018815312100"></a><a name="p1018815312100"></a>aom:alarmRule:create</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul158611184374"></a><a name="ul158611184374"></a><ul id="ul158611184374"><li>支持：项目(Project)</li></ul>
<a name="ul1881818153713"></a><a name="ul1881818153713"></a><ul id="ul1881818153713"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row018816314109"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p162455442316"><a name="p162455442316"></a><a name="p162455442316"></a>PUT /v1/{project_id}/ams/alarms</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p3188133121018"><a name="p3188133121018"></a><a name="p3188133121018"></a>修改阈值规则</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p7188103111108"><a name="p7188103111108"></a><a name="p7188103111108"></a>aom:alarmRule:set</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul1878171916379"></a><a name="ul1878171916379"></a><ul id="ul1878171916379"><li>支持：项目(Project)</li></ul>
<a name="ul3802196374"></a><a name="ul3802196374"></a><ul id="ul3802196374"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row20188103118105"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p22125742"><a name="p22125742"></a><a name="p22125742"></a>GET /v1/{project_id}/ams/alarms</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1018863119107"><a name="p1018863119107"></a><a name="p1018863119107"></a>查询阈值规则列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p61881831111010"><a name="p61881831111010"></a><a name="p61881831111010"></a>aom:alarmRule:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul1731417205375"></a><a name="ul1731417205375"></a><ul id="ul1731417205375"><li>支持：项目(Project)</li></ul>
<a name="ul19316520103712"></a><a name="ul19316520103712"></a><ul id="ul19316520103712"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row111888318107"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p25171793"><a name="p25171793"></a><a name="p25171793"></a>GET /v1/{project_id}/ams/alarms/{alarm_id}</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1242615201185"><a name="p1242615201185"></a><a name="p1242615201185"></a>查询单条阈值规则</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1318833117107"><a name="p1318833117107"></a><a name="p1318833117107"></a>aom:alarmRule:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul2030842153716"></a><a name="ul2030842153716"></a><ul id="ul2030842153716"><li>支持：项目(Project)</li></ul>
<a name="ul19310921173713"></a><a name="ul19310921173713"></a><ul id="ul19310921173713"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1858704991820"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p57388118"><a name="p57388118"></a><a name="p57388118"></a>DELETE /v1/{project_id}/ams/alarms/{alarm_id}</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p913510568182"><a name="p913510568182"></a><a name="p913510568182"></a>删除阈值规则</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1588149131818"><a name="p1588149131818"></a><a name="p1588149131818"></a>aom:alarmRule:delete</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul17296152210377"></a><a name="ul17296152210377"></a><ul id="ul17296152210377"><li>支持：项目(Project)</li></ul>
<a name="ul11298152211376"></a><a name="ul11298152211376"></a><ul id="ul11298152211376"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row146871357987"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p65120597504"><a name="p65120597504"></a><a name="p65120597504"></a>PUT /v1/{project_id}/inv/servicediscoveryrules</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p91911925144417"><a name="p91911925144417"></a><a name="p91911925144417"></a>添加或修改服务发现规则</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1858113310461"><a name="p1858113310461"></a><a name="p1858113310461"></a>aom:discoveryRule:set</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul1457314543474"></a><a name="ul1457314543474"></a><ul id="ul1457314543474"><li>支持：项目(Project)</li></ul>
<a name="ul85771554114716"></a><a name="ul85771554114716"></a><ul id="ul85771554114716"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row4769992914"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p05122590505"><a name="p05122590505"></a><a name="p05122590505"></a>GET /v1/{project_id}/inv/servicediscoveryrules</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p11410925124518"><a name="p11410925124518"></a><a name="p11410925124518"></a>查询服务发现规则</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p185843313462"><a name="p185843313462"></a><a name="p185843313462"></a>aom:discoveryRule:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul79647559472"></a><a name="ul79647559472"></a><ul id="ul79647559472"><li>支持：项目(Project)</li></ul>
<a name="ul179671255134715"></a><a name="ul179671255134715"></a><ul id="ul179671255134715"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row557813410919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1951212593502"><a name="p1951212593502"></a><a name="p1951212593502"></a>DELETE /v1/{project_id}/inv/servicediscoveryrules</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p84101425154517"><a name="p84101425154517"></a><a name="p84101425154517"></a>删除服务发现规则</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p98581733134610"><a name="p98581733134610"></a><a name="p98581733134610"></a>aom:discoveryRule:delete</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul4700156154715"></a><a name="ul4700156154715"></a><ul id="ul4700156154715"><li>支持：项目(Project)</li></ul>
<a name="ul12703195616478"></a><a name="ul12703195616478"></a><ul id="ul12703195616478"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row159583822212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0082628667_p47548937"><a name="zh-cn_topic_0082628667_p47548937"></a><a name="zh-cn_topic_0082628667_p47548937"></a>POST /v1/{project_id}/pe/policy</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p17959981227"><a name="p17959981227"></a><a name="p17959981227"></a>创建策略</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p8959128162217"><a name="p8959128162217"></a><a name="p8959128162217"></a>aom:autoScalingRule:create</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul836812239376"></a><a name="ul836812239376"></a><ul id="ul836812239376"><li>支持：项目(Project)</li></ul>
<a name="ul6370112315375"></a><a name="ul6370112315375"></a><ul id="ul6370112315375"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row99878127220"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0082628668_p26867045"><a name="zh-cn_topic_0082628668_p26867045"></a><a name="zh-cn_topic_0082628668_p26867045"></a>DELETE /v1/{project_id}/pe/policy</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p119873123229"><a name="p119873123229"></a><a name="p119873123229"></a>删除策略</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p8987912152211"><a name="p8987912152211"></a><a name="p8987912152211"></a>aom:autoScalingRule:delete</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul8275132416377"></a><a name="ul8275132416377"></a><ul id="ul8275132416377"><li>支持：项目(Project)</li></ul>
<a name="ul4277162410377"></a><a name="ul4277162410377"></a><ul id="ul4277162410377"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row8912191672212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1690013162222"><a name="p1690013162222"></a><a name="p1690013162222"></a>PUT  /v1/{project_id}/pe/policy/{policy_id}</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p790110161226"><a name="p790110161226"></a><a name="p790110161226"></a>更新策略</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p18901716132210"><a name="p18901716132210"></a><a name="p18901716132210"></a>aom:autoScalingRule:update</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul95722025193716"></a><a name="ul95722025193716"></a><ul id="ul95722025193716"><li>支持：项目(Project)</li></ul>
<a name="ul557452510371"></a><a name="ul557452510371"></a><ul id="ul557452510371"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row149112016132216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1190217163227"><a name="p1190217163227"></a><a name="p1190217163227"></a>GET /v1/{project_id}/pe/policy</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p89031716142215"><a name="p89031716142215"></a><a name="p89031716142215"></a>查看策略列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p17903151692212"><a name="p17903151692212"></a><a name="p17903151692212"></a>aom:autoScalingRule:list</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul1365212683712"></a><a name="ul1365212683712"></a><ul id="ul1365212683712"><li>支持：项目(Project)</li></ul>
<a name="ul66541026123710"></a><a name="ul66541026123710"></a><ul id="ul66541026123710"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row187618177228"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13868217142216"><a name="p13868217142216"></a><a name="p13868217142216"></a>GET /v1/{project_id}/pe/policy/{policy_id}</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1986814177226"><a name="p1986814177226"></a><a name="p1986814177226"></a>查看单个策略</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1187071714222"><a name="p1187071714222"></a><a name="p1187071714222"></a>aom:autoScalingRule:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul6588927133719"></a><a name="ul6588927133719"></a><ul id="ul6588927133719"><li>支持：项目(Project)</li></ul>
<a name="ul1590227133713"></a><a name="ul1590227133713"></a><ul id="ul1590227133713"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row10876317172211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p633635113373"><a name="p633635113373"></a><a name="p633635113373"></a>PUT  /v1/{project_id}/pe/policy/config</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p19872217162219"><a name="p19872217162219"></a><a name="p19872217162219"></a>更新策略组属性</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p198721217182211"><a name="p198721217182211"></a><a name="p198721217182211"></a>aom:autoScalingRule:update</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul1689929103717"></a><a name="ul1689929103717"></a><ul id="ul1689929103717"><li>支持：项目(Project)</li></ul>
<a name="ul136918299375"></a><a name="ul136918299375"></a><ul id="ul136918299375"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1067718203225"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p512721141412"><a name="p512721141412"></a><a name="p512721141412"></a>GET  /v1/{project_id}/pe/policy/config</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1767762052213"><a name="p1767762052213"></a><a name="p1767762052213"></a>查询策略组属性</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p767762010228"><a name="p767762010228"></a><a name="p767762010228"></a>aom:autoScalingRule:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul1689113053720"></a><a name="ul1689113053720"></a><ul id="ul1689113053720"><li>支持：项目(Project)</li></ul>
<a name="ul12692330133714"></a><a name="ul12692330133714"></a><ul id="ul12692330133714"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row1623050155711"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p12171164418717"><a name="p12171164418717"></a><a name="p12171164418717"></a>GET /v1/{projectId}/atps/monitorgroups</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p9171134415718"><a name="p9171134415718"></a><a name="p9171134415718"></a>查询应用列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1817194420719"><a name="p1817194420719"></a><a name="p1817194420719"></a>apm:inventory:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul10187044177"></a><a name="ul10187044177"></a><ul id="ul10187044177"><li>支持：项目(Project)</li></ul>
<a name="ul15187184412711"></a><a name="ul15187184412711"></a><ul id="ul15187184412711"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row65761458574"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p161872441671"><a name="p161872441671"></a><a name="p161872441671"></a>GET /v1/{projectId}/ats/applications</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p918710449710"><a name="p918710449710"></a><a name="p918710449710"></a>查询服务列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1818734415710"><a name="p1818734415710"></a><a name="p1818734415710"></a>apm:ats:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul11187444872"></a><a name="ul11187444872"></a><ul id="ul11187444872"><li>支持：项目(Project)</li></ul>
<a name="ul7187944171"></a><a name="ul7187944171"></a><ul id="ul7187944171"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row145665675715"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p618719446712"><a name="p618719446712"></a><a name="p618719446712"></a>GET /v1/{projectId}/ats/applications/{application}/instances</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p18187344173"><a name="p18187344173"></a><a name="p18187344173"></a>查询服务实例列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p3187154410716"><a name="p3187154410716"></a><a name="p3187154410716"></a>apm:ats:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul81874441679"></a><a name="ul81874441679"></a><ul id="ul81874441679"><li>支持：项目(Project)</li></ul>
<a name="ul11871441071"></a><a name="ul11871441071"></a><ul id="ul11871441071"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row74713735714"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13202174412710"><a name="p13202174412710"></a><a name="p13202174412710"></a>GET /v1/{projectId}/ats/applications/{application}/transactions</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p3202154412714"><a name="p3202154412714"></a><a name="p3202154412714"></a>查询服务事务列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p3202184412712"><a name="p3202184412712"></a><a name="p3202184412712"></a>apm:ats:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul1120213447712"></a><a name="ul1120213447712"></a><ul id="ul1120213447712"><li>支持：项目(Project)</li></ul>
<a name="ul1720244420718"></a><a name="ul1720244420718"></a><ul id="ul1720244420718"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row34164875712"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p142025441170"><a name="p142025441170"></a><a name="p142025441170"></a>GET /v1/{projectId}/ats/traces</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p22025449718"><a name="p22025449718"></a><a name="p22025449718"></a>查询调用链</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p11202544176"><a name="p11202544176"></a><a name="p11202544176"></a>apm:ats:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul102021444878"></a><a name="ul102021444878"></a><ul id="ul102021444878"><li>支持：项目(Project)</li></ul>
<a name="ul821884410719"></a><a name="ul821884410719"></a><ul id="ul821884410719"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
<tr id="row544709185710"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1993164974615"><a name="p1993164974615"></a><a name="p1993164974615"></a>GET /v1/{projectId}/ats/spans</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p16993154916464"><a name="p16993154916464"></a><a name="p16993154916464"></a>查询调用链详情</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p99938495463"><a name="p99938495463"></a><a name="p99938495463"></a>apm:ats:get</p>
</td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.5.1.4 "><a name="ul1199311494462"></a><a name="ul1199311494462"></a><ul id="ul1199311494462"><li>支持：项目(Project)</li></ul>
<a name="ul399319499464"></a><a name="ul399319499464"></a><ul id="ul399319499464"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
</tr>
</tbody>
</table>

