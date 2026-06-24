# Output Templates

Use these templates when the user asks for a red-flag table, memo, missing-materials list, clause review, or closing checklist.

## Executive Summary

Write 3-8 bullets. Include only issues affecting signing, closing, registration, valuation, control, payment safety, or liability.

```markdown
## 结论摘要

1. 【重大】...
2. 【较高】...
3. 【信息缺口】...
```

## Red-Flag Table

```markdown
| 等级 | 问题 | 事实与证据 | 交易影响 | 建议措施 | 待补充材料 |
|---|---|---|---|---|---|
| 重大 |  |  |  |  |  |
```

Rules:

- Each row must cite a file, official source, platform finding, user-provided claim, or clearly marked inference.
- “待补充材料” must name the document, period, subject, issuer, and use.
- For legal uncertainty, separate “legal issue” from “fact not yet verified”.

## Missing-Materials List

```markdown
| 优先级 | 材料名称 | 涉及主体/期间 | 出具方或提供方 | 用途 | 未提供的影响 |
|---|---|---|---|---|---|
| P0 |  |  |  |  |  |
```

Priority guide:

- P0: Blocks ownership, approval, payment, closing, registration, or regulatory judgment.
- P1: Affects price, liability, disclosure, or timetable.
- P2: Helps improve completeness but does not currently block the main conclusion.

## Clause Revision Table

```markdown
| 条款 | 问题 | 风险影响 | 修改方向 | 示例表述/补充文件 |
|---|---|---|---|---|
| 第 X 条 |  |  |  |  |
```

When giving sample language, keep it conditional and fact-sensitive. If the facts are insufficient, provide drafting instructions instead of pretending the final wording is ready.

## Closing Conditions Checklist

```markdown
| 条件 | 完成标准 | 责任方 | 完成时间 | 完成证据 | 未完成后果 |
|---|---|---|---|---|---|
| 其他股东放弃优先购买权 |  |  |  |  |  |
```

Prefer objective completion standards:

- Signed and sealed resolution.
- Written waiver from all required shareholders.
- Release registration for pledge or freeze.
- Official filing receipt or no-objection evidence.
- Tax declaration proof or withholding evidence.
- Updated shareholder register or registration file.

## Hard Stop Checklist

Use this table when an issue may block signing, closing, registration, payment release, legality, disclosure, or control transfer.

```markdown
| 硬阻断事项 | 触发事实 | 当前状态 | 完成标准 | 未完成后果 | 是否可豁免 |
|---|---|---|---|---|---|
| 国资评估/进场交易 |  | verified / unverified / conflict |  |  | 不建议豁免/可附条件豁免 |
```

Rules:

- Do not mark a hard stop as waived unless the legal basis and commercial instruction are both clear.
- If the issue is only suspected, mark it as `信息缺口` and state the minimum fact needed to classify it.
- Tie every hard stop to a condition precedent, closing deferral, long-stop date, or termination right.

## Regulatory Gate Table

```markdown
| 监管闸门 | 是否触发 | 触发事实 | 核验来源 | 完成证据 | 交易控制 |
|---|---|---|---|---|---|
| 国资 | 是/否/不明 |  |  |  |  |
| 上市/新三板 | 是/否/不明 |  |  |  |  |
| 外资/监管行业 | 是/否/不明 |  |  |  |  |
| 经营者集中/国家安全/数据安全 | 是/否/不明 |  |  |  |  |
| 税务/外汇/跨境付款 | 是/否/不明 |  |  |  |  |
```

Use official or primary sources for legal conclusions. Commercial-platform findings may identify issues but must remain `platform_found` until official-source verification is complete.

## Source Register

```markdown
| 编号 | 来源 | 类型 | 日期 | 关键内容 | 可靠性 | 备注 |
|---|---|---|---|---|---|---|
| S1 | 《股权转让协议》 | 文件 |  |  | 原件/扫描件/OCR |  |
```

Use evidence labels when helpful:

- `verified`: official source or primary file cross-check supports the point.
- `single_source_database`: one Tier 1 source supports the point, cross-check pending.
- `platform_found`: commercial platform result, official verification pending.
- `case_file_claim`: appears in provided transaction file or party statement, not independently accepted.
- `model_inference`: reasoned conclusion from identified evidence.
- `unverified`: mentioned but unsupported.
- `conflict`: sources conflict and must be reconciled.

## Memo Structure

```markdown
# 股权转让审查备忘录

## 一、审查范围与资料

## 二、交易画像与类型分流

## 三、结论摘要

## 四、硬阻断事项与监管闸门

## 五、红旗问题

## 六、资料缺口与核验事项

## 七、条款修改与交割条件

## 八、来源登记与限制说明
```

Do not style an internal memo as a formal legal opinion unless the user expressly asks for an opinion-ready version and provides enough verified materials.
