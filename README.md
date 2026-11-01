# Awesome-Data-Classification-Metadata-Tagging

**Top Data Classification & Metadata Tagging (SaaS & Open-Source) 🌟 Star if you like it! 🌟**

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Automated PII Discovery, Sensitive Data Tagging, Data Catalog Enrichment & Self-Hosted Classification Engines*

**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Data Classification & Metadata Tagging**. These tools enable organizations to automatically discover sensitive data (PII, PHI, financial records), apply classification tags, and enrich metadata catalogs—from fully managed enterprise platforms with ML-driven classifiers to open-source catalog platforms that give teams control over their data intelligence infrastructure.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

---

## Sector Overview & Market Dynamics

The global data classification and metadata tagging market is estimated at **$2.28 billion to $3.2 billion in 2026**, projected to surge past **$6 billion to $11 billion by 2030–2031** (growing at a 21%–34% CAGR) powered by enterprise AI adoption, regulatory compliance mandates (GDPR, CCPA, HIPAA), and exploding unstructured data volumes. The sector exhibits **moderate fragmentation with high concentration among cloud hyperscalers**: while cloud giants and established governance platforms (Microsoft, Snowflake, Informatica, Collibra) capture dominant platform spend, specialized vendors and AI-first startups (BigID, Securiti, Immuta, Atlan) continue to drive specialized innovation in DSPM, automated PII discovery, and contextual classification.

---

## SaaS/Hosted Platforms

The table below lists leading commercial SaaS and hosted platforms, sorted descending by company size (market capitalization / valuation):

