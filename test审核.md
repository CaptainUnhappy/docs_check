# Market Value 文档审核

## 英文

### 概念性问题

1. **术语解释不足**：
   ```
   $TAT is intended to record the economic value of the underlying various asset production.
   ```
   - 没有解释$TAT是什么，新用户可能不了解这个缩写代表什么
   - 没有详细说明"underlying various asset production"具体指的是哪些资产

2. **概念不明确**：
   ```
   Treasurenet's Oracle module uses the Oracle Feeder Tool to query for values from whitelisted data sources.
   ```
   - 没有解释什么是"Oracle Feeder Tool"
   - 没有说明"whitelisted data sources"包括哪些数据源

3. **公式表达有误**：
   ```
   - OIL Market value (USD) = Daily production _ Daily price _ Oil price discount
   - GAS Market value (USD) = Daily production \* Daily price
   ```
   - 油价公式中使用了下划线"_"而不是乘号"*"，格式不一致
   - 天然气公式中使用了反斜杠加星号"\*"而不是简单的星号"*"

4. **概念连接不清晰**：
   ```
   The oil price discount is a unique rule for this asset class, different oil grades correspond to different values. Acidity, and API gravity of the Oil production matters.
   ```
   - 没有明确解释API重力值的含义和重要性
   - 提到"这三个值"但只列出了两个值(API重力和酸度)

### 语法问题

1. **公式格式错误**：
   ```
   - OIL Market value (USD) = Daily production _ Daily price _ Oil price discount
   - GAS Market value (USD) = Daily production \* Daily price
   ```
   - 使用了不一致的乘法符号表示法("_"和"\*")

## 中文

### 概念性问题

1. **术语解释不足**：
   ```
   $TAT 旨在记录各种资产生产的经济价值。
   ```
   - 没有解释$TAT是什么，新用户可能不了解这个缩写代表什么

2. **概念不明确**：
   ```
   Treasurenet 的 Oracle 模块使用 Oracle Feeder 工具从白名单数据源查询价值。
   ```
   - 没有解释什么是"Oracle Feeder 工具"
   - 没有说明"白名单数据源"包括哪些数据源

3. **公式表达有误**：
   ```
   - 油价市场价值（美元）= 日产量 _ 日价格 _ 油价折扣
   - 天然气市场价值（美元）= 日产量 \* 日价格
   ```
   - 油价公式中使用了下划线"_"而不是乘号"*"，格式不一致
   - 天然气公式中使用了反斜杠加星号"\*"而不是简单的星号"*"

4. **概念连接不清晰**：
   ```
   油价折扣是这一资产类别的一项特殊规则，不同的油级对应不同的值。油的酸度和 API 重力值很重要。这三个值将影响该油井的油价折扣的大小，具体如下：
   ```
   - 提到"这三个值"但只列出了两个值(API重力和酸度)
   - 没有明确解释API重力值的含义和重要性

### 语法问题

1. **公式格式错误**：
   ```
   - 油价市场价值（美元）= 日产量 _ 日价格 _ 油价折扣
   - 天然气市场价值（美元）= 日产量 \* 日价格
   ```
   - 使用了不一致的乘法符号表示法("_"和"\*")

## 改进建议

### 英文部分

1. **术语解释完善**：
   - 在文档开头解释$TAT的完整含义
   - 示例："$TAT (Treasurenet Asset Token) is intended to record..."
   - 详细说明"underlying various asset production"具体指的是哪些资产类型

2. **概念明确化**：
   - 添加Oracle Feeder Tool的简要说明
   - 列出白名单数据源的示例或类型
   - 示例："...Oracle Feeder Tool (a data collection mechanism) to query for values from whitelisted data sources such as commodity exchanges and financial data providers."

3. **公式表达统一**：
   - 统一使用乘号"*"表示乘法
   - 修正为：
     ```
     - OIL Market value (USD) = Daily production * Daily price * Oil price discount
     - GAS Market value (USD) = Daily production * Daily price
     ```

4. **概念连接明确化**：
   - 明确解释API重力值的含义和重要性
   - 澄清"这三个值"指的是哪三个值，或修改为"这两个值"
   - 示例："API gravity (a measure of how heavy or light petroleum liquid is compared to water) and acidity of the oil production are critical factors. These two values will affect..."

### 中文部分

1. **术语解释完善**：
   - 在文档开头解释$TAT的完整含义
   - 示例："$TAT (Treasurenet资产代币) 旨在记录..."

2. **概念明确化**：
   - 添加Oracle Feeder工具的简要说明
   - 列出白名单数据源的示例或类型
   - 示例："...Oracle Feeder工具（一种数据收集机制）从白名单数据源（如商品交易所和金融数据提供商）查询价值。"

3. **公式表达统一**：
   - 统一使用乘号"*"表示乘法
   - 修正为：
     ```
     - 油价市场价值（美元）= 日产量 * 日价格 * 油价折扣
     - 天然气市场价值（美元）= 日产量 * 日价格
     ```

4. **概念连接明确化**：
   - 明确解释API重力值的含义和重要性
   - 澄清"这三个值"指的是哪三个值，或修改为"这两个值"
   - 示例："油的API重力值（衡量石油液体与水相比的轻重程度的指标）和酸度是关键因素。这两个值将影响..."

## 优先改进项

1. 解释$TAT的完整含义
2. 统一公式中的乘法符号表示法
3. 澄清"这三个值"的表述问题
4. 添加API重力值的解释

## 总体评价

文档整体结构清晰，中英文内容对应一致，但存在一些术语解释不足和表达不准确的问题。通过实施上述改进建议，可以显著提高文档的清晰度和专业性，使用户更容易理解市场价值的计算方法和相关概念。 