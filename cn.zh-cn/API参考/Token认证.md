# Token认证<a name="ZH-CN_TOPIC_0096010437"></a>

## 应用场景<a name="zh-cn_topic_0095238317_zh-cn_topic_0024478020_section5608799912249"></a>

当您使用Token认证方式完成认证鉴权时，需要获取用户Token并在调用接口时增加“X-Auth-Token”到业务接口请求消息头中。

本节介绍如何调用接口完成Token认证。如何获取Token值，请参考“[获取用户Token](http://support.huaweicloud.com/api-iam/zh-cn_topic_0057845583.html)”

## 调用接口步骤<a name="zh-cn_topic_0095238317_zh-cn_topic_0024478020_section3546598312249"></a>

1.  发送“POST https://_**IAM的Endpoint**_/v3/auth/tokens”，获取IAM的Endpoint及消息体中的区域名称，请参考[表1](#table611425921310)。

    **表 1**  IAM的Endpoint

    <a name="table611425921310"></a>
    <table><thead align="left"><tr id="row1011585971313"><th class="cellrowborder" valign="top" width="12%" id="mcps1.2.6.1.1"><p id="p153091771512"><a name="p153091771512"></a><a name="p153091771512"></a>服务名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.2.6.1.2"><p id="p1568524404210"><a name="p1568524404210"></a><a name="p1568524404210"></a>区域名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.2.6.1.3"><p id="p203063717153"><a name="p203063717153"></a><a name="p203063717153"></a>区域</p>
    </th>
    <th class="cellrowborder" valign="top" width="36%" id="mcps1.2.6.1.4"><p id="p4305157131510"><a name="p4305157131510"></a><a name="p4305157131510"></a>终端节点（Endpoint）</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.2.6.1.5"><p id="p152828731515"><a name="p152828731515"></a><a name="p152828731515"></a>协议类型</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row811575991315"><td class="cellrowborder" rowspan="6" valign="top" width="12%" headers="mcps1.2.6.1.1 "><p id="p9251144117142"><a name="p9251144117142"></a><a name="p9251144117142"></a>IAM</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.2 "><p id="p67501959114019"><a name="p67501959114019"></a><a name="p67501959114019"></a>华北-北京一</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.6.1.3 "><p id="p17750165920402"><a name="p17750165920402"></a><a name="p17750165920402"></a>cn-north-1</p>
    </td>
    <td class="cellrowborder" valign="top" width="36%" headers="mcps1.2.6.1.4 "><p id="p107503591405"><a name="p107503591405"></a><a name="p107503591405"></a>iam.cn-north-1.myhuaweicloud.com</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.5 "><p id="p3751165910407"><a name="p3751165910407"></a><a name="p3751165910407"></a>HTTPS</p>
    </td>
    </tr>
    <tr id="row73534483131"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p1775105914405"><a name="p1775105914405"></a><a name="p1775105914405"></a>华东-上海二</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p107511359104010"><a name="p107511359104010"></a><a name="p107511359104010"></a>cn-east-2</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p1075125913401"><a name="p1075125913401"></a><a name="p1075125913401"></a>iam.cn-east-2.myhuaweicloud.com</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.4 "><p id="p275165911404"><a name="p275165911404"></a><a name="p275165911404"></a>HTTPS</p>
    </td>
    </tr>
    <tr id="row575175310138"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p27511459104010"><a name="p27511459104010"></a><a name="p27511459104010"></a>华南-广州</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p1575195919407"><a name="p1575195919407"></a><a name="p1575195919407"></a>cn-south-1</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p1375195984014"><a name="p1375195984014"></a><a name="p1375195984014"></a>iam.cn-south-1.myhuaweicloud.com</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.4 "><p id="p1475175914409"><a name="p1475175914409"></a><a name="p1475175914409"></a>HTTPS</p>
    </td>
    </tr>
    <tr id="row138141254195912"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p175175934019"><a name="p175175934019"></a><a name="p175175934019"></a>东北-大连</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p57514590405"><a name="p57514590405"></a><a name="p57514590405"></a>cn-northeast-1</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p20751125994017"><a name="p20751125994017"></a><a name="p20751125994017"></a>iam.cn-northeast-1.myhuaweicloud.com</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.4 "><p id="p13751959184016"><a name="p13751959184016"></a><a name="p13751959184016"></a>HTTPS</p>
    </td>
    </tr>
    <tr id="row359052854016"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p1475116599400"><a name="p1475116599400"></a><a name="p1475116599400"></a>所有</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p19751459194011"><a name="p19751459194011"></a><a name="p19751459194011"></a>ALL</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p2751195914407"><a name="p2751195914407"></a><a name="p2751195914407"></a>iam.myhuaweicloud.com</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.4 "><p id="p12752175918405"><a name="p12752175918405"></a><a name="p12752175918405"></a>HTTPS</p>
    </td>
    </tr>
    <tr id="row1194272119012"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p0752259114011"><a name="p0752259114011"></a><a name="p0752259114011"></a>亚太-香港</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p11752759104016"><a name="p11752759104016"></a><a name="p11752759104016"></a>ap-southeast-1</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p1175225974016"><a name="p1175225974016"></a><a name="p1175225974016"></a>iam.ap-southeast-1.myhwclouds.com</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.6.1.4 "><p id="p17752459184012"><a name="p17752459184012"></a><a name="p17752459184012"></a>HTTPS</p>
    </td>
    </tr>
    </tbody>
    </table>

    请求内容示例如下：

    ```
    {
      "auth": {
        "identity": {
          "methods": [
            "password"
          ],
          "password": {
            "user": {
              "name": "username",    //username为用户名，请根据实际情况替换。
              "password": "******",    //******为用户密码，请根据实际情况替换。    
              "domain": {
                "name": "domainname"    //domainname为域名，请根据实际情况替换。
              }
            }
          }
        },
        "scope": {
          "project": {
            "name": "cn-north-1"    //cn-north-1为区域名，请根据实际情况替换。
    
          }
        }
      }
    }
    ```

2.  <a name="zh-cn_topic_0095238317_zh-cn_topic_0024478020_li2615608112249"></a>获取Token。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。
3.  调用业务接口，在请求消息头中增加“X-Auth-Token”，“X-Auth-Token”的取值为[2](#zh-cn_topic_0095238317_zh-cn_topic_0024478020_li2615608112249)中获取的Token。

