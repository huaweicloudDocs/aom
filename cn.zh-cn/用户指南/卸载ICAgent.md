# 卸载ICAgent<a name="ZH-CN_TOPIC_0127215850"></a>

服务器上的ICAgent被卸载后，会影响该服务器的运维能力，导致AOM功能不可用，请谨慎操作！

卸载方式，您可以按照需要进行选择：

-   [通过界面卸载](#section13185626133716)：此操作适用于正常安装ICAgent后需卸载的场景。
-   [登录服务器卸载](#section1218782615374)：此操作适用于未成功安装ICAgent需卸载重装的场景。
-   [远程卸载](#section76581424194316)：此操作适用于正常安装ICAgent后需远程卸载的场景。
-   [批量卸载](#section19497111135712)：此操作适用于正常安装ICAgent后需批量卸载的场景。

## 通过界面卸载<a name="section13185626133716"></a>

1.  登录[应用运维管理](https://console.huaweicloud.com/aom/#/aom/ams/summary)。
2.  在左侧导航栏中选择“采集器部署 \> Agent管理”。
3.  在页面右侧的下拉列表框中选择“其他: 用户自定义接入主机”。
4.  在ICAgent列表中选中一个或多个待卸载ICAgent的服务器前的复选框，单击“卸载ICAgent”。在“卸载ICAgent”对话框中单击“确定”。

    ICAgent开始卸载，卸载ICAgent预计需要1分钟左右，请耐心等待。待ICAgent的状态由“卸载中”变为“未安装”时，表示卸载成功。


## 登录服务器卸载<a name="section1218782615374"></a>

1.  以**root**用户登录需卸载ICAgent的服务器。
2.  执行如下命令卸载ICAgent。

    **bash /opt/oss/servicemgr/ICAgent/bin/manual/uninstall.sh;**

3.  当显示“ICAgent uninstall success”时，表示卸载成功。

## 远程卸载<a name="section76581424194316"></a>

除了上述登录服务器上执行uninstall.sh脚本卸载ICAgent的方式，还有类似[继承安装](安装ICAgent.md#section490015619361)的方式对主机进行远程卸载。

1.  在已安装ICAgent的服务器上执行如下命令，其中_x.x.x.x_表示服务器IP地址。

    **bash /opt/oss/servicemgr/ICAgent/bin/**remoteUninstall**/remote\_uninstall.sh -ip x.x.x.x**

2.  根据提示输入待卸载ICAgent的服务器root用户密码。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   如果已安装ICAgent的服务器安装过expect工具，执行上述命令后，即可完成卸载。如果已安装ICAgent的服务器未安装expect工具，请根据提示输入，进行卸载。  
    >-   请确保已安装ICAgent的服务器可以使用root用户执行SSH、SCP命令，来与待卸载ICAgent的服务器进行远端通信。  
    >-   当显示“ICAgent uninstall success”时，表示卸载成功。 卸载完成后，可在应用性能管理左侧导航栏中选择“采集器部署 \> Agent管理”，查看该服务器ICAgent状态。  


## 批量卸载<a name="section19497111135712"></a>

当您已有服务器安装过ICAgent，且该服务器“/opt/ICAgent/”路径下ICAgent安装包**ICProbeAgent.tar.gz**存在，通过该方式可对多个远端服务器进行一键式继承批量卸载。

>![](public_sys-resources/icon-notice.gif) **注意：**   
>批量卸载的ECS需同属一个VPC下，并在同一个网段中。  

**前提条件**

已收集需要卸载Agent的所有虚拟机IP、密码，按照iplist.cfg格式整理好，并上传到已安装过ICAgent机器的/opt/ICAgent/目录下。iplist.cfg格式示例如下所示，IP与密码之间用空格隔开：

_192.168.0.109 密码（请根据实际填写）_

_192.168.0.39 密码（请根据实际填写）_

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   iplist.cfg中包含您的敏感信息，建议您使用完之后清理一下。  
>-   如果所有弹性云服务器的密码一致，iplist.cfg中只需列出IP，无需填写密码，在执行时输入此密码即可；如果某个IP密码与其他不一致，则需在此IP后填写其密码。  

**操作步骤**

1.  在已安装ICAgent的服务器上执行如下命令。

    **bash /opt/oss/servicemgr/ICAgent/bin/remoteUninstall/remote\_uninstall.sh -batchModeConfig /opt/ICAgent/iplist.cfg**

    根据脚本提示输入待卸载机器的root用户默认密码，如果所有IP的密码在iplist.cfg中已有配置，则直接输入回车键跳过即可，否则请输入默认密码。

    ```
    batch uninstall begin
    Please input default passwd:
    send cmd to 192.168.0.109
    send cmd to 192.168.0.39
    2 tasks running, please wait...
    End of uninstall agent: 192.168.0.109
    End of uninstall agent: 192.168.0.39
    All hosts uninstall icagent finish.
    ```

    请耐心等待，当提示All hosts uninstall icagent finish.时，则表示配置文件中的所有主机卸载操作已完成。

2.  卸载完成后，在应用性能管理左侧导航栏中选择“采集器部署 \> Agent管理”，查看该服务器ICAgent状态。

