# Awesome EU AI Act [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, frameworks, standards, and resources for EU AI Act compliance and AI governance.

The [EU AI Act](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689) entered into force on 1 August 2024. High-risk AI systems (Annex III) must comply by August 2026 (subject to the [Digital Omnibus](https://digital-strategy.ec.europa.eu/en/policies/digital-omnibus) backstop). This list helps engineers, data scientists, compliance officers, and legal teams navigate the ecosystem.

**Contributing:** Pull requests welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Contents

- [Developer Tools & SDKs](#developer-tools--sdks)
- [Assessment & Classification](#assessment--classification)
- [AI Governance Platforms](#ai-governance-platforms)
- [Monitoring & Observability](#monitoring--observability)
- [Testing & Red-Teaming](#testing--red-teaming)
- [Evidence Formats & Frameworks](#evidence-formats--frameworks)
- [Standards](#standards)
- [Regulatory Documents](#regulatory-documents)
- [AESIA Resources (Spain)](#aesia-resources-spain)
- [Educational Resources](#educational-resources)
- [Communities](#communities)
- [News & Newsletters](#news--newsletters)

---

## Developer Tools & SDKs

*Tools that integrate into ML pipelines and generate compliance evidence.*

- **[Venturalitica SDK](https://github.com/Venturalitica/venturalitica-sdk)** — Open-source Python SDK for EU AI Act and ISO 42001 compliance evidence. Generates OSCAL policies, CycloneDX ML BOM, bias audits, and Annex IV documentation. `pip install venturalitica`
- **[Giskard](https://github.com/Giskard-AI/giskard)** — Open-source LLM testing and red-teaming framework with vulnerability scanning. CLI-first, integrates with HuggingFace and LangChain.
- **[VerifyWise](https://github.com/verifywise/verifywise)** — Open-source AI governance platform (BSL 1.1). Self-hosted compliance tracking for high-risk AI systems.
- **[Evidently AI](https://github.com/evidentlyai/evidently)** — ML monitoring and evaluation framework. 7K+ stars, 35M+ downloads. No compliance mapping, but strong data quality and drift detection (Art. 10 relevant).
- **[IBM OpenPages](https://www.ibm.com/products/openpages)** — GRC platform with AI governance module. Enterprise-grade, watsonx.governance integration.

## Assessment & Classification

*Tools to classify AI systems by risk level and assess compliance gaps.*

- **[Venturalitica /assess](https://venturalitica.com/assess)** — Free dual-plane assessment: ISO 42001 organizational maturity (Score A) + EU AI Act product compliance (Score B). Generates AIMS Starting Point Report.
- **[Modulos Risk Agent](https://modulos.ai)** — Interactive AI risk assessment with EUR quantification. No login required. ISO 42001 certified (first, via CertX).
- **[Trail-ML](https://trail-ml.com)** — EU AI Act compliance platform. ETH Zurich spin-off. Focus on risk classification and technical documentation.
- **[Holistic AI](https://holisticai.com)** — AI risk governance platform. Comprehensive auditing and mitigation across 8 risk domains.
- **[Enkrypt AI](https://enkryptai.com)** — AI risk classification and red-teaming for LLMs.

## AI Governance Platforms

*Enterprise platforms for AI risk management and governance.*

- **[Credo AI](https://credo.ai)** — AI governance platform. Policy enforcement, model registry, audit trails. SOC 2 Type II certified.
- **[Arthur AI](https://arthur.ai)** — ML observability and AI governance. Agent discovery and governance for agentic AI. SOC 2 Type II.
- **[Fiddler AI](https://fiddler.ai)** — ML monitoring and explainability. Amazon SageMaker integration. $30M Series C (2025).
- **[Saidot](https://saidot.com)** — AI governance knowledge graph with inherited governance data. EU AI Pact signatory.
- **[NAAIA](https://naaia.fr)** — French AI governance platform. First ISO 42001 certified in France (AFNOR). EU AI Pact signatory.
- **[Lumenova AI](https://lumenova.ai)** — AI governance and compliance platform. SOC 2 Type II.
- **[Trustible](https://trustible.com)** — AI governance and policy management.
- **[OneTrust](https://onetrust.com)** — GRC platform expanding into AI governance. $1.13B raised.
- **[Vanta](https://vanta.com)** — Automated compliance platform with AI governance modules. $504M raised.

## Monitoring & Observability

*Tools for post-deployment AI system monitoring (Art. 72 Post-Market Monitoring).*

- **[Evidently AI](https://github.com/evidentlyai/evidently)** — Data drift, model performance, and data quality monitoring. 40-lesson free course.
- **[Fiddler AI](https://fiddler.ai)** — ML monitoring, explainability, and fairness monitoring.
- **[WhyLabs](https://whylabs.ai)** — Data and ML monitoring platform.
- **[Arize AI](https://arize.com)** — ML observability platform with LLM tracing.

## Testing & Red-Teaming

*Tools for adversarial testing, robustness, and vulnerability scanning (Art. 15 Robustness).*

- **[Giskard](https://github.com/Giskard-AI/giskard)** — Automated LLM vulnerability scanning and red-teaming. 4K+ GitHub stars.
- **[DeepEval](https://github.com/confident-ai/deepeval)** — LLM evaluation framework with 14+ evaluation metrics.
- **[PyRIT](https://github.com/Azure/PyRIT)** — Microsoft's Python Risk Identification Tool for generative AI.
- **[Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai)** — UK AISI's framework for LLM safety evaluations.
- **[AI Verify](https://aiverifyfoundation.sg)** — Singapore government AI testing framework. Supports EU AI Act mappings.

## Evidence Formats & Frameworks

*Standards and formats for generating auditable compliance evidence.*

- **[OSCAL (Open Security Controls Assessment Language)](https://pages.nist.gov/OSCAL/)** — NIST standard for machine-readable compliance documentation. Native format for policy-as-code AI governance. Used by Venturalitica SDK.
- **[CycloneDX ML BOM](https://cyclonedx.org/capabilities/mlbom/)** — Machine Learning Bill of Materials standard. Documents model provenance, datasets, and dependencies (EU AI Act Annex IV.2).
- **[Model Card Toolkit](https://github.com/tensorflow/model-card-toolkit)** — Google's toolkit for generating model cards (Annex IV.3).
- **[Croissant](https://github.com/mlcommons/croissant)** — ML dataset format with provenance metadata (Art. 10 data governance).
- **[SLSA Framework](https://slsa.dev)** — Supply-chain security framework for software artifacts. Relevant for Art. 15.5 cybersecurity.

## Standards

*Technical standards relevant to EU AI Act compliance.*

### EU AI Act Harmonised Standards (JTC 21)

> **Note:** No harmonised standards are currently available (Stage 10-40 only). Organizations must comply with EU AI Act obligations regardless (Art. 40). Standards expected 2026-2027.

| Standard | Scope | Stage | EU AI Act Article |
|---|---|---|---|
| **prEN 18286** | Quality Management System for AI | Stage 40 (public consultation) | Art. 17 |
| **prEN 18228** | Risk Management | Stage 20 | Art. 9 |
| **prEN 18284** | Data Governance | Stage 10 | Art. 10 |
| **prEN 18283** | Fairness | Stage 10 | Art. 10 |
| **prEN 18229-1** | Transparency & Logging | Stage 20 | Arts. 12, 13 |
| **prEN 18229-2** | Accuracy & Robustness | Stage 20 | Art. 15 |
| **prEN 18282** | Cybersecurity | Stage 10 | Art. 15.5 |

### ISO Standards

- **[ISO 42001:2023](https://www.iso.org/standard/81230.html)** — AI Management System (AIMS). Organizational governance of AI. Complementary to EU AI Act (not a substitute).
- **[ISO/IEC 23894:2023](https://www.iso.org/standard/77304.html)** — AI Risk Management guidance.
- **[ISO/IEC 24028:2020](https://www.iso.org/standard/73920.html)** — AI Trustworthiness overview.
- **[ISO/IEC 5338:2023](https://www.iso.org/standard/81118.html)** — AI System Lifecycle Processes.

### NIST Frameworks

- **[NIST AI RMF 1.0](https://airc.nist.gov/RMF_Overview)** — AI Risk Management Framework. Governs, Map, Measure, Manage structure. US-origin but globally adopted.
- **[NIST AI RMF Playbook](https://airc.nist.gov/Docs/2)** — Practical implementation guidance.
- **[NIST SP 1270](https://airc.nist.gov/Docs/2)** — Towards a Standard for Identifying and Managing Bias in Artificial Intelligence.

## Regulatory Documents

*Official EU AI Act texts and guidance.*

- **[EU AI Act — Official Text](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689)** — Regulation (EU) 2024/1689. Official Journal, 12 July 2024.
- **[EU AI Act — Consolidated Reader-Friendly Version](https://artificialintelligenceact.eu)** — Annotated version by Future of Life Institute.
- **[AI Office — Implementation Guidance](https://digital-strategy.ec.europa.eu/en/policies/ai-office)** — European Commission AI Office resources.
- **[Digital Omnibus Proposal](https://digital-strategy.ec.europa.eu/en/policies/digital-omnibus)** — COM(2025) 836. Proposes deadline adjustments for Annex III systems.
- **[EU AI Act Annex III](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689#anx_III)** — High-risk AI system categories.
- **[EU AI Act Annex IV](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689#anx_IV)** — Technical documentation requirements.
- **[EU AI Pact](https://digital-strategy.ec.europa.eu/en/policies/ai-pact)** — Voluntary commitment for early compliance. Signatories: Modulos, Saidot, Collibra, and 100+ others.
- **[GPAI Code of Practice](https://digital-strategy.ec.europa.eu/en/policies/ai-act-general-purpose-ai)** — General Purpose AI model governance.

## AESIA Resources (Spain)

*Spanish AI Agency (Agencia Española de Supervisión de Inteligencia Artificial) guidance.*

> AESIA published 16 practical guides in December 2025 — the most comprehensive practical implementation resource available while JTC 21 standards are pending.

- **[AESIA Official Website](https://www.aesia.es)** — Spanish AI supervisory authority.
- **[AESIA Guide 04](https://www.aesia.es/guias)** — Quality Management System (Art. 17 / prEN 18286)
- **[AESIA Guide 05](https://www.aesia.es/guias)** — Risk Management System (Art. 9 / prEN 18228)
- **[AESIA Guide 07](https://www.aesia.es/guias)** — Data Governance + Fairness (Art. 10 / prEN 18284, 18283)
- **[AESIA Guide 08](https://www.aesia.es/guias)** — Transparency (Art. 13 / prEN 18229-1)
- **[AESIA Guide 09](https://www.aesia.es/guias)** — Accuracy & Performance (Art. 15 / prEN 18229-2)
- **[AESIA Guide 10](https://www.aesia.es/guias)** — Robustness (Art. 15.4 / prEN 18229-2)
- **[AESIA Guide 11](https://www.aesia.es/guias)** — Cybersecurity (Art. 15.5 / prEN 18282)
- **[AESIA Guide 12](https://www.aesia.es/guias)** — Logging & Record-keeping (Art. 12)
- **[AESIA Guide 15](https://www.aesia.es/guias)** — Technical Documentation (Art. 11, Annex IV)

## Educational Resources

*Courses, tutorials, and articles for learning EU AI Act compliance.*

### Courses

- **[ML Observability Course](https://learn.evidentlyai.com)** — Evidently AI. 40 lessons on ML monitoring and data quality. Free, no gate.
- **[MLOps Zoomcamp](https://github.com/DataTalksClub/mlops-zoomcamp)** — DataTalks.Club. Free MLOps course covering model deployment and monitoring.
- **[Andrew Ng AI for Everyone](https://www.coursera.org/learn/ai-for-everyone)** — Non-technical AI literacy. Useful for compliance officers.

### Articles & Tutorials

- **[EU AI Act Risk Classification: A Decision Tree](https://venturalitica.com/blog)** — Step-by-step classification guide with code examples.
- **[ISO 42001 for Engineers: From YAML to Certification](https://venturalitica.com/blog)** — Technical implementation guide.
- **[What is OSCAL and Why AI Governance Needs It](https://venturalitica.com/blog)** — Category-defining explanation of OSCAL for AI compliance.
- **[EU AI Act Compliance for Python Developers](https://venturalitica.com/blog)** — SDK-based tutorial with working code.

### Key Papers

- **[AI Assurance as Responsible Innovation](https://doi.org/10.1080/23299460.2023.2195395)** — Bridging the developer-regulator divide.
- **[Mapping the EU AI Act](https://arxiv.org/abs/2403.05982)** — Technical analysis of AI Act requirements. Madiega et al., 2024.
- **[NIST SP 1270: Bias in AI](https://doi.org/10.6028/NIST.SP.1270)** — Identifying and managing bias. 2022.

## Communities

*Where practitioners discuss EU AI Act compliance.*

- **[Venturalitica Discord](https://venturalitica.com/discord)** — Community for EU AI Act compliance engineers. Channels: #eu-ai-act, #iso-42001, #sdk-support.
- **[MLOps Community Slack](https://go.mlops.community/slack)** — 85K+ MLOps practitioners. Active #ai-governance channel.
- **[DataTalks.Club Slack](https://datatalks.club/slack.html)** — 50K+ data practitioners.
- **[IAPP AI Governance Community](https://iapp.org)** — Privacy and AI governance professionals.
- **[LinkedIn: EU AI Act Compliance](https://www.linkedin.com/groups/)** — Multiple groups focused on EU AI Act implementation.

## News & Newsletters

*Stay updated on EU AI Act developments.*

- **[AI Office Newsletter](https://digital-strategy.ec.europa.eu/en/subscribe-newsletter)** — Official European Commission AI Office updates.
- **[AI Supremacy Newsletter](https://www.getrevue.co/profile/aisupr)** — Weekly AI regulation and policy digest.
- **[The Batch (DeepLearning.AI)](https://www.deeplearning.ai/the-batch/)** — AI news with regulation coverage.
- **[Import AI](https://jack-clark.net)** — Jack Clark's AI research and policy newsletter.
- **[IAPP Daily Dashboard](https://iapp.org/news/daily-dashboard/)** — Privacy and AI governance news.

---

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a pull request.

**Criteria for inclusion:**
- Actively maintained (updated within 12 months)
- Directly relevant to EU AI Act compliance or AI governance
- Open-source tools: must have a public repository
- Commercial tools: must have a free tier, trial, or public documentation

**Not included:**
- Paid-only tools with no free tier or public docs
- Tools with no EU AI Act relevance
- Abandoned projects (no activity > 12 months)

---

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work.
