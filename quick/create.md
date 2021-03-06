# 创建加速域名

### 操作步骤

1.选择好计费方式后，点击创建加速，接入您的加速域名。

若您选择流量包预付费，则需先购买流量包才能创建域名。 若您选择日带宽峰值后付费，需保证账户余额>0才能创建域名。

![image-20191202160155391](images/image-20191202160155391.png)

2.点击【创建加速】后，请填写如下配置参数，详细见参数说明。

![image-20191202160241212](images/image-20191202160241212.png)



#### 配置参数说明

| 配置项    | 说明                                                         |
| --------- | :----------------------------------------------------------- |
| 项目组    | 将资源进行分项目管理，项目组可以管理您在UCloud平台的所以资源，可在“权限管理处设置”。 |
| 业务组    | 在对应的项目下设置不同的业务组进行资源管理。                 |
| 类型      | 页面加速：适用于电商类、网站类、游戏图片类静态资源加速场景。 <br> 下载加速：适用于游戏安装包、音视频原文件下载、手机固件分发等场景。<br/> 点播加速：适用于音视频点播加速等场景。 |
| 加速域名  | 指需要使用CDN加速的域名，如example.com，不能以HTTP或者HTTPS开头。<br/> 如开通的加速区域为国内加速，接入的域名必须在工信部备案后方可接入。<br/> 账户维度默认加速域名配额数量20个。<br /> 如需创建泛域名加速，请联系技术支持。 |
| 加速区域  | 目前支持国内加速和国外加速，国内：中国大陆，国外：海外加港澳台  <br/>流量计费模式下，只有购买了国外流量才能选择国外加速区域，带宽计费模式没有限制 |
| 测试URL   | 请输入一个文件的url地址，用于测试网址的连通性和可用性，域名要与前面填写的加速域名一致 |
| 源站      | 源站分为源站IP或域名，允许多个回源IP或者一个回源域名。<br/>当源站IP为多个时，将会以轮询的策略进行回源。<br/> 源站支持UFile公开bucket，暂不支持私有bucket作为源站。 |
| HTTPS加速 | 开启HTTPS加速，需上传域名对应证书。<br/>国内HTTPS可通过控制台直接开启<br/>国外HTTPS需域名接入成功后联系技术支持协助配置，一般需要一个工作日。 |
| 缓存配置  | 缓存配置请参考 https://docs.ucloud.cn/ucdn/guide             |

参数内容填写完成后，点击【创建】后，成功接入加速域名。等待审核通过后会分配对应的CNAME域名。