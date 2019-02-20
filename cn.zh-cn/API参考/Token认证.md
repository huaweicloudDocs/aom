# Token认证<a name="ZH-CN_TOPIC_0096010437"></a>

## 应用场景<a name="zh-cn_topic_0095238317_zh-cn_topic_0024478020_section5608799912249"></a>

当您使用Token认证方式完成认证鉴权时，需要获取用户Token并在调用接口时增加“X-Auth-Token”到业务接口请求消息头中。

本节介绍如何调用接口完成Token认证。如何获取Token值，请参考[获取用户Token](http://support.huaweicloud.com/api-iam/zh-cn_topic_0057845583.html)。

## 调用接口步骤<a name="zh-cn_topic_0095238317_zh-cn_topic_0024478020_section3546598312249"></a>

1.  发送“POST https://_**IAM的Endpoint**_/v3/auth/tokens”，获取IAM的Endpoint及消息体中的区域名称，请参考[地区和终端节点](https://developer.huaweicloud.com/endpoint)。

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

