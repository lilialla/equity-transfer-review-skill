# Legal Basis Refresh

Use this reference for transactions involving changing law, official registry status, regulatory policy, tax, state-owned assets, foreign investment, listed or NEEQ companies, anti-monopoly, national security review, foreign exchange, data, cybersecurity, or regulated industries.

## Verification Rule

Do not rely on memory for current law or policy. Verify with official or primary sources when the issue may affect legality, approval, filing, timetable, disclosure, tax, or closing.

Record:

- Source name.
- Source type.
- URL or database.
- Retrieval date.
- Effective date if available.
- Relevant article, section, announcement, form, or registry field.
- Limits of the search.

## Preferred Sources

| Topic | Preferred source type |
|---|---|
| Current laws and administrative regulations | Official law database, National People's Congress or State Council publication. |
| Company registration and shareholder status | National Enterprise Credit Information Publicity System and local market-regulation materials. |
| State-owned assets | SASAC rules, local SASAC rules, asset exchange rules, appraisal and listing documents. |
| Foreign investment | MOFCOM, NDRC, State Council, foreign investment access negative list, market-regulation filing materials. |
| Listed companies | CSRC rules, stock exchange rules, official announcements and disclosures. |
| NEEQ | NEEQ official rules and disclosures. |
| Anti-monopoly | SAMR merger-control rules, filing thresholds, official cases and guidance. |
| National security review | Official state security, foreign investment security review, and related State Council or ministry rules. |
| Foreign exchange and cross-border payment | SAFE rules, bank implementation requirements, transaction-specific bank feedback. |
| Tax | State Taxation Administration, local tax authority guidance, tax filing documents. |
| Data and cybersecurity | CAC, MIIT, public-security or sector regulator rules, data export/security assessment rules. |
| Regulated industries | The competent industry regulator and license issuer. |

Commercial databases and AI search tools may help discover issues, but mark them as `platform_found` or `unverified` until official-source verification is done.

## Regulatory Gate Matrix

Use this matrix to convert regulatory uncertainty into closing controls. Do not treat these rows as legal conclusions; use them as triggers for official-source verification.

| Gate | Trigger facts | Official-source check | Completion evidence | Transaction control |
|---|---|---|---|---|
| State-owned assets | State-owned transferor, target, actual controller, asset source, or public asset concern. | Approval authority, valuation/appraisal, appraisal filing or approval, public listing or asset exchange rules, local SASAC requirements. | Approval, valuation/appraisal filing, listing documents, asset exchange transaction certificate, no-objection evidence. | Hard condition precedent, closing deferral, no-waiver rule, long-stop termination. |
| Listed or NEEQ transfer | Listed/NEEQ company, controlling shareholder, restricted shares, related-party transfer, director/supervisor/senior manager, disclosure window. | CSRC, stock exchange, NEEQ rules, issuer announcements, lock-up and disclosure rules. | Disclosure announcement, exchange or NEEQ filing, board/shareholder approval, lock-up clearance. | Disclosure CP, transfer method confirmation, trading-window control, termination right. |
| Foreign investment | Foreign investor, foreign-invested target, negative-list industry, sensitive sector, control transfer, cross-border payment. | Foreign investment access negative list, market-regulation filing, MOFCOM/NDRC/State Council publications, industry regulator rules. | Filing/registration receipt, permit update, regulator consultation record, no-filing analysis with source limits. | Approval/filing CP, permit amendment deliverable, bank pre-review, closing deferral. |
| Financial or licensed industry | Finance, education, medical, telecom, internet, culture, data-heavy, cybersecurity, or other licensed sector. | Competent industry regulator, license issuer, permit transfer/change rules, data/cyber regulator. | Approval, permit amendment, no-objection, regulator consultation, compliance memo. | Industry approval CP, operating covenant, post-closing permit deadline only if legally acceptable. |
| Merger control | Control acquisition, joint control, revenue threshold concern, concentrated market, sensitive sector. | SAMR rules, thresholds, official cases and guidance. | Clearance, simplified-case publication, no-filing memo, counsel/regulator consultation record. | Clearance CP, gun-jumping covenant, long-stop, reverse termination allocation. |
| National security or data/cyber | Sensitive industry, critical infrastructure, important data, data export, foreign control, security review concern. | Official security review, CAC, MIIT, public-security or sector regulator sources. | Security review decision, data export/security assessment evidence, no-trigger analysis with source limits. | Hard CP, data-room limits, closing deferral, termination right. |
| Tax, FX, and payment | Natural person, non-resident, low price, indirect transfer, cross-border payment, offshore structure, installment or escrow. | Tax authority, SAFE, bank requirements, transaction-specific bank feedback. | Tax declaration/payment evidence, withholding evidence, stamp duty proof, bank pre-review, FX registration if applicable. | Tax/FX CP, escrow release condition, withholding covenant, refund/gross-up mechanism. |

## Regulatory Screen

Ask these questions before concluding:

1. Is either party state-owned, publicly listed, NEEQ-listed, foreign-invested, financial, education, medical, internet, data-heavy, or otherwise licensed?
2. Does the transaction transfer control, special voting rights, actual control, VIE interests, offshore holding interests, or employee platform units?
3. Does the transaction require valuation, exchange listing, public disclosure, shareholder approval, board approval, creditor or lender consent, foreign investment review, merger-control filing, national security review, data review, or industry approval?
4. Is there any lock-up, restricted transfer, information disclosure window, insider trading risk, related-party transaction rule, or controlling-shareholder duty?
5. Are tax, foreign exchange, cross-border payment, or bank compliance steps conditions to completion?

## Output Discipline

For each regulatory issue, output:

| Field | Requirement |
|---|---|
| Trigger fact | The fact that may trigger regulation. |
| Source | Official source or marked platform/user source. |
| Legal question | Approval, filing, disclosure, lock-up, tax, FX, industry qualification, or data/cyber issue. |
| Current status | Use one of `verified`, `single_source_database`, `platform_found`, `case_file_claim`, `model_inference`, `unverified`, or `conflict`. |
| Transaction impact | Blocker, condition precedent, timetable risk, disclosure risk, price or liability risk. |
| Next step | Specific official check, document request, counsel call, regulator consultation, or filing plan. |

Never say “no approval is required” unless the facts are complete enough and the source basis is identified. Prefer “no approval requirement was found in the checked sources as of [date], subject to [limits]” when appropriate.
