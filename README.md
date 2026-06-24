<p align="center">
  <img src="assets/logo.svg" width="128" alt="股权转让审核 Skill logo">
</p>

# 股权转让审核 Skill

这是一个面向中国法语境的开源法律 skill，用于辅助律师、法务或 AI agent 审查股权转让、股份转让、持股平台份额转让和投融资退出类交易。

它的核心目标不是做合同润色，而是围绕交易是否可交割建立审查框架：交易画像、权属核验、转让限制、内部批准、监管路径、税务事项、资料缺口、红旗风险、条款修改建议和交割条件。

## 使用方式

在支持本地 skill 加载的 agent 环境中使用本仓库，并把交易文件或事实材料交给 agent：

```text
Use $equity-transfer-review-skill to review this equity transfer deal.
Please output: transaction snapshot, evidence map, red-flag table,
missing materials, clause revision suggestions, and closing conditions.
```

如果没有交易文件，本 skill 应先输出资料清单、追问问题和审核路径，不应假装完成审核。

## 仓库结构

```text
SKILL.md                       # Agent 运行入口
agents/openai.yaml             # Skill metadata
assets/logo.svg                # Project logo
references/contract-review-playbook.md
references/materials-checklist.md
references/risk-taxonomy.md
references/output-templates.md
references/legal-basis-refresh.md
ATTRIBUTION.md                 # 原作者署名与原创边界
LICENSE                        # MIT
```

## 原创扩展

本项目参考了公开笔记中的方向，但没有搬运原图、原文或排版素材。已重写并扩展为独立 skill：

- 增加交易画像和证据地图。
- 增加权属、限制、程序、监管、税务、价款和交割维度的红旗分类。
- 增加资料缺口、条款修改、交割条件和 memo 输出模板。
- 增加 evidence-grade 输出纪律，区分文件事实、官方核验、平台发现、模型推论和未核验事项。
- 增加复杂场景的官方来源刷新要求。

灵感来源、署名和非背书说明见 [ATTRIBUTION.md](ATTRIBUTION.md)。

## 边界

- 这不是正式法律意见书。
- 不自动保证现行法、监管口径、工商登记、税务政策最新。
- 涉及国资、外资、上市/挂牌、金融、医疗、教育、数据、互联网、经营者集中、国家安全审查等事项时，必须核验最新官方来源。
- 对真实交易，不应把客户陈述直接当作已查明事实。

## License

MIT. See [LICENSE](LICENSE).
