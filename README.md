**ICO Std 2002:2026**　　　　　　　　　　　　　　July 2026

# ICO Std 2002: Ranking Methodology Standard
## 天机排名方法论标准
### The World's First Cross-Domain Ranking Methodology Universal Standard

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![License: CC BY 4.0](https://img.shields.io/badge/Docs-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Status: Draft](https://img.shields.io/badge/Status-Draft-orange.svg)](#status)
[![Standard: ICO Std 2002](https://img.shields.io/badge/Standard-ICO%20Std%202002-green.svg)](#architecture)

---

## 概述 | Overview

**ICO Std 2002** is the world's first universal standard for ranking methodology across diverse domains. It establishes a rigorous, transparent, and reproducible framework for designing, executing, and verifying ranking systems — from product quality ratings and brand valuations to city image indices and cultural heritage assessments.

**ICO Std 2002** 是全球首个跨领域排名方法论通用标准，为设计、执行和验证排名系统建立了严谨、透明、可复现的框架——覆盖产品质量评级、品牌估值、城市形象指数、文化遗产评估等广泛领域。

## Status

> ⚠️ **Early Stage — Draft for Public Comment**
>
> All specifications are currently in draft form and subject to revision based on community input.

- **Core Specification (Chapters 0–11)**: Draft framework
- **Domain Extensions (SE-01 to SE-09)**: Draft framework
- **Annexes (A–C)**: Draft framework
- **Public Comment Period**: To be announced

## Architecture | 架构

```
┌──────────────────────────────────────────────────────────────┐
│  Verification Layer (验证层)                                 │
│  DPP-CQ (ICO Std 2001) · Audit · Traceability · Certification│
├──────────────────────────────────────────────────────────────┤
│  Extension Layer (扩展层)                                     │
│  SE-01 Products · SE-02 Brands · SE-03 Individuals           │
│  SE-04 Cities · SE-05 Cultural Heritage · SE-06 Restaurants  │
│  SE-07 Intangible Assets · SE-08 Economy · SE-09 ESG         │
├──────────────────────────────────────────────────────────────┤
│  Core Layer (核心层) — ICO Std 2002                         │
│  Principles · Indicator Design · Weighting · Data Collection  │
│  Scoring & Ranking · Publication · Audit · Compliance        │
└──────────────────────────────────────────────────────────────┘
```

## Standards Alignment | 对标标准

| Standard | Alignment Area | Reference |
|---|---|---|
| **IREG Berlin Principles** | Ranking principles & ethics | [Annex A](annex/A-berlin-principles-mapping.md) |
| **ISO 20671** | Indicator system design | [Chapter 5](core/05-indicator-design.md) |
| **ISO 8000** | Data quality & collection | [Chapter 7](core/07-data-collection.md) |
| **ISO 10668** | Brand valuation methodology | [SE-02](extensions/SE-02-brands.md) |
| **ISO 17021** | Audit & conformity assessment | [Chapter 10](core/10-audit-traceability.md) |

## Applicable Domains | 适用领域

| Extension | Domain | Key Focus |
|---|---|---|
| SE-01 | Product Quality 产品品质 | Consumer goods, industrial products |
| SE-02 | Brand Value 品牌价值 | Corporate brands, personal brands |
| SE-03 | Individual Influence 人物影响力 | Public figures, thought leaders |
| SE-04 | City Image 城市形象 | Urban competitiveness, livability |
| SE-05 | Cultural Heritage 文化遗产与非遗 | UNESCO-aligned assessment |
| SE-06 | Restaurants & Gastronomy 餐厅与美食 | Michelin-style independent review |
| SE-07 | Intangible Assets 无形资产 | IP, goodwill, digital assets |
| SE-08 | Economy & Industry 经济与产业 | Sector rankings, economic indices |
| SE-09 | ESG & Sustainability ESG与可持续 | GRI/MSCI-aligned framework |

## Relationship with UN DCP | 与联合国DCP的关系

ICO Std 2002 aligns with the United Nations Development Cooperation Plan (UN DCP) principles by:

- Ensuring ranking methodologies support sustainable development goals (SDGs)
- Promoting inclusive and equitable assessment practices across all nations
- Requiring transparency and stakeholder participation in ranking governance
- Embedding cultural sensitivity and context-awareness in evaluation criteria

ICO Std 2002 与联合国发展合作计划（UN DCP）原则保持对齐，确保排名方法论支持可持续发展目标，促进包容和公平的评估实践，要求排名治理的透明度和利益相关方参与，并在评估标准中嵌入文化敏感性和情境感知。

## Relationship with DPP-CQ (ICO Std 2001) | 与DPP-CQ的关系

ICO Std 2002 (Ranking Methodology) is the natural complement to ICO Std 2001 (DPP-CQ):

- **DPP-CQ** provides the *data provenance and verification* infrastructure
- **ICO Std 2002** provides the *ranking methodology* that operates on verified data
- Together, they form a **complete trust chain**: verified data → validated ranking → certified result

## Directory Structure | 目录结构

```
tianji-ranking-standard/
├── README.md                 # This file
├── CHANGELOG.md              # Version history
├── LICENSE                   # Apache 2.0
├── _config.yml               # GitHub Pages config
├── core/                     # Core specification (Chapters 0-11)
│   ├── 00-preface.md
│   ├── 01-scope.md
│   ├── 02-normative-references.md
│   ├── 03-terms.md
│   ├── 04-principles.md
│   ├── 05-indicator-design.md
│   ├── 06-weighting-rules.md
│   ├── 07-data-collection.md
│   ├── 08-scoring-ranking.md
│   ├── 09-publication-transparency.md
│   ├── 10-audit-traceability.md
│   └── 11-compliance.md
├── extensions/               # Domain-specific extensions (SE-01 to SE-09)
│   ├── SE-01-products.md
│   ├── SE-02-brands.md
│   ├── SE-03-individuals.md
│   ├── SE-04-cities.md
│   ├── SE-05-cultural-heritage.md
│   ├── SE-06-restaurants.md
│   ├── SE-07-intangible-assets.md
│   ├── SE-08-economy.md
│   └── SE-09-esg.md
├── annex/                    # Informative annexes
│   ├── A-berlin-principles-mapping.md
│   ├── B-iso-alignment.md
│   └── C-examples.md
└── docs/                     # GitHub Pages documentation site
    └── index.html
```

## Getting Involved | 参与方式

- **Issues**: Technical questions and proposals → [Open an Issue](https://github.com/ICO-cloud/tianji-ranking-standard/issues)
- **Email**: Formal inquiries → info@icoun.org
- **Working Groups**: Join domain-specific working groups for SE-01 through SE-09

## License

- **Code & Schema**: [Apache License 2.0](LICENSE)
- **Documentation**: [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/)
