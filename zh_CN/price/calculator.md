# 价格计算

EMQX Cloud 价格计算允许您依据实际业务需求预估创建部署所需费用。对于以前从未使用过 EMQX Cloud 的客户以及要重新组织或扩展 EMQX Cloud 部署规格的用户，EMQX Cloud 价格计算是非常有用的。



## 访问 EMQX Cloud 价格估算

* 对于**未登录** EMQX Cloud 的用户，您可以前往 [价格方案](https://www.emqx.com/zh/cloud/pricing) 页面，使用费用估算。

我们提供了 Serverless 版的价格模拟计算器，您可以根据实际业务来预估每月大致的消费。
![estimate_serverless](./_assets/calculator_serverless.png)

专有版的部署价格则可以选择相应的配置了解到。
![estimate_dedicated](./_assets/calculator_dedicated.png)


* 对于**登录**到 EMQX Cloud 的用户，您可以前往 [新建部署](https://cloud.emqx.com/console/deployments/0?oper=new)，选择专有版的部署规格，使用价格估算，并创建部署。
  
![estimate_console](./_assets/deployment_price.png)


## Serverless 价格公式
连接费用 = 连接的客户端 * 客户端连接的时间（以分钟计算，不足一分钟以一分钟计算） / 1,000,000 *  8 <br/>
流量费用 = 部署流入和流出的消息产生的流量（byte）/ 1024 / 1024 / 1024 * 1.5

::: warning
由于实际使用情况不同，计算价格与实际价格之间可能存在差异，请以账单价格为准。
:::

## 专有版部署每小时价格

您可以在价格页面获取到区域和规格对应部署每小时价格。

![price_detail](./_assets/calculator.png)


> 专业版：选择阿里云平台，深圳区域，最大连接数 1,000，消息上下行 TPS 为 1,000，则每小时价格为 1.28，则每月基础费用为： 1.28 * 730 = 934。





## 支持云服务商和地区（专有版）

EMQX Cloud 目前支持云服务商有：阿里云、华为云、腾讯云和亚马逊云科技。如您需要其他云服务商或地区，您可以提 [工单](../feature/tickets.md)或邮件(cloud-support@emqx.io)与我们取得联系。

| 平台   | 区域                   |
| ------ | ---------------------- |
| 阿里云 | 北京，上海，深圳，杭州，张家口 |
| 华为云 | 广州，上海，北京       |
| 腾讯云 | 广州，上海，北京 |
| 亚马逊云科技 | 宁夏，北京 |
