英文
```
Production Audit
Production audit refers to the comparison of Producer’s reported production quantity against published government production record, from the previous month, to calculate a production deviation ratio.

According to the production deviation ratio, the Producer's collateral will be deducted if applicable, and the reported production quantity will be adjusted to align with the result of the production audit.

How is a production audit conducted?
Each asset class has its own asset data module for data processing and audit. Here, the OilData and GasData modules are utilized, in tandem with the Oracle module.

Producers can use an automated Tool, the ProductionData Uploader for reporting each natural gas and oil well’s daily production.

Notice: Treasurenet automated Tool requires connection to industry accepted production recording hardware and data service.

Monthly, an automated Tool, the Oracle Feeder Tool, will fetch the production data of that well from the whitelisted government publications;

The OilData and GasData module will compare the reported values and published values to calculate the production deviation ratio for the month;

Production deviation ratio = (Producer's reported production stored on the chain - whitelist reported production) / whitelist reported production \_ 100%

Calculate the verified production quantity and its corresponding market value based on the production deviation ratio for the month;

Deduct collateral, if applicable, according to the production deviation ratio

How to start a production audit?
In the WellManagement page of the Producer Portal, Producers select and click [Mint TAT].

Choose [yes] in the pop-up window

Trigger the audit action for that month's production.
Mint the corresponding TAT according to the production audit result
```
中文
```
生产审计
生产审计是指将生产商报告的生产数量与政府发布的生产记录进行比对，以计算生产偏差比例。

根据生产偏差比例，如适用，将扣除生产商的担保物，并将报告的生产数量调整为与生产审计结果相符。

如何进行生产审计？
每个资产类别都有自己的资产数据模块用于数据处理和审计。这里，使用了 OilData 和 GasData 模块，与 Oracle 模块一起配合使用。

生产商可以使用自动化工具——ProductionData Uploader，报告每口天然气井和油井的日产量。

注意：Treasurenet 自动化工具需要连接到行业公认的生产记录硬件和数据服务。

每月，自动化工具——Oracle Feeder Tool，将从白名单政府出版物中获取该井的生产数据；

OilData 和 GasData 模块将比较报告值和发布值，计算该月的生产偏差比例；

生产偏差比例 =（链上存储的生产商报告的生产量 - 白名单报告的生产量）/ 白名单报告的生产量 × 100%

根据月度生产偏差比例计算验证的生产数量及其相应的市场价值；

根据生产偏差比例，如适用，扣除担保物。

如何开始生产审计？
在生产商门户网站的 WellManagement 页面上，生产商选择并点击[Mint TAT]。

在弹出窗口中选择[是]

触发该月份生产的审计操作。
根据生产审计结果，铸造相应的 TAT。
```