# 卸载ICAgent<a name="aom_02_0096"></a>

服务器上的ICAgent被卸载后，会影响该服务器的运维能力，导致拓扑、调用链等功能不可用，请谨慎操作！

-   [通过界面卸载](#zh-cn_topic_0173929605_section6443113288)：此操作适用于正常安装ICAgent后需卸载的场景。
-   [登录服务器卸载](#zh-cn_topic_0173929605_section24710112816)：此操作适用于未成功安装ICAgent需卸载重装的场景。

## 通过界面卸载<a name="zh-cn_topic_0173929605_section6443113288"></a>

1.  登录AOM控制台，在左侧导航栏中选择“采集器部署 \> Agent管理”。
2.  在页面右侧的下拉列表框中选择“其他: 用户自定义接入主机”。
3.  在ICAgent列表中选中一个或多个待卸载ICAgent的服务器前的复选框，单击“卸载ICAgent”。在“卸载ICAgent”对话框中单击“确定”。

    ICAgent开始卸载，卸载ICAgent预计需要1分钟左右，请耐心等待。待ICAgent的状态由“卸载中”变为“未安装”时，表示卸载成功。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >通过界面卸载ICAgent后如果需要再次安装，请等待5分钟后执行安装操作，否则可能出现被再次自动卸载的情况。  


## 登录服务器卸载<a name="zh-cn_topic_0173929605_section24710112816"></a>

1.  以**root**用户登录需卸载ICAgent的服务器。
2.  执行如下命令卸载ICAgent。

    **bash /opt/oss/servicemgr/ICAgent/bin/manual/uninstall.sh;**

3.  当显示“ICAgent uninstall success”时，表示卸载成功。

