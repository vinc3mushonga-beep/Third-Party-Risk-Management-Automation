# Third-Party Risk Management (TPRM) Framework 🌐

### Enterprise Supply Chain Governance, Cloud Vendor Vetting, & Compliance Automation Baseline

## 🏢 Corporate Mandate & Project Scope
As a multinational enterprise, relies heavily on third-party Software-as-a-Service (SaaS) applications, external sub-processors, and cloud platform vendors. Under regulations like **EU GDPR (Article 28 - Processors)** and **South African POPIA (Section 21 - Security measures regarding operator)**, legally liable if a third-party vendor loses our customer data.

This repository hosts the **TPRM Framework**. It serves as an end-to-end operational blueprint for identifying, assessing, scoring, and continuously monitoring supply chain risks. It bridges abstract legal compliance mandates with actionable, technical vendor security baselines—ensuring no external software is onboarded without passing strict governance gates.

---

## 📂 Repository Architecture

This repository is engineered to replicate an enterprise-grade corporate risk portal:
* `vendor-onboarding/` : Mandatory pre-vetting intake forms, critical tiering matrix questionnaires, and GDPR Data Processing Addendums (DPAs).
* `assessment-templates/` : Automated Vendor Risk Vetting templates aligned with the **Shared Assessments SIG Core** and **NIST SP 800-161**.
* `automated-scoring/` : Inherent vs. Residual Vendor Risk Matrix tables utilizing automated weighted logic scripts.
* `continuous-monitoring/` : Playbooks detailing continuous security telemetry verification (such as SOC 2 verification pipelines and automated vendor offboarding protocols).

---

## 🏗️ Technical Vetting Framework & Automation Stack

Accelerates and standardizes third-party evaluations using a strict compliance tiering architecture:

### 1. Supply Chain Control Alignment (NIST SP 800-161)
* Every external system undergoes a mandatory technical mapping against the **NIST Supply Chain Risk Management (SCRM)** framework, specifically auditing vendor patch deployment speeds, encrypting-at-rest configurations, and physical data center access security.

### 2. Legal Data Processor Mandates (GDPR Art. 28 / POPIA Sec 20-21)
* Vendors processing employee or customer data must execute a mandatory **Data Processing Addendum (DPA)**. This legally binds the vendor to mirrors strict security boundaries, mandating a strict 72-hour breach notification window back to our internal Security Operations Center (SOC).

### 3. AWS Security Artifact Verification (The Cloud Vetting standard)
* When vetting external cloud integrations, the GRC team utilizes **AWS Artifact** and independent assurance portals to scrutinize the vendor's underlying host infrastructure (verifying active **ISO 27001** and **SOC 2 Type II** audit attestations) under the Cloud Shared Responsibility Model.

---

## 📜 Professional Framework Alignment Demonstrated
* **NIST SP 800-161 Rev. 1:** Supply Chain Risk Management Practices for Systems and Organizations.
* **EU GDPR:** Article 28 (Processor Requirements), Article 32 (Security of Processing).
* **South African POPIA:** Section 20 (Processing by operator), Section 21 (Security measures regarding operator processing).
* **AICPA SOC 2:** Trust Services Criteria (Security, Availability, and Confidentiality).
