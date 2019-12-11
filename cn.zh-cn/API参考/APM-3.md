# APM<a name="aom_04_0065"></a>

**表 1**  APM

<a name="table21011495256"></a>
<table><thead align="left"><tr id="row6821749102512"><th class="cellrowborder" valign="top" width="23.232323232323232%" id="mcps1.2.5.1.1"><p id="p1082749172511"><a name="p1082749172511"></a><a name="p1082749172511"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="28.28282828282828%" id="mcps1.2.5.1.2"><p id="p88294916253"><a name="p88294916253"></a><a name="p88294916253"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="24.242424242424242%" id="mcps1.2.5.1.3"><p id="p382349102520"><a name="p382349102520"></a><a name="p382349102520"></a>授权范围</p>
</th>
<th class="cellrowborder" valign="top" width="24.242424242424242%" id="mcps1.2.5.1.4"><p id="p18821749152512"><a name="p18821749152512"></a><a name="p18821749152512"></a>对应API接口</p>
</th>
</tr>
</thead>
<tbody><tr id="row1130073615270"><td class="cellrowborder" valign="top" width="23.232323232323232%" headers="mcps1.2.5.1.1 "><p id="p9171134415718"><a name="p9171134415718"></a><a name="p9171134415718"></a>查询应用列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.28282828282828%" headers="mcps1.2.5.1.2 "><p id="p1817194420719"><a name="p1817194420719"></a><a name="p1817194420719"></a>apm:inventory:get</p>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.3 "><a name="ul776919514308"></a><a name="ul776919514308"></a><ul id="ul776919514308"><li>支持：IAM项目(Project)</li></ul>
<a name="ul4770125153013"></a><a name="ul4770125153013"></a><ul id="ul4770125153013"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.4 "><p id="p12171164418717"><a name="p12171164418717"></a><a name="p12171164418717"></a>GET /v1/{projectId}/atps/monitorgroups</p>
</td>
</tr>
<tr id="row16299836152711"><td class="cellrowborder" valign="top" width="23.232323232323232%" headers="mcps1.2.5.1.1 "><p id="p918710449710"><a name="p918710449710"></a><a name="p918710449710"></a>查询服务列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.28282828282828%" headers="mcps1.2.5.1.2 "><p id="p1818734415710"><a name="p1818734415710"></a><a name="p1818734415710"></a>apm:ats:get</p>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.3 "><a name="ul15289116470"></a><a name="ul15289116470"></a><ul id="ul15289116470"><li>支持：IAM项目(Project)</li></ul>
<a name="ul1128913115475"></a><a name="ul1128913115475"></a><ul id="ul1128913115475"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.4 "><p id="p161872441671"><a name="p161872441671"></a><a name="p161872441671"></a>GET /v1/{projectId}/ats/applications</p>
</td>
</tr>
<tr id="row88771839192710"><td class="cellrowborder" valign="top" width="23.232323232323232%" headers="mcps1.2.5.1.1 "><p id="p18187344173"><a name="p18187344173"></a><a name="p18187344173"></a>查询服务实例列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.28282828282828%" headers="mcps1.2.5.1.2 "><p id="p3187154410716"><a name="p3187154410716"></a><a name="p3187154410716"></a>apm:ats:get</p>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.3 "><a name="ul1638913219477"></a><a name="ul1638913219477"></a><ul id="ul1638913219477"><li>支持：IAM项目(Project)</li></ul>
<a name="ul1738922144719"></a><a name="ul1738922144719"></a><ul id="ul1738922144719"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.4 "><p id="p618719446712"><a name="p618719446712"></a><a name="p618719446712"></a>GET /v1/{projectId}/ats/applications/{application}/instances</p>
</td>
</tr>
<tr id="row1687643915272"><td class="cellrowborder" valign="top" width="23.232323232323232%" headers="mcps1.2.5.1.1 "><p id="p3202154412714"><a name="p3202154412714"></a><a name="p3202154412714"></a>查询服务事务列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.28282828282828%" headers="mcps1.2.5.1.2 "><p id="p3202184412712"><a name="p3202184412712"></a><a name="p3202184412712"></a>apm:ats:get</p>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.3 "><a name="ul19431138479"></a><a name="ul19431138479"></a><ul id="ul19431138479"><li>支持：IAM项目(Project)</li></ul>
<a name="ul24317384711"></a><a name="ul24317384711"></a><ul id="ul24317384711"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.4 "><p id="p13202174412710"><a name="p13202174412710"></a><a name="p13202174412710"></a>GET /v1/{projectId}/ats/applications/{application}/transactions</p>
</td>
</tr>
<tr id="row787417392271"><td class="cellrowborder" valign="top" width="23.232323232323232%" headers="mcps1.2.5.1.1 "><p id="p22025449718"><a name="p22025449718"></a><a name="p22025449718"></a>查询调用链</p>
</td>
<td class="cellrowborder" valign="top" width="28.28282828282828%" headers="mcps1.2.5.1.2 "><p id="p11202544176"><a name="p11202544176"></a><a name="p11202544176"></a>apm:ats:get</p>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.3 "><a name="ul19656173174715"></a><a name="ul19656173174715"></a><ul id="ul19656173174715"><li>支持：IAM项目(Project)</li></ul>
<a name="ul1865612394718"></a><a name="ul1865612394718"></a><ul id="ul1865612394718"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.4 "><p id="p142025441170"><a name="p142025441170"></a><a name="p142025441170"></a>GET /v1/{projectId}/ats/traces</p>
</td>
</tr>
<tr id="row6873039172715"><td class="cellrowborder" valign="top" width="23.232323232323232%" headers="mcps1.2.5.1.1 "><p id="p16993154916464"><a name="p16993154916464"></a><a name="p16993154916464"></a>查询调用链详情</p>
</td>
<td class="cellrowborder" valign="top" width="28.28282828282828%" headers="mcps1.2.5.1.2 "><p id="p99938495463"><a name="p99938495463"></a><a name="p99938495463"></a>apm:ats:get</p>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.3 "><a name="ul578119414478"></a><a name="ul578119414478"></a><ul id="ul578119414478"><li>支持：IAM项目(Project)</li></ul>
<a name="ul17781134184710"></a><a name="ul17781134184710"></a><ul id="ul17781134184710"><li>不支持：企业项目(Enterprise Project)</li></ul>
</td>
<td class="cellrowborder" valign="top" width="24.242424242424242%" headers="mcps1.2.5.1.4 "><p id="p1993164974615"><a name="p1993164974615"></a><a name="p1993164974615"></a>GET /v1/{projectId}/ats/spans</p>
</td>
</tr>
</tbody>
</table>

