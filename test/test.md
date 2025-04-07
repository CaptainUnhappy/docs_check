Market Value
What is market value?
$TAT is intended to record the economic value of the underlying various asset production.

Here, market value refers to the value of natural gas and oil produced as observed in real-world trading markets. Treasurenet’s Oracle module uses the Oracle Feeder Tool to query for values from whitelisted data sources.

How to calculate market value?
Different assets have different ways of calculating market value. But, the general framework would be to

observe a publicly acceptable financial value and
apply any relevant discount factor
Here, the current market value calculation is simple for natural gas and oil, due to the naturally observable qualities of the asset.

- OIL Market value (USD) = Daily production _ Daily price _ Oil price discount
- GAS Market value (USD) = Daily production \* Daily price

What is the Oil price discount?
The oil price discount is a unique rule for this asset class, different oil grades correspond to different values. Acidity, and API gravity of the Oil production matters. These three values will affect the size of the oil price discount for this well, specifically as follows:

- 90% discount ratio: API gravity > 31.10 && Acidity < 0.50%
- 85% discount ratio: API gravity > 31.10 && Acidity >= 0.50%
- 80% discount ratio: API gravity <= 31.10 && Acidity < 0.50%
- 75% discount ratio: API gravity <= 31.10 && Acidity >= 0.50%

市场价值
什么是市场价值？
$TAT 旨在记录各种资产生产的经济价值。

在这里，市场价值指的是天然气和石油在实际交易市场上的价值。Treasurenet 的 Oracle 模块使用 Oracle Feeder 工具从白名单数据源查询价值。

如何计算市场价值？
不同的资产有不同的市场价值计算方式。但是，一般的框架是：

观察一个公认的金融价值，并且
应用任何相关的折扣因素
在这里，目前的市场价值计算对于天然气和石油来说是简单的，因为这些资产具有自然可观察的特性。

- 油价市场价值（美元）= 日产量 _ 日价格 _ 油价折扣
- 天然气市场价值（美元）= 日产量 \* 日价格

什么是油价折扣？
油价折扣是这一资产类别的一项特殊规则，不同的油级对应不同的值。油的酸度和 API 重力值很重要。这三个值将影响该油井的油价折扣的大小，具体如下：

- 90% 折扣比率：API 重力值 > 31.10 && 酸度 < 0.50%
- 85% 折扣比率：API 重力值 > 31.10 && 酸度 >= 0.50%
- 80% 折扣比率：API 重力值 <= 31.10 && 酸度 < 0.50%
- 75% 折扣比率：API 重力值 <= 31.10 && 酸度 >= 0.50%
