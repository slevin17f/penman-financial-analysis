---
name: penman-financial-analysis
description: |
  按 Stephen Penman《Financial Statement Analysis and Security Valuation》第五版分析报表与证券价值。用于重构经营和融资、分解盈利、用剩余收益或异常盈利增长估值、反推价格隐含增长、编制预测及检查会计质量和偿债缺口。
metadata:
  cangjie.generated-by: cangjie-tools v2.5.0
  cangjie.variant: single
  cangjie.bundle-id: bundle.penman-financial-analysis
  cangjie.capability-count: 13
  cangjie.entrypoint-count: 1
---
# Financial Statement Analysis and Security Valuation（国际版第五版） — 全书能力入口

## 触发与不触发

**适用**：与本书能力域相关的咨询与任务（见下方路由表的意图列）。
**不适用**：
- 即时行情获取、个性化交易指令及审计鉴证。

## 核心原则（常驻速览，概览类问题读到这里即可回答）

1. 先明确估值日、财报可得日、币种单位、总额或每股、权利人、预测期及要求回报率的对象。把原始披露、重分类和预测分列。
2. 做完整案例时先核权益桥，再分经营和融资，拆出可持续盈利，最后预测剩余收益、检查终值并反推价格要求。单项问题只加载所需卡片。
3. 列出公式、代入值、对账差额、终值假设及一项足以改变结果的情景。缺少数据时交付可算部分与缺项。

## 能力路由（先读本表，按意图加载 1 张能力卡）

| 用户意图 | 先读 | 补读/备注 |
|---|---|---|
| 从业务和报表选择估值模型，核对自由现金流与折现对象 | references/capabilities/models.md | references/capabilities/residual.md、references/capabilities/operations.md |
| 用期初账面权益和剩余收益解释市净率 | references/capabilities/residual.md | references/capabilities/equity.md、references/capabilities/implied.md |
| 从远期盈利和异常盈利增长解释市盈率 | references/capabilities/aeg.md | references/capabilities/residual.md、references/capabilities/implied.md |
| 从市场价反推出隐含增长，并检验该预期 | references/capabilities/implied.md | references/capabilities/residual.md、references/capabilities/risk.md |
| 从权益变动表核对综合收益与普通股东净分配 | references/capabilities/equity.md | references/capabilities/operations.md、references/capabilities/residual.md |
| 重构经营与融资项目，核对现金流勾稽 | references/capabilities/operations.md | references/capabilities/equity.md、references/capabilities/returns.md |
| 拆解净经营回报和融资杠杆对权益回报的贡献 | references/capabilities/returns.md | references/capabilities/operations.md、references/capabilities/growth.md |
| 区分可持续盈利、非经常项目和资本投入驱动的增长 | references/capabilities/growth.md | references/capabilities/returns.md、references/capabilities/quality.md |
| 估算剩余经营收益并桥接企业价值与普通股价值 | references/capabilities/operating-value.md | references/capabilities/operations.md、references/capabilities/forecast.md |
| 把经营战略译成一组可勾稽的预测报表 | references/capabilities/forecast.md | references/capabilities/growth.md、references/capabilities/operating-value.md |
| 检查会计确认时点和准备金对未来盈利的影响 | references/capabilities/quality.md | references/capabilities/growth.md、references/capabilities/forecast.md |
| 比较经营情景和价格对应的股权预期回报 | references/capabilities/risk.md | references/capabilities/implied.md、references/capabilities/forecast.md |
| 按债务到期表检验偿债覆盖并定位现金缺口 | references/capabilities/credit.md | references/capabilities/operations.md、references/capabilities/forecast.md |

**非能力类查询**：
- 书名/作者/章节/整书概览 → references/overview.md
- 术语解释 → references/glossary.md
- 决策规则速查（不需要原文依据时） → references/cheatsheet.md
- 完整意图与关键词索引（本表未覆盖的意图先查这里） → references/capability-index.md

## 加载规则

- 每次任务先读本文件，再按路由表加载 **1** 张能力卡；任务明确跨域时最多加载 2 张。
- 概览/书名类问题不加载能力卡，用「核心原则」与 overview.md 回答。
- 路由表与 capability-index.md 都无法命中的意图，明确告知超出本书范围，不要硬套。

## 边界与判停

- 估值人与折现率或损益归属无法配对时暂停报出点估值；关键披露缺失时给出有依据的条件区间。
