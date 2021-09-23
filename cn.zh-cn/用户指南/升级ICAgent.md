# 升级ICAgent<a name="aom_02_0013"></a>

为了更好的采集体验，AOM会不断更新ICAgent版本。当系统提示您有新的ICAgent版本时，您可以按照如下操作步骤进行升级。

>![](public_sys-resources/icon-note.gif) **说明：** 
>如果ICAgent存在严重的bug时，系统会对采集的版本进行升级。

1.  在左侧导航栏中选择“配置管理 \> Agent管理”。
2.  <a name="lf53afe92b28749b8be5a3ee0491c691a"></a>在页面右侧的下拉列表框中选择“集群：xxx”或“其他：用户自定义接入主机”。
3.  升级ICAgent。如果在[步骤2](#lf53afe92b28749b8be5a3ee0491c691a)中下拉列表框中选择的是“集群：xxx”，则单击“升级ICAgent”。可实现整个集群的升级操作，即在ICAgent列表下的所有主机一次性完成升级。如果在[步骤2](#lf53afe92b28749b8be5a3ee0491c691a)中下拉列表框中选择的是“其他：用户自定义接入主机”，则先选择主机后单击“升级ICAgent”。
4.  ICAgent开始升级，升级ICAgent预计需要1分钟左右，请耐心等待。待ICAgent的状态由“升级中”变为“运行”时，表示升级成功。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果升级后，界面显示ICAgent状态异常或者其它升级失败场景，请直接登录节点使用安装命令重新安装ICAgent即可（覆盖式安装，无需卸载操作）。


