# 安装ICAgent<a name="ZH-CN_TOPIC_0127215848"></a>

ICAgent状态说明详见下表。

**表 1**  ICAgent状态

<a name="table178415320113"></a>
<table><thead align="left"><tr id="row87841335115"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p278081612119"><a name="p278081612119"></a><a name="p278081612119"></a>状态</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p67814168111"><a name="p67814168111"></a><a name="p67814168111"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row187841321112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p978513162111"><a name="p978513162111"></a><a name="p978513162111"></a>运行</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p978610163116"><a name="p978610163116"></a><a name="p978610163116"></a>该主机ICAgent运行正常。</p>
</td>
</tr>
<tr id="row1778473101115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p87882016101117"><a name="p87882016101117"></a><a name="p87882016101117"></a>未安装</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p2788216121111"><a name="p2788216121111"></a><a name="p2788216121111"></a>该主机未安装ICAgent。安装ICAgent，详细操作请参见<a href="安装ICAgent.md">安装ICAgent</a>。</p>
</td>
</tr>
<tr id="row378483181120"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p179091619119"><a name="p179091619119"></a><a name="p179091619119"></a>安装中</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p137925167113"><a name="p137925167113"></a><a name="p137925167113"></a>正在为该主机安装ICAgent。安装ICAgent预计需要1分钟左右，请耐心等待。</p>
</td>
</tr>
<tr id="row167841334116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p87941616161112"><a name="p87941616161112"></a><a name="p87941616161112"></a>安装失败</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p167951316191119"><a name="p167951316191119"></a><a name="p167951316191119"></a>该主机ICAgent安装失败，请<a href="卸载ICAgent.md#section1218782615374">登录服务器卸载</a>后重新安装。</p>
</td>
</tr>
<tr id="row87841031113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p13798181641119"><a name="p13798181641119"></a><a name="p13798181641119"></a>升级中</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p17997166114"><a name="p17997166114"></a><a name="p17997166114"></a>正在升级该主机ICAgent。升级ICAgent预计需要1分钟左右，请耐心等待。</p>
</td>
</tr>
<tr id="row5784535116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p280014165112"><a name="p280014165112"></a><a name="p280014165112"></a>升级失败</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13801101641119"><a name="p13801101641119"></a><a name="p13801101641119"></a>该主机ICAgent升级失败。请<a href="卸载ICAgent.md#section1218782615374">登录服务器卸载</a>后重新安装。</p>
</td>
</tr>
<tr id="row1491511151116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p15802191631117"><a name="p15802191631117"></a><a name="p15802191631117"></a>离线</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1580381610114"><a name="p1580381610114"></a><a name="p1580381610114"></a>由于网络问题导致该主机ICAgent功能异常。请检查并恢复网络。</p>
</td>
</tr>
<tr id="row1191311171114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1380461681118"><a name="p1380461681118"></a><a name="p1380461681118"></a>异常</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p108041216131119"><a name="p108041216131119"></a><a name="p108041216131119"></a>该主机ICAgent功能异常，请联系人工客服处理。</p>
</td>
</tr>
</tbody>
</table>

## 安装前提<a name="zh-cn_topic_0089684077_section789175015231"></a>

在进行ICAgent安装前，需要先确保本地浏览器时间与服务器时区、时间都一致。若有多个服务器，则要保证本地浏览器、多个服务器的时区、时间都一致。否则，可能会导致安装后不能在界面上准确查看应用、服务器的指标数据。

## 安装方式说明<a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_section154003208582"></a>

