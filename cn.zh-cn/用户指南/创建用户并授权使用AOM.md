# 创建用户并授权使用AOM<a name="aom_02_0090"></a>

如果您需要对您所拥有的AOM进行精细的权限管理，您可以使用统一身份认证服务（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为云账号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用AOM资源。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将AOM资源委托给更专业、高效的其他华为云账号或者云服务，这些账号或者云服务可以根据权限进行代运维。

如果华为云账号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用AOM服务的其它功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#zh-cn_topic_0169701339_fig13279111625016)所示。

## 前提条件<a name="zh-cn_topic_0169701339_section18761381264"></a>

给用户组授权之前，请您了解用户组可以添加的AOM权限，并结合实际需求进行选择，AOM支持的系统权限，请参见[AOM系统权限](https://support.huaweicloud.com/productdesc-aom/aom_06_0021.html)。若您需要对除AOM之外的其他服务授权，IAM支持服务的所有系统权限请参见[系统权限](https://support.huaweicloud.com/usermanual-permissions/iam_01_0001.html)。

## 示例流程<a name="zh-cn_topic_0169701339_section346220507231"></a>

**图 1**  给用户授权AOM权限流程<a name="zh-cn_topic_0169701339_fig13279111625016"></a>  
![](figures/给用户授权AOM权限流程.png "给用户授权AOM权限流程")

1.  <a name="zh-cn_topic_0169701339_li11838175082320"></a>[创建用户组并授权](https://support.huaweicloud.com/usermanual-iam/iam_03_0001.html)

    在IAM控制台创建用户组，并授予AOM只读权限“AOM ReadOnlyAccess”。

2.  [创建用户并加入用户组](https://support.huaweicloud.com/usermanual-iam/iam_02_0001.html)

    在IAM控制台创建用户，并将其加入[1](#zh-cn_topic_0169701339_li11838175082320)中创建的用户组。

3.  [用户登录](https://support.huaweicloud.com/usermanual-iam/iam_01_0552.html)并验证权限

    新创建的用户登录控制台，验证AOM的只读权限。


