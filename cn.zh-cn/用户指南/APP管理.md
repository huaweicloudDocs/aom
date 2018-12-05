# APP管理<a name="ZH-CN_TOPIC_0129033201"></a>

APP管理即创建移动APP应用。

>![](public_sys-resources/icon-note.gif) **说明：**   
>1.  Mobile探针需要的手机权限：  
>    权限1：android.permission.INTERNET  
>    权限2：android.permission.ACCESS\_NETWORK\_STATE  
>2.  执行埋点命令行的环境必须安装Java1.8及以上版本，并设置了正确的JAVA\_HOME环境变量。  

## 新建移动APP应用<a name="zh-cn_topic_0127936423_section091961131017"></a>

1.  登录[应用运维管理](https://console.huaweicloud.com/aom/#/aom/ams/summary)。
2.  在左侧导航栏中选择“Mobile”，展开选项卡，单击“APP管理”。
3.  单击“下载埋点工具包”下载埋点工具，并解压埋点工具包到本地。

    Windows：

    ![](figures/zh-cn_image_0129033208.jpg)

    Linux：

    ![](figures/zh-cn_image_0129033211.jpg)

4.  创建APP。单击“添加”，按提示输入应用名称后点击“生成”，系统将生成专属您应用的埋点命令行。

    黑色背景框中会生成Windows和Linux的命令行。

    ![](figures/zh-cn_image_0129033214.png)

5.  单击“完成拷贝”，完成应用创建并自动拷贝命令行到剪贴板。
6.  将拷贝的命令行粘贴到记事本文档，将其中的\{APK\_PATH\}替换为您的实际apk地址。

    Windows：

    1.  进入apk\_instrumenter文件夹。
    2.  在当前文件夹打开命令行：

        ![](figures/zh-cn_image_0129033217.png)

    3.  把生成的Windows命令行中的 “\{APK\_PATH\}” 替换为需要埋点的apk全路径。

        ![](figures/zh-cn_image_0129033220.png)


    Linux:

    1.  进入apk\_instrumenter文件夹
    2.  把生成的Linux命令行中的 “\{APK\_PATH\}” 替换为需要埋点的apk全路径，例：

        ![](figures/zh-cn_image_0129033223.png)


7.  根据您运行埋点的操作系统拷贝对应执行命令行运行命令。

    Windows

    1.  在刚才打开的cmd中执行替换好的命令行

        ![](figures/zh-cn_image_0129033226.jpg)

    2.  埋点完成后会弹出一个文件夹，文件夹中包含了原始apk和埋点后的apk，名称如

        ![](figures/zh-cn_image_0129033229.jpg)


    Linux:

    在apk\_instrumenter目录下执行埋点命令行，执行完毕后生成的apk会显示在命令行中：

    ![](figures/zh-cn_image_0142529170.png)

8.  将APK签名即可发布安装。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >**埋点完成后是不带签名的，需要用户自己对生成后的apk进行签名**。  


## 埋点命令行<a name="zh-cn_topic_0127936423_section4222102941910"></a>

1.  在应用创建完成后，埋点命令行就已存在于剪贴板中。若您不慎丢失命令行，或需要埋点升级的app，可在列表右侧的动作列单击![](figures/zh-cn_image_0129033235.png)按钮。

    ![](figures/zh-cn_image_0129033238.png)

2.  在“查看埋点命令行”弹框中单击“完成拷贝”重新获取埋点命令行。

    ![](figures/zh-cn_image_0129033241.png)

3.  重新执行埋点过程生成新的APK文件即可。

## 更多APP管理界面操作<a name="zh-cn_topic_0127936423_section16744158919"></a>

在APP管理中，您还可以执行如下表操作。

**表 1**  相关操作

<a name="zh-cn_topic_0127936423_table15831736105910"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127936423_row14583153620596"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0127936423_p10583203610596"><a name="zh-cn_topic_0127936423_p10583203610596"></a><a name="zh-cn_topic_0127936423_p10583203610596"></a>操作</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0127936423_p35838364598"><a name="zh-cn_topic_0127936423_p35838364598"></a><a name="zh-cn_topic_0127936423_p35838364598"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127936423_row1058316369591"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127936423_p3583036195916"><a name="zh-cn_topic_0127936423_p3583036195916"></a><a name="zh-cn_topic_0127936423_p3583036195916"></a>全选或者取消全选</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127936423_p258317365591"><a name="zh-cn_topic_0127936423_p258317365591"></a><a name="zh-cn_topic_0127936423_p258317365591"></a>可通过<a name="zh-cn_topic_0127936423_image536513147519"></a><a name="zh-cn_topic_0127936423_image536513147519"></a><span><img id="zh-cn_topic_0127936423_image536513147519" src="figures/zh-cn_image_0129033244.png"></span>全选APP管理表中行，通过<a name="zh-cn_topic_0127936423_image1251516262073"></a><a name="zh-cn_topic_0127936423_image1251516262073"></a><span><img id="zh-cn_topic_0127936423_image1251516262073" src="figures/zh-cn_image_0129033247.png" width="20.9475" height="20.045627"></span>可取消全选。</p>
</td>
</tr>
<tr id="zh-cn_topic_0127936423_row019992094812"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127936423_p205831436115916"><a name="zh-cn_topic_0127936423_p205831436115916"></a><a name="zh-cn_topic_0127936423_p205831436115916"></a>跳转到拓扑界面</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127936423_p1167075833016"><a name="zh-cn_topic_0127936423_p1167075833016"></a><a name="zh-cn_topic_0127936423_p1167075833016"></a>单击列表右侧的动作列单击<a name="zh-cn_topic_0127936423_image194232024181112"></a><a name="zh-cn_topic_0127936423_image194232024181112"></a><span><img id="zh-cn_topic_0127936423_image194232024181112" src="figures/zh-cn_image_0129033250.png"></span>按钮，可跳转到Mobile拓扑界面详细查看调用过程。</p>
</td>
</tr>
<tr id="zh-cn_topic_0127936423_row185831236125917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127936423_p1358333615919"><a name="zh-cn_topic_0127936423_p1358333615919"></a><a name="zh-cn_topic_0127936423_p1358333615919"></a>跳转到APP汇总界面</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127936423_p2317132418122"><a name="zh-cn_topic_0127936423_p2317132418122"></a><a name="zh-cn_topic_0127936423_p2317132418122"></a>单击列表右侧的动作列单击<a name="zh-cn_topic_0127936423_image1762782117139"></a><a name="zh-cn_topic_0127936423_image1762782117139"></a><span><img id="zh-cn_topic_0127936423_image1762782117139" src="figures/zh-cn_image_0129033253.png"></span>按钮，可跳转到APP汇总界面，查看用户体验详情。</p>
</td>
</tr>
</tbody>
</table>

