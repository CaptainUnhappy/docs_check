# Market Value 文档审核

## 英文

### 概念性问题

1. **关键术语未解释**：

   ```
   $TAT is intended to record the economic value of the underlying various asset production.
   ```

   - "$TAT"是一个关键术语，但文档中没有提供明确解释
   - 建议添加$TAT 的具体定义和用途说明

2. **术语解释不足**：

   ```
   Treasurenet's Oracle module uses the Oracle Feeder Tool to query for values from whitelisted data sources.
   ```

   - "Oracle module"和"Oracle Feeder Tool"缺乏必要解释
   - 没有说明什么是"whitelisted data sources"以及如何确定这些数据源

3. **公式表达有误**：

   ```
   - OIL Market value (USD) = Daily production _ Daily price _ Oil price discount
   ```

   - 公式中使用了下划线"\_"而不是乘号"\*"，表达不正确
   - 可能导致用户对计算方法产生误解

4. **概念连接不清晰**：
   ```
   The oil price discount is a unique rule for this asset class, different oil grades correspond to different values. Acidity, and API gravity of the Oil production matters. These three values will affect the size of the oil price discount for this well, specifically as follows:
   ```
   - 提到"these three values"但只列出了两个值(API gravity 和 Acidity)，缺少第三个值的说明
   - 概念之间的关系没有明确说明

### 步骤说明问题

1. **步骤不详细**：
   ```
   observe a publicly acceptable financial value and
   apply any relevant discount factor
   ```
   - 没有详细说明如何观察"publicly acceptable financial value"
   - 没有解释如何确定和应用"relevant discount factor"

### 语法问题

1. **格式不一致**：

   ```
   - OIL Market value (USD) = Daily production _ Daily price _ Oil price discount
   - GAS Market value (USD) = Daily production \* Daily price
   ```

   - 两个公式使用了不同的乘号表示方法("\_"和"\*")，格式不一致
   - 建议统一使用标准乘号"\*"表示

2. **标点符号使用不当**：
   ```
   Different assets have different ways of calculating market value. But, the general framework would be to
   ```
   - "But,"作为句首使用不符合正式文档的写作规范
   - 建议改为连贯的句子结构
