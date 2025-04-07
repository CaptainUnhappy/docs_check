# Market Value 文档审核

## 英文

### 概念性问题

1. **术语解释不足**：
   ```
   `$TAT` is intended to record the economic value of the underlying various asset production.
   ```
   - 没有解释"$TAT"是什么，以及它的用途和意义
   - 没有说明"underlying various asset production"具体指什么
   - 不理解的概念："$TAT"的具体定义和功能

2. **概念不明确**：
   ```
   Here, market value refers to the value of natural gas and oil produced as observed in real-world trading markets. Treasurenet's Oracle module uses the Oracle Feeder Tool to query for values from whitelisted data sources.
   ```
   - 没有解释"Oracle module"和"Oracle Feeder Tool"的具体功能和作用
   - 没有说明"whitelisted data sources"是什么以及如何选择
   - 不理解的概念："Oracle module"和"Oracle Feeder Tool"的具体功能和关系

3. **概念连接不清晰**：
   ```
   Different assets have different ways of calculating market value. But, the general framework would be to
   1. observe a publicly acceptable financial value and
   2. apply any relevant discount factor
   ```
   - 没有明确解释"publicly acceptable financial value"如何获取
   - 没有说明"relevant discount factor"如何确定
   - 不理解的概念："publicly acceptable financial value"和"relevant discount factor"的具体含义和来源

4. **公式表达有误**：
   ```
   - OIL Market value (USD) = Daily production * Daily price * Oil price discount
   - GAS Market value (USD) = Daily production * Daily price
   ```
   - 乘法符号使用了"*"，应该统一使用"×"
   - 没有解释公式中各个变量的含义和单位
   - 不理解的概念：公式中各个变量的具体含义和单位

5. **概念不明确**：
   ```
   The oil price discount is a unique rule for this asset class, different oil grades correspond to different values. Acidity, and API gravity of the Oil production matters.
   ```
   - 没有解释"API gravity"是什么，以及它的意义和测量方法
   - 没有说明"Acidity"如何测量和影响价格
   - 不理解的概念："API gravity"和"Acidity"的具体含义和测量方法

6. **概念连接不清晰**：
   ```
   These three values will affect the size of the oil price discount for this well, specifically as follows:
   ```
   - 前文只提到了两个值（Acidity和API gravity），但这里提到"These three values"
   - 没有明确解释第三个值是什么
   - 不理解的概念：第三个影响油价折扣的值是什么

### 语法问题

1. **标点符号使用不当**：
   - 文档中使用了破折号"-"作为列表项标记，但在英文文档中通常使用项目符号"•"或数字

## 改进建议

### 英文部分

1. **术语解释完善**：
   - 解释"$TAT"的具体含义和功能
   - 示例："$TAT is a token that represents the economic value of real-world assets like natural gas and oil. It is minted based on the verified production and market value of these assets."

2. **概念明确化**：
   - 解释"Oracle module"和"Oracle Feeder Tool"的功能和作用
   - 示例："The Oracle module is a system that provides verified external data to the blockchain. The Oracle Feeder Tool is an automated system that queries trusted data sources to obtain market prices and production data for assets."

3. **概念连接明确化**：
   - 明确解释"publicly acceptable financial value"和"relevant discount factor"
   - 示例："Publicly acceptable financial value refers to market prices from recognized exchanges or industry publications. Relevant discount factors are adjustments applied to the base price based on asset quality, location, or other factors."

4. **公式表达修正**：
   - 修正乘法符号，使用标准符号
   - 示例："OIL Market value (USD) = Daily production × Daily price × Oil price discount"
   - 添加变量解释："Daily production: The amount of oil produced in one day (measured in barrels). Daily price: The market price of oil per barrel on that day. Oil price discount: A percentage applied based on oil quality."

5. **概念明确化**：
   - 解释"API gravity"和"Acidity"
   - 示例："API gravity is a measure of how heavy or light petroleum liquid is compared to water. It is used to classify oil types, with higher API gravity indicating lighter oil. Acidity refers to the amount of acidic compounds in the oil, measured as a percentage of total weight."

6. **概念连接明确化**：
   - 明确解释影响油价折扣的因素
   - 示例："Two main factors affect the oil price discount: API gravity and acidity. API gravity determines if the oil is light (>31.10) or heavy (≤31.10), while acidity determines if the oil is sweet (<0.50%) or sour (≥0.50%). These classifications together determine the discount ratio applied to the base price."

## 相关链接

- [Market Value 文档](https://docs.treasurenet.io/docs/assets/tat_mint/market_value)
- [Production Audit 文档](https://docs.treasurenet.io/docs/assets/tat_mint/production_audit)
- [Data Requirements 文档](https://docs.treasurenet.io/docs/assets/tat_mint/data_requirements) 