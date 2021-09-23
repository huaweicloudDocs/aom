# 安装ICAgent（华为云主机）<a name="aom_02_002301"></a>

ICAgent用于采集指标、日志和应用性能数据。对于在ECS、BMS控制台直接购买的主机，您需手动安装ICAgent。对于通过CCE间接购买的主机，ICAgent会自动安装，您不用安装ICAgent。

## 安装前提<a name="s09e4ef44770c48209617bb793bb12e54"></a>

-   在进行ICAgent安装前，需要先确保本地浏览器时间与服务器时区、时间都一致。若有多个服务器，则要保证本地浏览器、多个服务器的时区、时间都一致。否则，可能会导致安装后不能在界面上准确查看应用、服务器的指标数据。
-   ICAgent进程需要root用户安装和运行。

## 安装方式说明<a name="s2b4c9d68297049329fe7cdd4885fbfc0"></a>

ICAgent有两种安装方式，您可以按照您的场景进行选择。您需要注意的是，下述两种安装方式，都不适用于容器节点（通过ServiceStage、CCE创建的集群容器节点）。容器节点不需要手动安装ICAgent，只需要在创建集群或部署应用时进行操作。

安装方式见[表1](#td567fa2f6ccc421ca2e6a4b8a51ee8c6)：

**表 1**  安装方式

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
<p id="p1542611457013"><a name="p1542611457013"></a><a name="p1542611457013"></a>请参考<a href="安装ICAgent.md#section490015619361">继承安装</a>。</p>
</td>
</tr>
</tbody>
</table>

## 首次安装<a name="section12550163711538"></a>

您申请服务器后，首次安装ICAgent，需执行如下操作：

1.  获取AK/SK。
    -   若您已获取过AK/SK，请跳过该步骤。
    -   若您未获取过AK/SK，请获取AK/SK。

2.  在左侧导航栏中选择“配置管理 \> Agent管理”。
3.  单击“安装ICAgent”。
4.  （可选）为了避免泄露您的AK/SK，请勾选下图所示的复选框，执行关闭历史记录命令。

    ![](figures/zh-cn_image_0000001086353480.png)

5.  生成ICAgent安装命令，复制并执行该命令进行安装。
6.  安装完成后，执行以下命令，开启历史记录。

    **_set -o history_**

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >-   当显示“ICAgent install success”时，表示安装成功，ICAgent已安装在了/opt/oss/servicemgr/目录。安装成功后，在应用运维管理左侧导航栏中选择“配置管理 \> Agent管理”，查看该服务器ICAgent状态。
    >-   安装失败，请参考卸载ICAgent章节的[登录服务器卸载](卸载ICAgent.md#section1218782615374)后重新安装，如果还未安装成功，请联系技术工程师。


## 后续操作<a name="section11142226119"></a>

更多安装方式及升级、卸载ICAgent请参考[Agent管理（华为云主机）](Agent管理（华为云主机）.md)。

