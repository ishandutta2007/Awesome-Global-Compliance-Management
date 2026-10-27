# Awesome-Global-Compliance-Management

# Top Global Compliance Management Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Regulatory Change Tracking, Control Mapping & Multi-Jurisdictional Compliance*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Global Compliance Management**. These tools enable organizations to monitor regulatory changes across jurisdictions, map requirements to internal controls, manage policy lifecycles, and maintain audit-ready evidence—ensuring compliance with frameworks like GDPR, ISO 27001, SOC 2, NIS2, DORA, and industry-specific regulations.

**Examples** include Workday Global Compliance, Diligent, MetricStream, Archer, Workiva, SAI360, OneTrust, LogicGate, Compliance.ai, and RadarFirst (the category leaders).

**Open-source emphasis**: Global Compliance Management is a domain where open-source tooling is **emerging but fragmented**. The strongest active projects are **Cairn** (self-hosted GRC with multi-framework compliance and regulatory incident clocks) and **Comp AI** (SOC 2, ISO 27001, HIPAA, GDPR automation). For regulatory change monitoring specifically, **GRCX** provides a focused radar for financial services regulators. Other projects address compliance-as-code, policy enforcement, or framework-specific automation. No single open-source platform matches the full global compliance breadth of OneTrust or MetricStream, but Cairn and Comp AI provide credible self-hosted foundations.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Workday Global Compliance](https://www.workday.com/)**  
  Compliance capabilities within Workday's financial and HCM suites, covering SOX compliance, audit trails, policy management, and regulatory reporting integrated with financial and workforce data.

- **[Diligent](https://www.diligent.com/)**  
  Diligent One Platform integrates governance, risk, and compliance with modules for board management, risk assessment, internal controls, audit management, and compliance tracking; provides analytics and customizable dashboards for transparency in managing risks and meeting compliance obligations.

- **[MetricStream](https://www.metricstream.com/)**  
  AI-powered GRC platform recognized as a Category Leader across all seven GRC categories by Chartis Research; features continuous risk sensing, AI assistants for compliance workflows, autonomous evidence gathering, and regulatory change management.

- **[Archer](https://www.archerirm.com/)**  
  Enterprise GRC platform with integrated risk register, regulatory compliance mapping, third-party risk governance, and audit-ready evidence with timestamped trails; serves 1,500+ customers across 48 countries.

- **[Workiva](https://www.workiva.com/)**  
  Financial compliance and SEC reporting platform with ICFR and SOX compliance capabilities; provides a single source of truth with data traceability and streamlined audit interactions.

- **[SAI360](https://www.sai360.com/)**  
  GRC platform with regulatory change management, policy management, and compliance training integration for regulated industries.

- **[OneTrust](https://www.onetrust.com/)**  
  GRC platform named a Leader in the IDC MarketScape for Worldwide GRC Software 2025; unifies privacy, AI governance, risk management, and third-party monitoring with automated processes and AI-powered data governance; trusted by 14,000+ global brands.

- **[LogicGate](https://www.logicgate.ai/)**  
  AI GRC platform with GRC Agents for ERM, TPRM, AI Governance, and Business Continuity Management; features Automated Control Testing and upcoming MCP Server Access for natural language Risk Cloud queries.

- **[Compliance.ai](https://www.compliance.ai/)**  
  Regulatory intelligence platform that aggregates and classifies regulatory content from thousands of sources, mapping changes to organizational policies and controls.

- **[RadarFirst](https://www.radarfirst.com/)**  
  Incident response and compliance platform with automated risk assessment for privacy and security incidents, including regulatory notification decisioning.

## Open-Source GitHub Projects

- **[Cairn](https://github.com/frousselet/cairn)**  
  Self-hosted GRC platform (GNU AGPL) covering governance (ISO 27001 clause 4 context), assets with CIA valuation, risk management using ISO 27005 and EBIOS RM, **compliance frameworks with audits and a nonconformity register**, and incidents with sealed evidence and **statutory notification clocks (GDPR, NIS2, DORA)** . Features inter-framework mappings so requirements can be reused across standards, a public Trust Center page, and steering dashboards with PDF/DOCX/PPTX/XLSX reports. Every feature is API-accessible via REST and built-in MCP server; optional AI (off by default) supports Mistral, OpenAI, Claude, or local Ollama. Single-container Docker deployment. **Governance is enforced through permissioned state transitions that leave audit trails**—not status dropdowns . **The most comprehensive open-source global compliance foundation** for organizations needing multi-framework tracking with regulatory incident management.

- **[Comp AI (Community Edition)](https://github.com/trycompai/comp)**  
  Free, open-source compliance automation platform (AGPLv3) for **SOC 2, ISO 27001, HIPAA, and GDPR**; automates evidence collection, policy management, and control implementation while keeping data on your infrastructure . Community Edition is self-hosted; Comp AI Cloud is a separate managed product with additional capabilities. **Strongest for SaaS companies pursuing standard certifications**, with automated evidence collection reducing audit preparation burden.

- **[GRCX](https://github.com/grcx-dev/grcx)**  
  Open-source **regulatory radar for financial services compliance teams**; monitors publications from **BoE, FCA, MAS, SEC, and ESMA** via IMAP/RSS/HTTP feeds, maps each new publication to your control frameworks using an LLM, assesses severity, and surfaces a prioritized queue . Built-in frameworks include ISO 27001, FCA SYSC, MAS TRM, NIST CSF, BCBS 239, and SOC 2; custom frameworks via YAML. Writes every detection and assessment to a **cryptographically chained audit log (SHA-256, append-only, verifiable)**. Every assessment is subject to human override . **The only open-source regulatory change monitoring tool**—focused on financial services but the pattern is extensible.

- **[Probo](https://github.com/getprobo/probo)**  
  Self-hostable GRC platform (ISC licensed) for SOC 2, GDPR, and ISO 27001; covers risk registers, control tracking, vendor risk, data privacy (DPIA/TIA), access reviews, audit programs, and document approval workflows . Exposes 270+ MCP tools for AI agent automation, `prb` CLI with 44+ command groups, GraphQL API, and n8n community node. Docker-deployable with policy-based RBAC and immutable audit logs. **Strong for engineering-led compliance automation**, though less focused on multi-jurisdictional regulatory change tracking than Cairn or GRCX.

- **[Openlane](https://github.com/theopenlane/core)**  
  Open-source compliance automation alternative to Vanta, Drata, and Secureframe (Apache-2.0); supports **SOC 2, GDPR, ISO 27001, NIST 800-53, and more** . Security features like SSO and 2FA enforcement ship with every module rather than sitting behind an enterprise tier. Runs on Go, PostgreSQL, Redis, and OpenFGA without requiring a pile of SaaS dependencies. **Fully permissive licensing** (Apache-2.0) distinguishes it from AGPL alternatives.

- **[Evidentia](https://github.com/Polycentric-Labs/evidentia)**  
  Open-source GRC platform built for **FedRAMP High, CMMC Level 2, and EU sovereign-cloud deployments**; uses **OSCAL** (NIST's open standard) for inputs and outputs, ensuring data portability . Features 89 bundled frameworks, CI-native gap analysis via GitHub Action that runs on every PR and blocks merge on compliance regression, AI-optional risk statement generation via LiteLLM, and GPG/Sigstore evidence signing . **Library-first architecture** (Python library → CLI → REST API) supports embedding compliance checks into engineering workflows.

- **[Conformiti](https://github.com/dboudreau00/Conformiti)**  
  Open-source GRC compliance tool for SaaS products managing the full audit lifecycle; ships with **SOC 2, ISO 27001:2022, and PCI DSS v4.0.1** control libraries (217 controls), evidence folder trees segregated by control, role-based document access, review scheduling with email reminders (IMAP/POP3 + SMTP or Amazon SES), analytics dashboards, risk register with CSV/XLSX import, and **immutable audit trail with in-app viewer** . Django/React stack with Docker deployment. **Strong for organizations running multiple concurrent audits** with document-heavy evidence workflows.

### Additional Strong Open-Source Options

- **ARKA Protocol Core** — Open-source compliance engine that transforms regulatory requirements into executable, auditable logic using a declarative DSL; features multi-chain audit trail anchoring (Ethereum, Solana, Cosmos) and plugin architecture; Apache-2.0 licensed . **Rule-engine focused**—for building compliant applications rather than managing organizational compliance programs.
- **Noreli North Advanced Compliance** — Comprehensive GRC built natively on Frappe/ERPNext; features control management with COSO alignment, risk register with inherent/residual scoring, knowledge graph for control-risk relationships, and optional AI for anomaly detection; supports SOX 404, COSO, COBIT 2019, ISO 27001, GDPR, HIPAA, and PCI-DSS . **Best for organizations already on ERPNext** seeking integrated compliance workflows.
- **Open Policy Agent (OPA)** — Policy engine for cloud-native environments using Rego declarative language; enforces compliance policies across Kubernetes, Istio, Envoy, and infrastructure . **Policy-as-code focused**—for runtime enforcement rather than compliance management.
- **Compliance Masonry** — CLI tool for constructing System Security Plans (SSP) and compliance documentation from machine-readable OpenControl YAML files; supports NIST 800-53 and multi-framework mappings . **Documentation-generation focused**.

**Frameworks for building custom systems**: Combine **Cairn** for multi-framework compliance tracking with regulatory incident clocks and audit trails, **GRCX** for regulatory change monitoring (financial services regulators), **Comp AI** or **Openlane** for SOC 2/ISO 27001 automation, and **Evidentia** for CI-native compliance-as-code with OSCAL portability in a self-hosted global compliance management stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Global compliance platforms handling regulatory data and audit evidence must comply with applicable regulations in every jurisdiction of operation; evidence integrity and audit trails are critical for regulatory defensibility.
- **Open-source global compliance remains fragmented**—Cairn provides the strongest multi-framework foundation with regulatory incident management, GRCX addresses regulatory change monitoring for financial services, and Comp AI/Openlane focus on standard certification automation. No single open-source platform matches OneTrust or MetricStream's full breadth across privacy, ethics, third-party risk, and multi-jurisdictional regulatory intelligence. Organizations requiring comprehensive global compliance should evaluate commercial platforms or plan for integration across multiple open-source components.
- Verify license terms for commercial use; Cairn uses GNU AGPL , Comp AI uses AGPLv3 , GRCX is open-source , Probo uses ISC , Openlane uses Apache-2.0 , and Evidentia is open-source .

---

**Made for compliance officers, regulatory affairs teams, GRC analysts, and legal operations leaders.**  
Let's make global compliance management more open, auditable, and jurisdiction-aware.
