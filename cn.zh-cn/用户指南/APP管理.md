# APP管理<a name="apm_02_0031"></a>

APP管理即创建移动APP应用。

>![](public_sys-resources/icon-note.gif) **说明：**   
>1.  Mobile探针需要的手机权限：  
>    权限1：android.permission.INTERNET  
>    权限2：android.permission.ACCESS\_NETWORK\_STATE  
>2.  执行埋点命令工具的环境必须安装Java1.8及以上版本，并设置了正确的JAVA\_HOME环境变量。  

## 新建移动APP应用<a name="zh-cn_topic_0171729842_section091961131017"></a>

1.  在左侧导航栏中选择“Mobile”，展开选项卡，单击“APP管理”。
2.  单击“创建APP”，按提示输入应用名称并选择APP类型后点击“生成”，系统将生成专属您应用的埋点命令行。

    黑色背景框中会生成Windows和Linux的命令行。

    ![](figures/zh-cn_image_0191419114.png)

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >APP类型支持Android和IOS两种。  

3.  单击“完成拷贝”，完成应用创建并自动拷贝命令行到剪贴板。
4.  将拷贝的命令行粘贴到记事本文档，待埋点时使用。

## 为APP埋点<a name="zh-cn_topic_0171729842_section4804959132419"></a>

如何为APP埋点请参见[快速接入Mobile](https://support.huaweicloud.com/qs-apm/apm_00_0012.html)。

## 埋点命令行<a name="zh-cn_topic_0171729842_section4222102941910"></a>

1.  在应用创建完成后，埋点命令行就已存在于剪贴板中。若您不慎丢失命令行，或需要埋点升级的app，请在操作列单击“查看埋点命令行”。

    ![](figures/zh-cn_image_0185276084.png)

2.  在“查看埋点命令行”弹框中单击“完成拷贝”重新获取埋点命令行。

    ![](figures/查看埋点命令行2.png)

3.  重新执行埋点过程生成新的APK文件。

    等待3分钟，移动APP的性能统计数据就会发送到Mobile后台服务器上，此时，进入已创建APP的汇总页面就可以看到APP的性能数据。同时在Mobile拓扑页面中也可以看到对应后台服务的拓扑信息，将前端展开后就可以看到Android的统计信息。


## 更多APP管理界面操作<a name="zh-cn_topic_0171729842_section16744158919"></a>

在APP管理中，您还可以执行如[表1](#zh-cn_topic_0171729842_table15831736105910)操作。

**表 1**  相关操作

<a name="zh-cn_topic_0171729842_table15831736105910"></a>
<table><thead align="left"><tr id="zh-cn_topic_0171729842_row14583153620596"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0171729842_p10583203610596"><a name="zh-cn_topic_0171729842_p10583203610596"></a><a name="zh-cn_topic_0171729842_p10583203610596"></a>操作</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0171729842_p35838364598"><a name="zh-cn_topic_0171729842_p35838364598"></a><a name="zh-cn_topic_0171729842_p35838364598"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0171729842_row1058316369591"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0171729842_p3583036195916"><a name="zh-cn_topic_0171729842_p3583036195916"></a><a name="zh-cn_topic_0171729842_p3583036195916"></a>全选或者取消全选</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0171729842_p258317365591"><a name="zh-cn_topic_0171729842_p258317365591"></a><a name="zh-cn_topic_0171729842_p258317365591"></a>可通过<a name="zh-cn_topic_0171729842_image15495131411915"></a><a name="zh-cn_topic_0171729842_image15495131411915"></a><span><img id="zh-cn_topic_0171729842_image15495131411915" src="figures/icon-全选2.png"></span>全选APP管理表中行，通过<a name="zh-cn_topic_0171729842_image19871195411259"></a><a name="zh-cn_topic_0171729842_image19871195411259"></a><span><img id="zh-cn_topic_0171729842_image19871195411259" src="figures/icon-取消全选2.png" width="21.28" height="20.354719"></span>可取消全选。</p>
</td>
</tr>
<tr id="zh-cn_topic_0171729842_row019992094812"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0171729842_p159781620175512"><a name="zh-cn_topic_0171729842_p159781620175512"></a><a name="zh-cn_topic_0171729842_p159781620175512"></a>跳转到拓扑界面</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0171729842_p1167075833016"><a name="zh-cn_topic_0171729842_p1167075833016"></a><a name="zh-cn_topic_0171729842_p1167075833016"></a>在操作列单击“查看拓扑”，可跳转到Mobile拓扑界面详细查看调用过程。</p>
</td>
</tr>
<tr id="zh-cn_topic_0171729842_row185831236125917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0171729842_p1358333615919"><a name="zh-cn_topic_0171729842_p1358333615919"></a><a name="zh-cn_topic_0171729842_p1358333615919"></a>跳转到APP汇总界面</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0171729842_p2317132418122"><a name="zh-cn_topic_0171729842_p2317132418122"></a><a name="zh-cn_topic_0171729842_p2317132418122"></a>在操作列单击“查看汇总”，可跳转到APP汇总界面，查看用户体验详情。</p>
</td>
</tr>
</tbody>
</table>

