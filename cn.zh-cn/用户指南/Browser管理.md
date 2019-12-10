# Browser管理<a name="aom_02_0073"></a>

Browser管理即创建浏览器应用。

## 新建浏览器应用<a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_section1896116102227"></a>

1.  登录AOM控制台，在左侧导航栏中选择“Browser \> 管理”。
2.  创建浏览器应用。单击“创建浏览器应用”，按提示输入应用名称后点击“生成”，系统将生成专属您应用的埋点命令行。

    ![](figures/zh-cn_image_0188093536.png)

3.  单击“完成拷贝”，完成应用创建并自动拷贝命令行到剪贴板。

    >![](public_sys-resources/icon-notice.gif) **须知：**   
    >若您的页面涉及跨域访问，您需要在跨域目标服务器上配置以下自定义Header：Access-Control-Allow-Methods: POST,OPTIONS,GET,PUTAccess-Control-Allow-Headers: X-Application-Id,Content-Type,X-EP-App-Id,X-App-Id,Pinpoint-TxType,Pinpoint-SrcResId,Pinpoint-TraceID,Pinpoint-pSpanID,Pinpoint-SpanID,X-Device-Id,X-Forwarded-For,X-Real-IpAccess-Control-Expose-Headers: Date,X-Dest-Resource-Id,Pinpoint-TxType,Pinpoint-SrcResId,X-App-Id,Pinpoint-CallChain,Zipkin-TraceID,Pinpoint-MonitorG,Timing-Allow-Origin  


## 嵌入命令行<a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_section12998155554416"></a>

1.  在应用创建完成后，埋点命令行就已存在于剪贴板中。若您不慎丢失命令行，可在列表“操作”列点击“查看埋点命令行”。

    ![](figures/zh-cn_image_0188093630.png)

2.  在“查看埋点命令行”弹框中单击“完成拷贝”重新获取埋点命令行。

    ![](figures/查看埋点命令行1.png)

3.  将命令行粘贴在您想要监控的页面的HTML文件中**<head\>**代码块的**第一行**，然后重启应用即可。

    >![](public_sys-resources/icon-notice.gif) **须知：**   
    >如果相比全站的监控数据您更关心单页面的监控数据，您可以为单页面创建一个应用并嵌入它的专属命令行，这样通过该应用即可查看单页面的监控数据。  


## 更多浏览器管理界面操作<a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_section16744158919"></a>

在浏览器管理中，您还可以执行如下表操作。

**表 1**  相关操作

<a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_table15831736105910"></a>
<table><thead align="left"><tr id="zh-cn_topic_0129033177_zh-cn_topic_0127936427_row14583153620596"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p10583203610596"><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p10583203610596"></a><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p10583203610596"></a>操作</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p35838364598"><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p35838364598"></a><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p35838364598"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0129033177_zh-cn_topic_0127936427_row019992094812"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p205831436115916"><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p205831436115916"></a><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p205831436115916"></a>跳转到拓扑界面</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p1167075833016"><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p1167075833016"></a><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p1167075833016"></a>单击列表“操作”列的“查看拓扑”，可跳转到Browser拓扑界面详细查看调用过程。</p>
</td>
</tr>
<tr id="zh-cn_topic_0129033177_zh-cn_topic_0127936427_row185831236125917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p1358333615919"><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p1358333615919"></a><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p1358333615919"></a>跳转到浏览器汇总界面</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p2317132418122"><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p2317132418122"></a><a name="zh-cn_topic_0129033177_zh-cn_topic_0127936427_p2317132418122"></a>单击列表“操作”列的“查看汇总”，可跳转到浏览器汇总界面，查看用户体验详情。</p>
</td>
</tr>
</tbody>
</table>

