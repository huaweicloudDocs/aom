# 安装ICAgent<a name="aom_02_0012"></a>

ICAgent用于采集指标、日志和应用性能数据。对于在ECS、BMS控制台直接购买的主机，您需手动安装ICAgent。对于通过CCE间接购买的主机，ICAgent会自动安装。

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
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p108041216131119"><a name="p108041216131119"></a><a name="p108041216131119"></a>该主机ICAgent功能异常，请联系技术人员处理。</p>
</td>
</tr>
</tbody>
</table>

## 安装前提<a name="s09e4ef44770c48209617bb793bb12e54"></a>

在进行ICAgent安装前，需要先确保本地浏览器时间与服务器时区、时间都一致。若有多个服务器，则要保证本地浏览器、多个服务器的时区、时间都一致。否则，可能会导致安装后不能在界面上准确查看应用、服务器的指标数据。

## 安装方式说明<a name="s2b4c9d68297049329fe7cdd4885fbfc0"></a>

ICAgent有两种安装方式，您可以按照您的场景进行选择。您需要注意的是，下述两种安装方式，都不适用于容器节点（通过ServiceStage、CCE创建的集群容器节点）。容器节点不需要手动安装ICAgent，只需要在创建集群或部署应用时进行操作。

安装方式见[表2](#td567fa2f6ccc421ca2e6a4b8a51ee8c6)：

**表 2**  安装方式

<a name="td567fa2f6ccc421ca2e6a4b8a51ee8c6"></a>
<table><thead align="left"><tr id="r7097d3d7ea6f44f6834079532fb878e9"><th class="cellrowborder" valign="top" width="20.3%" id="mcps1.2.3.1.1"><p id="a00543c221a544b7b88f63298f371e936"><a name="a00543c221a544b7b88f63298f371e936"></a><a name="a00543c221a544b7b88f63298f371e936"></a>方式</p>
</th>
<th class="cellrowborder" valign="top" width="79.7%" id="mcps1.2.3.1.2"><p id="ab21f48108a7f4e81842d0a30b53bb26f"><a name="ab21f48108a7f4e81842d0a30b53bb26f"></a><a name="ab21f48108a7f4e81842d0a30b53bb26f"></a>适用场景</p>
</th>
</tr>
</thead>
<tbody><tr id="r6003a646dec346d89ba0fb71bfb4c36c"><td class="cellrowborder" valign="top" width="20.3%" headers="mcps1.2.3.1.1 "><p id="a49db8f5a625b43e7a3d42c015767db75"><a name="a49db8f5a625b43e7a3d42c015767db75"></a><a name="a49db8f5a625b43e7a3d42c015767db75"></a>首次安装</p>
</td>
<td class="cellrowborder" valign="top" width="79.7%" headers="mcps1.2.3.1.2 "><p id="acfeeec445cba4229985b849a069c2f82"><a name="acfeeec445cba4229985b849a069c2f82"></a><a name="acfeeec445cba4229985b849a069c2f82"></a>当满足以下条件时，您需要按照该方式安装：</p>
<a name="o6d4dabb4e6e34e0eb034e404138f221c"></a><a name="o6d4dabb4e6e34e0eb034e404138f221c"></a><ol id="o6d4dabb4e6e34e0eb034e404138f221c"><li>服务器已经绑定了EIP。</li><li>该服务器上未安装过ICAgent。</li></ol>
</td>
</tr>
<tr id="rfc682cc73dd24a7e98bd1f20fd46a24e"><td class="cellrowborder" valign="top" width="20.3%" headers="mcps1.2.3.1.1 "><p id="abb2d78de36dc42e3bc0507c474b40bd8"><a name="abb2d78de36dc42e3bc0507c474b40bd8"></a><a name="abb2d78de36dc42e3bc0507c474b40bd8"></a>继承安装</p>
</td>
<td class="cellrowborder" valign="top" width="79.7%" headers="mcps1.2.3.1.2 "><p id="ab9ed7f2f42d142dab2391213ac17681e"><a name="ab9ed7f2f42d142dab2391213ac17681e"></a><a name="ab9ed7f2f42d142dab2391213ac17681e"></a>当满足以下条件时，您需要按照该方式安装：</p>
<p id="a66d8b62db3e140d7adb0d0016eb24896"><a name="a66d8b62db3e140d7adb0d0016eb24896"></a><a name="a66d8b62db3e140d7adb0d0016eb24896"></a>您有多个服务器需要安装ICAgent，其中一个服务器绑定了EIP，而剩余的没有绑定EIP。其中一个服务器已经通过首次安装方式装好了ICAgent，对于没有绑定EIP的服务器，您可以采用该安装方式。</p>
</td>
</tr>
</tbody>
</table>

## 首次安装<a name="section689913619366"></a>

您申请服务器后，首次安装ICAgent，需执行如下操作：

1.  获取AK/SK。
    -   若您已获取过AK/SK，请跳过该步骤。
    -   若您未获取过AK/SK，请获取AK/SK。

2.  在左侧导航栏中选择“配置管理 \> Agent管理”。
3.  选择“其他: 用户自定义接入主机”，单击“安装ICAgent”，选择“主机类型”为“华为云主机”。
4.  （可选）为了避免泄露您的AK/SK，请勾选下图所示的复选框，执行关闭历史记录命令。

    ![](figures/zh-cn_image_0000001133528241.png)

5.  生成ICAgent安装命令，复制并执行该命令进行安装。
6.  安装完成后，执行以下命令，开启历史记录。

    **set -o history**

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >-   当显示“ICAgent install success”时，表示安装成功，ICAgent已安装在了/opt/oss/servicemgr/目录。安装成功后，在应用运维管理左侧导航栏中选择“配置管理 \> Agent管理”，查看该服务器ICAgent状态。
    >-   安装失败，请参考卸载ICAgent章节的[登录服务器卸载](卸载ICAgent.md#section1218782615374)后重新安装，如果还未安装成功，请联系技术工程师。


## 继承安装<a name="section490015619361"></a>

当用户已有服务器安装过ICAgent，且该服务器“/opt/ICAgent/“路径下ICAgent安装包**ICProbeAgent.zip**存在，通过该方式可对远端服务器进行一键式继承安装。

1.  在已安装ICAgent的服务器上执行如下命令，其中_x.x.x.x_表示服务器IP地址。

    **bash /opt/oss/servicemgr/ICAgent/bin/remoteInstall/remote\_install.sh -ip** **x.x.x.x**

2.  根据提示输入待安装ICAgent的服务器root用户密码。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >-   如果已安装ICAgent的服务器安装过expect工具，执行上述命令后，即可完成安装。如果已安装ICAgent的服务器未安装expect工具，请根据提示输入，进行安装。
    >-   请确保已安装ICAgent的服务器可以使用root用户执行SSH、SCP命令，来与待安装ICAgent的服务器进行远端通信。
    >-   当显示“ICAgent install success”时，表示安装成功，ICAgent已安装在了/opt/oss/servicemgr/目录。安装成功后，在应用运维管理左侧导航栏中选择“配置管理 \> Agent管理”，查看该服务器ICAgent状态。
    >-   安装失败，请参考卸载ICAgent章节的[登录服务器卸载](卸载ICAgent.md#section1218782615374)后重新安装，如果还未安装成功，请联系技术工程师。


## 继承批量安装<a name="section844164283613"></a>

当您已有服务器安装过ICAgent，且该服务器“/opt/ICAgent/”路径下ICAgent安装包**ICProbeAgent.zip**存在，通过该方式可对多个远端服务器进行一键式继承批量安装。

>![](public_sys-resources/icon-notice.gif) **须知：** 
>1.  批量安装的ECS需和已安装成功的节点保持网络互通，scp、ssh命令可用。
>2.  如果已安装的服务器使用了委托方式安装，其它批量安装的节点也需要设置委托。
>3.  批量安装脚本依赖python版本，建议在python2.x版本的机器上执行此操作，python3.x版本不支持。
>4.  iplist.cfg文件中每一行应以回车作为结尾。

**前提条件**

已收集需要安装Agent的所有虚拟机IP、密码，按照iplist.cfg格式整理好，并上传到已安装过ICAgent机器的/opt/ICAgent/目录下。iplist.cfg格式示例如下所示，IP与密码之间用空格隔开：

_192.168.0.109 密码（请根据实际填写）_

_192.168.0.39 密码（请根据实际填写）_

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   iplist.cfg中包含您的敏感信息，建议您使用完之后清理一下。
>-   如果所有弹性云服务器的密码一致，iplist.cfg中只需列出IP，无需填写密码，在执行时输入此密码即可；如果某个IP密码与其他不一致，则需在此IP后填写其密码。
>-   批量安装功能依赖python2.7.\*版本，如果安装时提示找不到python请安装python版本后重试。

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

2.  安装完成后，在应用运维管理左侧导航栏中选择“配置管理 \> Agent管理”，查看该服务器ICAgent状态。