ICAgent有两种安装方式，您可以按照您的场景进行选择。您需要注意的是，下述两种安装方式，都不适用于容器节点（通过ServiceStage、AOS、CCE创建的集群容器节点）。容器节点不需要手动安装ICAgent，只需要在创建集群或部署应用时进行操作，详见[快速入门](https://support.huaweicloud.com/qs-aom/aom_00_0001.html)。

安装方式见[表2](#zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_table5921281716319)：

**表 2**  安装方式

<a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_table5921281716319"></a>
<table><thead align="left"><tr id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_row4088670316319"><th class="cellrowborder" valign="top" width="20.3%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p1007152116319"><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p1007152116319"></a><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p1007152116319"></a>方式</p>
</th>
<th class="cellrowborder" valign="top" width="79.7%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p1048688816319"><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p1048688816319"></a><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p1048688816319"></a>适用场景</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_row6164033616319"><td class="cellrowborder" valign="top" width="20.3%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p2681132116319"><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p2681132116319"></a><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p2681132116319"></a>首次安装</p>
</td>
<td class="cellrowborder" valign="top" width="79.7%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p2423342716319"><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p2423342716319"></a><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p2423342716319"></a>当满足以下条件时，您需要按照该方式安装：</p>
<a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_ol240967611653"></a><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_ol240967611653"></a><ol id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_ol240967611653"><li>服务器已经绑定了EIP。绑定EIP的详细操作请参见<a href="http://support.huaweicloud.com/usermanual-vpc/zh-cn_topic_0013748738.html" target="_blank" rel="noopener noreferrer">为弹性云服务器申请和绑定弹性IP</a>。</li><li>该服务器上未安装过ICAgent。</li></ol>
</td>
</tr>
<tr id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_row1653765616319"><td class="cellrowborder" valign="top" width="20.3%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p6448173016319"><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p6448173016319"></a><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p6448173016319"></a>继承安装</p>
</td>
<td class="cellrowborder" valign="top" width="79.7%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p5563762416319"><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p5563762416319"></a><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p5563762416319"></a>当满足以下条件时，您需要按照该方式安装：</p>
<p id="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p28718779182051"><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p28718779182051"></a><a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582509_p28718779182051"></a>您有多个服务器需要安装ICAgent，其中一个服务器绑定了EIP，而剩余的没有绑定EIP。其中一个服务器已经通过首次安装方式装好了ICAgent，对于没有绑定EIP的服务器，您可以采用该安装方式。</p>
</td>
</tr>
</tbody>
</table>

## 首次安装<a name="section689913619366"></a>

您在华为云上申请服务器后，首次安装ICAgent，需执行如下操作：

1.  获取AK/SK。
    -   若您已在华为云获取过AK/SK，请跳过该步骤。
    -   若您未在华为云获取过AK/SK，请参考[如何获取AK/SK和projectid值](http://support.huaweicloud.com/apm_faq/apm_03_0001.html)章节获取AK/SK。

2.  登录[应用运维管理](https://console.huaweicloud.com/aom/#/aom/ams/summary)。
3.  在左侧导航栏中选择“采集器部署 \> Agent管理”。
4.  单击“安装ICAgent”。
5.  生成ICAgent安装命令，并复制该命令。
    1.  在文本框中输入已获取的AK/SK，生成ICAgent安装命令。

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >请确保以上参数输入正确，否则将无法安装ICAgent。  

    2.  <a name="zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582074_li1462214222118"></a>单击“复制命令”。

        ![](figures/安装ICAgent.png)


6.  使用PuTTY等远程登录工具，以root用户登录待安装ICAgent的服务器，执行[步骤5.b](#zh-cn_topic_0089684077_zh-cn_topic_0089582074_zh-cn_topic_0089684077_zh-cn_topic_0089582074_li1462214222118)复制到的安装命令进行安装。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   当显示“ICAgent install success”时，表示安装成功，ICAgent已安装在了/opt/oss/servicemgr/目录。安装成功后，在应用运维管理左侧导航栏中选择“采集器部署 \> Agent管理”，查看该服务器ICAgent状态。  
    >-   安装失败，请参考卸载ICAgent章节的[登录服务器卸载](卸载ICAgent.md#section1218782615374)后重新安装，如果还未安装成功，请联系华为技术工程师。  


## 继承安装<a name="section490015619361"></a>

当用户已有服务器安装过ICAgent，且该服务器“/opt/ICAgent/“路径下ICAgent安装包**ICProbeAgent.zip**存在，通过该方式可对远端服务器进行一键式继承安装。

1.  在已安装ICAgent的服务器上执行如下命令，其中_x.x.x.x_表示服务器IP地址。

    **bash /opt/oss/servicemgr/ICAgent/bin/remoteInstall/remote\_install.sh -ip** **x.x.x.x**

2.  根据提示输入待安装ICAgent的服务器root用户密码。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   如果已安装ICAgent的服务器安装过expect工具，执行上述命令后，即可完成安装。如果已安装ICAgent的服务器未安装expect工具，请根据提示输入，进行安装。  
    >-   请确保已安装ICAgent的服务器可以使用root用户执行SSH、SCP命令，来与待安装ICAgent的服务器进行远端通信。  
    >-   当显示“ICAgent install success”时，表示安装成功，ICAgent已安装在了/opt/oss/servicemgr/目录。安装成功后，在应用运维管理左侧导航栏中选择“采集器部署 \> Agent管理”，查看该服务器ICAgent状态。  
    >-   安装失败，请参考卸载ICAgent章节的[登录服务器卸载](卸载ICAgent.md#section1218782615374)后重新安装，如果还未安装成功，请联系华为技术工程师。  


## 继承批量安装<a name="section844164283613"></a>

当您已有服务器安装过ICAgent，且该服务器“/opt/ICAgent/”路径下ICAgent安装包**ICProbeAgent.zip**存在，通过该方式可对多个远端服务器进行一键式继承批量安装。

>![](public_sys-resources/icon-notice.gif) **注意：**   
>批量安装的ECS需同属一个VPC下，并在同一个网段中。  

**前提条件**

已收集需要安装Agent的所有虚拟机IP、密码，按照iplist.cfg格式整理好，并上传到已安装过ICAgent机器的/opt/ICAgent/目录下。iplist.cfg格式示例如下所示，IP与密码之间用空格隔开：

_192.168.0.109 密码（请根据实际填写）_

_192.168.0.39 密码（请根据实际填写）_

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   iplist.cfg中包含您的敏感信息，建议您使用完之后清理一下。  
>-   如果所有弹性云服务器的密码一致，iplist.cfg中只需列出IP，无需填写密码，在执行时输入此密码即可；如果某个IP密码与其他不一致，则需在此IP后填写其密码。  

**操作步骤**

1.  在已安装ICAgent的服务器上执行如下命令。

    **bash /opt/oss/servicemgr/ICAgent/bin/remoteInstall/remote\_install.sh -batchModeConfig /opt/ICAgent/iplist.cfg**

    根据脚本提示输入待安装机器的root用户默认密码，如果所有IP的密码在iplist.cfg中已有配置，则直接输入回车键跳过即可，否则请输入默认密码。

    ```
    batch install begin
    Please input default passwd:
    send cmd to 192.168.0.109
    send cmd to 192.168.0.39
    2 tasks running, please wait...
    2 tasks running, please wait...
    2 tasks running, please wait...
    End of install agent: 192.168.0.39
    End of install agent: 192.168.0.109
    All hosts install icagent finish.
    ```

    请耐心等待，当提示All hosts install icagent finish.时，则表示配置文件中的所有主机安装操作已完成。

2.  安装完成后，在应用性能管理左侧导航栏中选择“采集器部署 \> Agent管理”，查看该服务器ICAgent状态。