| Platform | Company Size (Valuation / Revenue) | Starting Tier Pricing | Free Tier / Trial Limits | Core Focus & Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Microsoft Purview Information Protection](https://www.microsoft.com/en-us/security/business/microsoft-purview)** | ~$3.88T Market Cap | **$12/user/month** (M365 E5 Compliance add-on; requires base E3 license) or **$57/user/month** (full Microsoft 365 E5) | **90-day free trial** with up to **25 user licenses** for Microsoft Purview Suite; basic manual sensitivity labels included in E3 | Sensitivity labeling and automated PII/sensitive data classification deeply integrated across Microsoft 365, SharePoint, Exchange, and hybrid cloud environments. |
| **[Snowflake Tagging & Classification](https://www.snowflake.com/)** | ~$110B–$116B Market Cap | **$2.00 per credit** (Standard Edition on-demand list price; native schema classification `SYSTEM$CLASSIFY_SCHEMA` included in warehouse runtime) | **30-day free trial** with **$400 in usage credits** (whichever expires first) | Native SQL-driven sensitive data classification and tagging directly inside Snowflake; samples up to 10k rows and supports AI-assisted semantic classification (`ai_mode: true`). |
| **[Informatica CDGC](https://www.informatica.com/)** | ~$7.6B Valuation (Acquired by Salesforce) | **~$131,760/year** (AWS Marketplace entry base bundle starting around 120 IPUs / ~$10,980/month) | **30-day free trial** for IDMC cloud services (guided PoC sandbox required for full CDGC governance module) | Cloud Data Governance and Catalog powered by CLAIRE AI; delivers 200+ predefined data classifications combining rule-based heuristics and automated machine learning. |
| **[Collibra Data Intelligence](https://www.collibra.com/)** | $5.25B Valuation (~$150M–$250M ARR) | **~$170,000/year** (AWS Marketplace platform base subscription floor / ~$14,166/month) | **No free tier**; interactive self-guided web demo and guided sandbox PoC available upon request | Enterprise data catalog and governance platform offering Unified Data Classification (UDC) using rule-based classification executed via edge agents without data egress. |
| **[OneTrust DataDiscovery](https://www.onetrust.com/)** | $4.5B Valuation (~$500M+ ARR) | **~$10,000/year** (Starting entry package for targeted discovery modules / ~$833/month) | **14-day free trial** for select platform modules; interactive click-through guided tours available | Automated data discovery, regulatory mapping, and classification engine with bi-directional synchronization to Microsoft Purview Information Protection tags. |
| **[Alation](https://www.alation.com/)** | $1.7B Valuation (~$109M+ ARR) | **$60,000/year** (AWS Marketplace baseline 12-month contract entry floor / ~$5,000/month) | **No free tier**; sales-assisted Proof of Concept (PoC) under Trial Use Agreement and interactive tours | Enterprise data intelligence catalog featuring classification, sensitivity tags, and domain ownership surfacing directly across data products, tables, and columns. |
| **[Securiti](https://securiti.ai/)** | $1.725B Valuation (Acquired by Veeam, ~$75M–$100M ARR) | **~$100,000/year** (AWS Marketplace entry annual commitment for Data Command Center / ~$8,333/month) | **No permanent free tier**; interactive module tours and free access to Securiti Education hands-on labs/academies | Data Command Center providing AI-powered DSPM, sensitive/dark data discovery, contextual intelligence, and automated policy-driven file labeling across multi-cloud environments. |
| **[BigID](https://bigid.com/)** | $1.0B–$1.25B Valuation (~$100M ARR) | **~$25,000/year** (Entry-level deployment floor; cloud foundation marketplace bundles typically list around $175,000/year) | **No free tier**; self-guided interactive product tours and scheduled live vendor data risk assessments | Data intelligence platform featuring deep ML-driven PII/sensitive data discovery, contextual correlation, and automated catalog classification across structured and unstructured data. |
| **[Immuta](https://www.immuta.com/)** | $1.0B Valuation (~$50M–$100M ARR) | **~$96,000/year** (AWS Marketplace standard annual commitment based on ~960 Immuta Units / ~$8,000/month) | **No free tier**; personalized enterprise live demos and scoped technical sandbox PoC evaluations | Contextual data security and access control platform with two-phase classification (pattern identification + neighboring-column contextual risk assessment for toxic join prevention). |
| **[Atlan](https://atlan.com/)** | $750M Valuation (~$50M–$90M ARR) | **~$120,000/year** (Enterprise marketplace annual contract floor / ~$10,000/month billed annually) | **No free tier**; self-guided interactive product tours and customized guided demo PoC environments | Modern collaborative active metadata platform featuring automated tagging, sensitive data classification, and end-to-end data lineage visualization. |

---

## Open-Source GitHub Projects

The table below lists open-source projects for data classification, metadata management, cataloging, and PII discovery, sorted descending by GitHub star counts. Each project includes a live star badge linking directly to its GitHub Stargazers page:

| Project | Stars | Tech Stack | License | Core Focus & Description |
| :--- | :--- | :--- | :--- | :--- |
| **[OpenMetadata](https://github.com/open-metadata/OpenMetadata)** | [![Stars](https://img.shields.io/github/stars/open-metadata/OpenMetadata?style=social&color=white)](https://github.com/open-metadata/OpenMetadata/stargazers) | Java, Python, React | Apache-2.0 | Unified metadata management platform featuring native Auto Classification agents for automated PII discovery, column-level sensitive tagging, schema lineage, and data quality testing. |
| **[DataHub](https://github.com/datahub-project/datahub)** | [![Stars](https://img.shields.io/github/stars/datahub-project/datahub?style=social&color=white)](https://github.com/datahub-project/datahub/stargazers) | Java, Python, React | Apache-2.0 | Extensible metadata catalog built for modern data stacks; provides automated metadata ingestion, dataset documentation, tag propagation, glossary terms, and governance workflows. |
| **[Presidio](https://github.com/microsoft/presidio)** | [![Stars](https://img.shields.io/github/stars/microsoft/presidio?style=social&color=white)](https://github.com/microsoft/presidio/stargazers) | Python, C# | MIT | Microsoft's open-source contextual PII detection and anonymization SDK; features customizable NER recognizers, rule-based engines, and redaction pipelines for text and structured data. |
| **[Amundsen](https://github.com/amundsen-io/amundsen)** | [![Stars](https://img.shields.io/github/stars/amundsen-io/amundsen?style=social&color=white)](https://github.com/amundsen-io/amundsen/stargazers) | Python, TypeScript | Apache-2.0 | Data discovery and metadata engine created at Lyft; indexes data assets, surfaces table/column descriptions, and enables metadata tagging for search and compliance. |
| **[Apache Gravitino](https://github.com/apache/gravitino)** | [![Stars](https://img.shields.io/github/stars/apache/gravitino?style=social&color=white)](https://github.com/apache/gravitino/stargazers) | Java, Python | Apache-2.0 | High-performance, geo-distributed federated metadata lakehouse catalog providing unified metadata, access control, and tag-based governance across multi-cloud engines. |
| **[Apache Atlas](https://github.com/apache/atlas)** | [![Stars](https://img.shields.io/github/stars/apache/atlas?style=social&color=white)](https://github.com/apache/atlas/stargazers) | Java | Apache-2.0 | Foundational enterprise governance and metadata framework for Hadoop and cloud ecosystems; features classification classification hierarchies, automated tag propagation via lineage, and security integration with Apache Ranger. |
| **[Data Profiler](https://github.com/capitalone/Data-Profiler)** | [![Stars](https://img.shields.io/github/stars/capitalone/Data-Profiler?style=social&color=white)](https://github.com/capitalone/Data-Profiler/stargazers) | Python | Apache-2.0 | Capital One's machine-learning-powered data profiling and sensitive record detection library; identifies schema schemas, statistics, and sensitive PII types across tabular, JSON, and unstructured text files. |
| **[ODD Platform](https://github.com/opendatadiscovery/odd-platform)** | [![Stars](https://img.shields.io/github/stars/opendatadiscovery/odd-platform?style=social&color=white)](https://github.com/opendatadiscovery/odd-platform/stargazers) | Java, TypeScript | Apache-2.0 | Open-source data discovery and observational governance platform supporting automated cataloging, end-to-end data lineage, SLA monitoring, and sensitive data tagging. |
| **[Data Boar](https://github.com/DataBoar/data-boar)** | [![Stars](https://img.shields.io/github/stars/DataBoar/data-boar?style=social&color=white)](https://github.com/DataBoar/data-boar/stargazers) | Python | BSD-3-Clause | Compliance-oriented scanner designed for forensic-grade PII and sensitive data discovery; features multilingual encoding support, archive inspection (zip/tar/7z), magic byte verification, and audit report generation. |
| **[ACCESS](https://github.com/nicolacanzonieri/access)** | [![Stars](https://img.shields.io/github/stars/nicolacanzonieri/access?style=social&color=white)](https://github.com/nicolacanzonieri/access/stargazers) | Python | GPL-3.0 | Automated Cataloging and Classification Engine; reference project using NLP pipelines and TF-IDF scoring for document categorization and automated metadata tagging. |

---

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (maintain tabular structure and star count sorting).
3. Include: name, link, specific pricing/limits, license (for open-source), and star badge.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

---

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Data classification platforms handling PII and regulated data must comply with data protection regulations (GDPR, HIPAA, CCPA, etc.) and implement appropriate access controls for classification metadata and scan results.
- **The "ML-driven discovery" vs. "rule-based classification" vs. "contextual classification" vs. "compliance scanner" vs. "catalog enrichment" distinction is critical.** **BigID and Securiti** use ML-driven discovery across structured and unstructured sources. **Collibra UDC** is rule-based for transparent auditability. **Immuta** is contextual, assessing risk based on neighboring columns to prevent toxic joins. **Data Boar** and **Capital One Data Profiler** focus on forensic scanning and profiling. **OpenMetadata** and **DataHub** focus on catalog enrichment and governance orchestration.
- Enterprise SaaS pricing varies based on contract volume, connector counts, and cloud marketplace private offers. Listed prices reflect public baseline floors and standard pricing tiers.
- Self-hosted open-source solutions require proper infrastructure, security hardening, and ongoing maintenance. Classification tools scan sensitive data—ensure your deployment meets your organization's privacy and compliance requirements before connecting production data sources.

---

**Made for data governance teams, privacy officers, and organizations building transparent data classification solutions.**
