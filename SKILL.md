---
name: equity-transfer-review-skill
description: 股权转让、股份转让、员工持股平台份额转让、上层持股平台转让、境外架构权益转让等交易的法律审查与尽调用 skill。用于审核股权转让协议、补充协议、股东协议、章程条款、工商档案、资料室文件，输出红旗问题表、资料缺口清单、条款修改建议、交割条件清单、交易备忘录或律师复核清单；适用于中国法语境下的转让方处分资格、转让限制、同意程序、监管审批、付款税费、工商变更和交割可完成性审查。
---

# 股权转让审核

## Use When

Use this skill for equity or equity-like transfer review in China-facing transactions, including limited-liability company equity transfers, share transfers, employee stock platform or partnership interest transfers, upper-level holding vehicle transfers, offshore or VIE interest transfers, and exit arrangements in financing or M&A deals.

Do not use it as the lead skill for standalone financing term-sheet drafting, ordinary corporate governance advice, shareholder dispute litigation, pure tax planning, securities trading compliance, or full-scope M&A due diligence. For those, route to the more specific legal skill first and use this skill only for the transfer-closing workstream.

## Core Standard

把股权转让审核作为“交易可交割性审查”，不要停留在合同润色。每个结论都回答：

- 转让方是否有权处分拟转让权益。
- 交易是否能够合法、有效、可证明地完成。
- 买方或受让方应通过哪些条件、文件、付款安排或交割机制控制风险。

默认用中文输出。不要把工作成果表述为正式法律意见书。若用户要求法律意见、监管申报意见或可出具版本，列明假设、资料范围、核验来源、限制和待执业律师复核事项。

## Route

先判断用户目标和输入材料，再加载必要 reference：

- 无材料或早期咨询：用户只描述交易、没有上传文件，先读取 `references/intake-questionnaire.md`，输出关键问题问卷、资料清单和建议审核路径。
- 交易类型不明或包含特殊主体/特殊权益：读取 `references/scenario-gates.md`，先完成交易类型分流，再进入条款或尽调审查。
- 协议审核：用户提供股权转让协议、补充协议、股东协议或章程条款时，读取 `references/contract-review-playbook.md`。
- 交易尽调：用户提供资料室、工商档案、历史沿革、出资或税务材料时，读取 `references/materials-checklist.md` 和 `references/risk-taxonomy.md`。
- 红旗、备忘录或清单：用户要求风险清单、问题台账、补充资料清单、交割条件或 memo 时，读取 `references/output-templates.md`。
- 复杂监管：涉及国资、外资、上市公司、新三板、金融、教育、医疗、数据、互联网、经营者集中、国家安全审查、跨境架构或境外权益时，读取 `references/legal-basis-refresh.md` 并核验最新官方来源。
- 修订批注版：用户要求直接处理 DOCX 时，叠加能处理 Word 修订或批注的文档 skill；本 skill 只负责法律审查逻辑和批注内容。

如果用户没有提供文件，不要假装已经完成审核。输出定制化资料清单、检索方案、关键问题问卷和建议的审核路径。

## Workflow

1. 先做交易类型分流：确认有限责任公司股权、股份公司股份、合伙或员工持股平台份额、上层平台权益、境外或 VIE 权益、国资、上市/挂牌、外资、监管行业或控制权变更等触发项。
2. 固定交易画像：列明标的公司、司法辖区、主体类型、转让方、受让方、比例、价款、基准日、签署日、交割日、付款路径和交易目的。
3. 建立证据地图：逐份列出文件名、日期、签署或盖章状态、来源、可靠性、页码或截图路径；关键金额、比例、日期、主体名称和签章必须回看原件或原图。
4. 审查权属与处分资格：核对登记股东、实益持有人、出资取得、代持、信托、共有、质押、冻结、查封、执行、破产、继承争议、认缴/实缴状态、出资责任和税务凭证。
5. 审查转让限制与同意程序：核查章程、股东协议、投资协议、特殊权利、优先购买权、同意权、共同出售、强制随售、锁定期、禁止转让、控制权变更、回购、董事会或股东会批准、投资人否决权、配偶同意等。
6. 审查交易文件：逐条检查标的、价款、付款、税费、先决条件、交割、工商变更、陈述保证、披露、过渡期、违约责任、赔偿、解除、保密、争议解决和通知。
7. 审查监管与第三方要求：对国资、外资、上市或挂牌、金融和其他监管行业确认审批、评估、挂牌、备案、披露、锁定期、适格股东和交易方式要求；对经营者集中、国家安全审查、外汇、税务、境外投资、数据安全、网络安全列为专项问题。
8. 形成交易导向结论：每个问题按“事实、依据、风险、影响、建议、交割处理、待补充”输出；把建议落到条件先决、交割交付物、价款留置、监管账户、赔偿、陈述保证、披露函、交割后承诺、终止权或交易前整改。

## Output Rules

默认优先输出高信号成果：

- 结论摘要：3-8 条，只写影响签署、交割、估值、控制权或责任承担的事项。
- 交易类型分流：先说明适用的交易类型、强制核验项和不适用项。
- 红旗问题表、资料缺口清单、条款修改建议、交割条件清单、监管闸门表和来源登记表；表格字段使用 `references/output-templates.md`。

风险等级使用：`重大`、`较高`、`中等`、`低`、`信息缺口`。不要只写“建议完善”；必须说明完善到什么程度、由谁提供、何时完成、完成证据是什么。

## Evidence Rules

使用简洁、可追溯引用：

- 文件引用：例如《股权转让协议》第 2.1 条、《公司章程》第 8 页第十六条。
- 登记引用：例如国家企业信用信息公示系统，查询日期，检索主体。
- 付款引用：例如银行回单日期、付款方、收款方、金额和用途。
- 推论引用：标为“推论”，并列出组合依据。

证据冲突时，先列冲突，再评估来源可靠性。不要在展示可靠性分析之前直接选择一个结论。

## Provenance

本 skill 为原创重写和扩展的法律工作流，灵感来自公开小红书笔记《股权转让skill》（氛围律师 VibeLawyer，2026-06-19）。仓库不包含原图、原文搬运或第三方素材；来源笔记不是法律依据。完整署名和边界见 `ATTRIBUTION.md`。
