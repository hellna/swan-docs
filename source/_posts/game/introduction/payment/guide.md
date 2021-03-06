---
title:  百度收银台支付开通指引
layout: gamedoc
categoryName: introduction
sidebar: payment
topic: payment
priority: 03-01
---

## 百度收银台支付产品介绍
百度收银台支付是百度面向有开发能力的智能小程序合作者提供的支付能力，聚合了主流的百度钱包、微信、支付宝、网银等多种支付方式，方便开发者一站式快速接入多种支付渠道，让百度用户能在智能小程序场景下，直接完成支付、交易闭环，提升用户支付体验的同时，提高订单转化率。

百度收银台接入后效果：
智能小程序订单确认页 - 百度收银台（弹窗）- 完成付款。
![图片](/img/game/introduction/payment/0.png)

## 百度收银台支付账号开通
开通条件：已完成认证的账号，且需要提供企业营业执照及对公银行账户

开通百度收银台账号有两种方式：
* 若您已入驻百度电商平台，可以绑定已有电商平台账号。 
* 若无百度电商平台账号，可以重新开通账号

#### 绑定已有百度电商平台账号
1. 绑定电商平台账号，在百度收银台下，点击“点击此处”。
![图片](/img/game/introduction/payment/1.png)
2. 输入百度电商平台账号的用户名、密码。
![图片](/img/game/introduction/payment/2.png)
3. 小程序与支付服务绑定，可以选择已创建的支付服务或重新创建新的支付服务。
   绑定支付服务入口“百度收银台 - 开通流程 - 前往设置”。
![图片](/img/game/introduction/payment/3.png)
   绑定支付服务：可以创建新服务或绑定已有服务。
![图片](/img/game/introduction/payment/4.png)

#### 创建新的账号

1. 百度收银台开通流程下，点击“前往提交”。
![图片](/img/game/introduction/payment/5.png)
2. 勾选服务协议。
![图片](/img/game/introduction/payment/6.png)
3. 资质填写，包括企业信息及法人信息，资质审核需要 2 个工作日。
![图片](/img/game/introduction/payment/7.png)
![图片](/img/game/introduction/payment/8.png)

4. 资质审核通过后，可进行开发者信息设置

   开发者设置入口：百度收银台 - 开通流程 - 前往设置。
   ![图片](/img/game/introduction/payment/9.png)
   
   设置信息包括开发者公钥和收银台参数（线上环境）
  ![图片](/img/game/introduction/payment/10.png)
  
5. 创建服务，进入创建服务页，填写服务名称、录入银行卡信息、并且进行财务设置。填写服务信息后，提交平台进行服务审核，审核周期 1 个工作日，审核通过后服务即可上线。
![图片](/img/game/introduction/payment/11.png)
* 目前银行卡仅支持对公账户，请务必保证目前银行卡仅支持对公账户，请务必保证开户名是对公账户名并且和银行开户证明信息一致。
* 银行卡号请正确填写对公银行卡号，卡号不能包含空格。
* 开户银行请填写银行支行全称，请不要填写简称。

![图片](/img/game/introduction/payment/12.png)

|事项|说明|
|--|--|
|结算周期|小程序可以选择 T+1,T+7,T+14,T+28，小游戏默认 T+28。|
|佣金|小程序收取千分之六，小游戏收取百分之一。|
|每日退款上限（元）| 每日发起给用户退款的最大金额。如每日退款上限为 10000 元，当日退款的总金额则不可以超过 10000 元，超过 10000 元则退款失败，次日可以再次发起退款。|
|打款预留（元）| 自动付款至绑定银行卡时，可以设置预留金额，此部分金额不进行付款，预留金额可以用来给用户进行退款，以防企业资产为 0 时，不能给用户退款的情况。如预留金额为 1000 元，T 日产生流水 1200 元，T+1 日则付款 200 元至绑定银行卡，1000 元在企业资产中。打款预留金额可进行修改。|

> 防止资金池金额小于退款金额时退款失败的情况，建议根据业务退款情况，设置“每日退款上限(元)”和“打款预留(元)”。
