# 补充性规格说明

@(SSAD)

### <center> **补充性规格说明**

#### 修订历史
|版本|日期|描述|作者|
|---|---|---|---|
|初始草案|2018年6月26日|第一个草案。|苏瀚添|

#### 简介
本文档记录了Scan-code-ordering-system所有未在用例中描述的需求。

#### 功能性
1. 日志和错误处理
保存错误日志。
2. 可拔插规则
支持餐厅对某些功能进行个性化定制。
3. 安全性
因为设计扫码支付，因此扫码点餐系统需要对餐厅用户进行认证。

#### 可用性
人性因素

- 强调人性化。餐厅需要根据菜品对菜单进行更改、顾客需要根据菜单点餐，因此页面不宜太复杂，字体不宜过小或者过大，图片不宜过大，使顾客能够在最短的时间内获取必要的信息。
- 不淡化服务员在服务中的作用。顾客出现问题，应该有服务员及时解决，扫码点餐不代表和服务员完全脱离，应该避免点餐系统反客为主，淡化服务员作用，降低顾客的体验。
- 声音提示。点餐系统出现订单的增加或者变更，应该响起相应提示音，避免服务员错过订单。

#### 可靠性
1. 可恢复性
及时保存订单信息入数据库，避免订单信息丢失或者系统出错导致订单丢失的情况，使订单信息能够具有可恢复性。

2. 性能
应该保证系统性能，避免降低工作效率，给顾客带来不好的体验。

#### 可支持性
1. 可适应性
扫码点餐系统面向的顾客持有不同的手机，系统应该支持各种手机和与之对应的系统。

2. 可配置性。
系统应该能够在各种餐厅的电脑设备中可靠准确快速稳定地运行。

#### 实现约束
项目小组决定采用web技术解决方案。

#### 购买构件
本系统项目暂不需要购买构件。

#### 免费开源构件
我们在系统中尽量使用免费的web技术开源构件。

#### 接口
1. 重要硬件和接口
用户手机端、餐厅电脑端。

2. 软件接口
需要与外部支付系统协作，需要微信/支付宝作为外部的支付系统接入在本系统中，接入桥梁可能为支付的二维码。

#### 应用的领域（业务）规则
|ID|规则|可变性|来源|
|--|-----|---|---|
|规则1|顾客折扣规则。示例：新顾客打8折。|高 每个商家有不同规则|商家|
|规则2|菜品折扣规则。示例：红烧牛肉打8折。|高 每个商家有不同规则|商家|

#### 法律问题
我们使用的构件为开源的，但是必须如果投入使用并且创造盈利，必须给予相应的说明，避免法律纠纷。

#### 所关注领域内的信息
1. 定价
定价必须根据商家制定，真实不造假，系统提供给商家定价的权利，但是系统并不私自制定价格。

2. 支付处理
目前系统暂时根据商家微信/支付宝二维码进行支付，待系统改进之后可能会利用微信或者支付宝的api，进行直接对商家微信/支付宝账户支付。


