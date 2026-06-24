# Scenario Gates

Use this reference before substantive review when the transaction type is unclear or when special rights, special entities, or regulated industries may be involved.

The goal is to classify the deal before selecting materials, risk categories, legal-source checks, and closing controls.

## Gate Matrix

| Scenario | Trigger facts | Must check | Typical closing controls |
|---|---|---|---|
| Limited-liability company equity transfer | Target is an LLC; subject is registered equity or subscribed capital. | Registered shareholder, subscribed/paid-in capital, articles, shareholder consent or waiver, preemptive right procedure, registration change. | Waiver letters, shareholder resolution, articles amendment, updated shareholder register, market-regulation filing, price holdback for registration. |
| Company contribution liability | Unpaid, accelerated, defective, withdrawn, non-monetary, or disputed capital contribution. | Contribution schedule, payment proof, valuation of non-cash contribution, creditor claim or acceleration risk, liability allocation between transferor and transferee. | Pre-closing cure, special indemnity, escrow/holdback, disclosure schedule, contribution warranty survival, price adjustment. |
| 股份公司股份转让 | Target is a joint-stock company; shares may be restricted, pledged, locked up, or listed/NEEQ-related. | Share class, shareholder register, transfer venue or method, lock-up, disclosure, insider/related-party rules, board/shareholder approvals. | Transfer method confirmation, disclosure CP, lock-up clearance, exchange/NEEQ filing evidence, special termination right. |
| Partnership or employee platform unit transfer | Subject is partnership interest, employee incentive unit, ESOP platform share, or indirect participation right. | Partnership agreement, GP consent, platform rules, vesting, repurchase, bad leaver/good leaver, tax and withholding, nominee or incentive documentation. | GP consent, platform resolution, repurchase waiver, tax withholding evidence, revised platform register, post-closing covenant. |
| Upper-level holding vehicle transfer | Parties transfer shares or interests in an entity that indirectly holds the target. | Upstream cap table, change-of-control clauses, investor rights, tax on indirect transfer, downstream consent, consolidated control impact. | Upstream consent package, disclosure schedule, downstream no-breach confirmation, tax filing plan, control-change waiver. |
| Offshore or VIE interest transfer | Offshore holding, red-chip, VIE documents, ODI/FDI/SAFE, or cross-border payment is involved. | Offshore chain, VIE control documents, foreign investment access, ODI/FDI/SAFE, bank requirements, indirect transfer tax, data/cyber issues if relevant. | Legal-source memo, bank checklist, tax filing evidence, VIE document amendment, long-stop and termination right. |
| State-owned asset transfer | Transferor, target, actual controller, or asset source is state-owned or public asset related. | Approval authority, valuation, appraisal filing/approval, exchange listing, public transaction, internal decision, asset exchange rules. | Approval and appraisal CP, exchange transaction evidence, public listing completion, no-objection evidence, closing deferral. |
| Listed, NEEQ, or securities-regulated transfer | Listed/NEEQ company, controlling shareholder, director/supervisor/senior manager, restricted shares, disclosure window, or related-party transaction. | Lock-up, trading method, disclosure, related-party approval, insider information, short-swing or reduction rules, exchange/CSRC/NEEQ rules. | Disclosure CP, trading window confirmation, board/shareholder approval, exchange filing, lock-up clearance, special termination right. |
| Foreign investment or regulated industry | Foreign investor, foreign-invested target, negative-list industry, finance, education, medical, internet, data-heavy, telecom, culture, or other licensed sector. | Access restrictions, qualification, information reporting, industry approval, permit change, national security review, data/cyber review. | Approval/filing CP, permit amendment evidence, regulator consultation record, no-filing analysis, closing deferral. |
| Tax, foreign exchange, and payment completion | Natural person, non-resident, low-price transfer, installment, escrow, cross-border payment, or offshore indirect transfer. | Tax basis, withholding, filing, stamp duty, low-price adjustment, treaty position if any, FX registration, bank review materials. | Tax filing and payment evidence, withholding covenant, bank pre-review, escrow release condition, refund and gross-up mechanism. |
| Merger control or competition concern | Control acquisition, revenue thresholds, joint control, concentrated industry, or sensitive sector. | Filing thresholds, control definition, gun-jumping risk, timetable, SAMR or competent authority guidance. | Filing/no-filing analysis, clearance CP, interim operation covenant, long-stop and reverse termination allocation. |

## Classification Output

At the start of a review, include a short classification:

```markdown
## 交易类型分流

| 类型 | 是否触发 | 依据/事实 | 后续核验 |
|---|---|---|---|
| 有限责任公司股权转让 | 是/否/不明 |  |  |
| 出资责任专项 | 是/否/不明 |  |  |
| 国资/上市/外资/监管行业 | 是/否/不明 |  |  |
```

If a gate is `不明`, treat it as `信息缺口` and request the minimum facts or documents needed to classify it. If a gate is triggered, connect it to a condition precedent, closing deliverable, source verification item, or termination fallback.
