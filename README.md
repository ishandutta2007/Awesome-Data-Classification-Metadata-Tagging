# Awesome-Data-Classification-Metadata-Tagging

# Awesome-Data-Classification-Metadata-Tagging

**Top Data Classification Metadata Tagging (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Automated PII Discovery, Sensitive Data Tagging, Data Catalog Enrichment & Self-Hosted Classification Engines*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Data Classification & Metadata Tagging**. These tools enable organizations to automatically discover sensitive data (PII, PHI, financial records), apply classification tags, and enrich metadata catalogs—from fully managed enterprise platforms with ML-driven classifiers to open-source catalog platforms that give teams control over their data intelligence infrastructure.



**Examples** include BigID, Microsoft Purview Information Protection, Collibra Data Intelligence, Alation, Atlan, OneTrust DataDiscovery, Immuta, Securiti, Informatica CDGC, and Snowflake Tagging & Classification (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted data classification, metadata management, and open catalog infrastructure. **Critical note**: The open-source landscape has matured—**OpenMetadata** (via Collate) now offers Auto Classification with custom AI-powered recognizers and a feedback loop , while **Data Boar** provides a focused compliance-oriented scanner . **Apache Gravitino** offers federated metadata cataloging . No open-source project matches BigID's ML depth or Collibra's governance workflows out of the box, but for core classification and catalog enrichment, the open-source options are production-capable.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[BigID](https://bigid.com/)**

  **Data intelligence and classification platform** with ML-driven PII discovery. **Pricing**: **Quote-only**—"Pricing available upon request"; no public tiers, no free version listed . **Free tier**: None. **Best for**: enterprises needing deep ML-based discovery across structured and unstructured data—**trade-off**: enterprise sales process; no self-serve evaluation.



- **[Microsoft Purview Information Protection](https://www.microsoft.com/en-us/security/business/microsoft-purview)**

  **Sensitivity labeling and classification** across Microsoft 365 and hybrid environments. **Pricing**: Requires **M365 E5 Compliance add-on ($12/user/month)** or full E5 ($57/user/month) for complete functionality . **Free tier**: Basic labels on E3. **Best for**: Microsoft 365 enterprises needing classification integrated with DLP and information protection—**trade-off**: licensing cost; Microsoft ecosystem focus.



- **[Collibra Data Intelligence](https://www.collibra.com/)**

  **Data catalog and governance** with **Unified Data Classification (UDC)**. UDC uses **rule-based classification** (not ML) for transparency and flexibility; automatic classification via Edge keeps data within your network—samples are cached locally, not transferred to Collibra . **Pricing**: Quote-only; enterprise contracts. **Free tier**: None. **Best for**: enterprises wanting transparent, rule-based classification with governance workflows—**trade-off**: rule-based approach requires manual data class definition; enterprise pricing.



- **[Alation](https://www.alation.com/)**

  **Data catalog** with classification and sensitivity fields surfaced on data products. Catalog fields (Picker type) on tables and columns sync to data product pages for visibility into classification and domain . **Pricing**: Quote-only. **Free tier**: None. **Best for**: organizations wanting catalog-centric classification visibility—**trade-off**: classification is field-based, not ML-driven discovery.



- **[Atlan](https://atlan.com/)**

  **Data catalog** with **Tagging & Classification** for identifying and monitoring sensitive data with custom tags . **Pricing**: Quote-only. **Free tier**: None. **Best for**: teams wanting a modern catalog with flexible tagging—**trade-off**: classification depth varies by integration.



- **[OneTrust DataDiscovery](https://www.onetrust.com/)**

  **Data discovery and classification** with **Microsoft Purview integration**. Synchronizes file classifications from Purview Information Protection tags; two-way classification between Microsoft Purview and OneTrust catalog; applies regulatory classifications and data policies . **Pricing**: Quote-only. **Free tier**: None. **Best for**: privacy teams needing discovery synced with Microsoft 365 classifications—**trade-off**: integration-centric; best for Microsoft-heavy environments.



- **[Immuta](https://www.immuta.com/)**

  **Data security platform** with **two-phase classification**: **Identification** (entity tags by content pattern) and **Classification** (contextual risk tags using frameworks). Classification tags consider neighboring columns—a procedure code becomes PHI only when patient identity is detected in other columns . **Pricing**: Quote-only. **Free tier**: None. **Best for**: teams needing contextual, framework-based classification for policy enforcement—**trade-off**: enterprise pricing; ABAC focus.



- **[Securiti](https://securiti.ai/)**

  **Data security posture management (DSPM)** with discovery and classification. Automatically discovers cloud-native, shadow, and dark data; classifies sensitive, regulated, or custom data using AI and contextual intelligence; auto-labels files based on policies . **Pricing**: Quote-only. **Free tier**: None. **Best for**: multi-cloud environments needing DSPM with classification—**trade-off**: broader DSPM platform; classification is one module.



- **[Informatica CDGC](https://www.informatica.com/)**

  **Cloud Data Governance and Catalog** with **CLAIRE AI** classification. **200+ predefined data classifications** by default; users choose CLAIRE-generated classifications, rule-based classifications, or both; metadata ingested into catalog then classified . **Pricing**: Quote-only. **Free tier**: None. **Best for**: Informatica customers wanting AI-assisted classification within their governance platform—**trade-off**: tied to Informatica ecosystem.



- **[Snowflake Tagging & Classification](https://www.snowflake.com/)**

  **Native classification** via `SYSTEM$CLASSIFY_SCHEMA`. Schedules tables for classification; samples up to 10,000 rows; **`auto_tag: true`** sets recommended system tags on columns; **`ai_mode: true`** uses LLMs for additional semantic categories (billed under `AI_SENSITIVE_DATA_CLASSIFICATION`) . **Pricing**: Included with Snowflake; AI mode billed separately. **Free tier**: Trial credits. **Best for**: Snowflake customers wanting native PII classification without external tools—**trade-off**: Snowflake-only; parallel classification can exhaust warehouse resources .



## Open-Source GitHub Projects



- **[OpenMetadata (Collate)](https://github.com/open-metadata/OpenMetadata)**

  **Open-source metadata platform with Auto Classification** (Apache-2.0) — **the most complete open-source data classification and catalog platform** found in this research, with **Collate** adding AI-powered recognizers . **Features**: **Auto Classification Metadata Agent** automatically tags PII-sensitive data; **Collate 1.12** adds **custom AI-powered recognizers** using regex patterns, column names, and data content scanning; **feedback loop** lets users report false positives with explanations, improving model accuracy . **Column Bulk Operations** aggregate identical column names across all asset types to set descriptions, tags, and glossary terms simultaneously—also detects inconsistencies where the same column has different definitions . **Data Quality Test Library** for reusable parameterized SQL-based tests; **Human & AI Audit Logs** with six-month retention; **ODCS 3.1 and OpenLineage support** for interoperability . **Tech stack**: Java, React, PostgreSQL/MySQL. **Deploy**: Self-hosted (Docker, Kubernetes) or Collate Cloud. **Trade-off**: **Auto Classification with custom recognizers is a Collate (commercial) feature**—the open-source version has the base Auto Classification agent but not the custom AI recognizer loop. **Best for**: organizations wanting a self-hosted metadata catalog with PII classification and bulk tag management—especially those already using OpenMetadata for cataloging.



- **[Data Boar](https://pypi.org/project/data-boar/)**

  **Compliance-oriented data discovery and classification scanner** (PyPI package) — **the most focused open-source tool for regulatory-driven data inventory** . **Features**: **Multilingual and legacy encoding support**; **compressed file scanning** (zip, tar, gz, 7z); **content-type detection** for renamed files (magic bytes reveal real format even if extension is misleading); **plain-text reads with configurable character budget** so the engine sees real structure before deciding; **hard pattern hits** (IDs, payment data, strong PII) stay decisive for triage; **jurisdiction hints** (DPO-oriented notes, not legal conclusions); **US health sector inventory limits** supported . **Outputs**: Excel reports, briefing-ready leadership priorities, audit evidence . **Tech stack**: Python (Docker Hub: `fabioleitao/data_boar`). **Deploy**: `pip install data-boar`; CLI, dashboard, or API. **Trade-off**: **Inventory and triage only**—it finds where sensitive data may live and assigns technical severity; it does not enforce access policies or automate remediation. **Best for**: privacy teams and compliance consultants needing evidence-first data discovery for audits (LGPD, ISO 27701, SOC 2)—especially those preparing for regulator requests or DLP rollouts .



- **[Apache Gravitino](https://github.com/apache/gravitino)**

  **Universal catalog for data and AI** (Apache-2.0) — **the most ambitious open-source metadata federation project**, providing a single source of truth for multi-regional data . **Features**: **Geo-distributed architecture** for global metadata access; **unified data and AI asset management**; **centralized security and data access management**; simplified metadata management with a UI . **Tech stack**: Java. **Deploy**: Self-hosted. **Trade-off**: **Catalog federation, not classification**—it unifies metadata from existing catalogs but does not perform PII discovery or automated tagging itself. **Best for**: organizations with heterogeneous metadata sources wanting a federated catalog layer before adding classification.



- **[ACCESS (Automated Cataloging and Classification Engine)](https://github.com/nicolacanzonieri/access)**

  **Python-based document cataloging and classification engine** (license per repo) — **an early-stage project for automated document tagging** . **Features**: **SQLite-based metadata persistence**; **automatic tagging** via custom NLP pipeline (tokenization, cleaning, lemmatization) with **TF-IDF scoring** for tag relevance; **tag-based search** (planned); CLI (planned); unique document storage via UUIDs . **Tech stack**: Python, SQLite. **Deploy**: Local Python application. **Trade-off**: **Incomplete project**—"The project is still uncomplete and need some works before final release." Tag-based search and CLI are planned, not shipped . **Best for**: developers wanting a reference implementation for TF-IDF-based document classification—not production-ready.



### Additional Strong Open-Source Options



- **Flowfile** — Open-source data platform with visual pipeline builder and **data catalog with Delta Lake storage, version history, and lineage tracking** (PyPI package) . **Note**: **Catalog and lineage, not PII classification**—it provides metadata management but not automated sensitive data discovery. **Best for**: teams wanting a self-hosted data catalog with pipeline integration.

- **No mature open-source PII classification engine exists beyond OpenMetadata's Collate add-on and Data Boar.** The category is dominated by proprietary vendors with ML-driven discovery and governance workflows. Open-source options provide catalog foundations and focused scanners, but not full classification platforms.



**Frameworks for building custom systems**: Combine **OpenMetadata** for catalog and base Auto Classification with **Data Boar** for compliance-oriented PII scanning and **Apache Gravitino** for metadata federation—creating a limited open-source classification stack. **None of these match BigID's ML depth or Collibra's governance workflows.**



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Data classification platforms handling PII and regulated data must comply with data protection regulations (GDPR, HIPAA, CCPA, etc.) and implement appropriate access controls for classification metadata and scan results.

- **The "ML-driven discovery" vs. "rule-based classification" vs. "contextual classification" vs. "compliance scanner" vs. "catalog enrichment" distinction is critical.** **BigID and Securiti** use **ML-driven discovery**—they identify sensitive data across structured and unstructured sources . **Collibra UDC** is **rule-based**—transparent and flexible, but requires manual data class definition . **Immuta** is **contextual**—classification considers neighboring columns, not just individual patterns . **Data Boar** is a **compliance scanner**—it inventories and triages but does not enforce policies . **OpenMetadata** is **catalog enrichment**—it tags assets in a metadata catalog . **Choose based on whether you need ML discovery, transparent rules, contextual risk, compliance evidence, or catalog tagging.**

- **Collibra's UDC deliberately avoids ML**—it uses classification rules for transparency and flexibility. **The trade-off**: you define data classes and rules manually; there is no automated ML discovery. **For regulated industries prioritizing auditability over automation, this is a feature.**

- **Immuta's two-phase classification is genuinely different.** Entity tags identify patterns; classification tags assess risk **with context from neighboring columns**—a procedure code becomes PHI only when patient identity is detected elsewhere . **This contextual approach reduces false positives and captures toxic joins** that column-level tagging misses.

- **Snowflake's AI mode uses LLMs for semantic categories** beyond standard classification—billed under `AI_SENSITIVE_DATA_CLASSIFICATION` . **The trade-off**: parallel classification can exhaust warehouse resources; plan warehouse sizing before classifying large schemas .

- **Data Boar is the most focused open-source compliance scanner.** It handles multilingual encodings, compressed archives, and misleading file extensions—and produces briefing-ready reports for audits . **The trade-off**: inventory and triage only—no policy enforcement or automated remediation.

- **OpenMetadata's custom AI recognizers are a Collate feature**, not fully open source. The open-source version has the base Auto Classification agent but lacks the custom recognizer feedback loop . **For open-source users, base PII tagging is available; custom recognizers require Collate.**

- **Pricing opacity is universal** across BigID, Microsoft Purview (E5 licensing), Collibra, Alation, Atlan, OneTrust, Immuta, Securiti, and Informatica. All require sales contact or licensing commitment. **Validate with direct vendor conversations against your data source count and classification requirements.**

- Self-hosted open-source solutions require proper infrastructure (PostgreSQL for OpenMetadata, Python for Data Boar), security hardening, and ongoing maintenance. **Classification tools scan sensitive data**—ensure your deployment meets your organization's privacy and compliance requirements before connecting production data sources.



---



**Made for data governance teams, privacy officers, and organizations building transparent data classification solutions.**

Let's make Data Classification & Metadata Tagging more open, data-driven, and privacy-aware.
