# Corporate Vendor Intake & Criticality Tiering Matrix

**Document ID:** OMNI-TPRM-INT-001  
**Version:** 1.0  
**Classification:** Internal GRC Operational Standard  
**Regulatory Alignment:** GDPR Article 28 | POPIA Section 21 | NIST SP 800-161 (SR-4)

---

## 1. Operational Overview
Every business unit seeking to procure or integrate a third-party software solution, SaaS application, or external cloud infrastructure resource must formally submit this intake request to the TPRM team. This matrix mathematically defines the vendor’s **Inherent Risk Tier**, which dictates the depth of due diligence required before a procurement contract can be executed.

---

## 📊 Inherent Risk Ingestion Questionnaire

Hiring managers must answer the following binary triage queries regarding the vendor's logical boundaries:

| Screening Query | Operational Inherent Vector | Risk Value Impact |
| :--- | :--- | :--- |
| **Q1:** Will the vendor ingest, process, or store any customer's Personal Identifiable Information (PII) or European citizen records? | **GDPR / POPIA Privacy Scope** | Yes = Add 3 Points<br>No = 0 Points |
| **Q2:** Will the third-party application require direct programmatic access (API, Service Account, IAM Role) into the production's AWS environment? | **Cloud Network Perimeter Attack Surface** | Yes = Add 4 Points<br>No = 0 Points |
| **Q3:** Does the vendor software directly manipulate financial transactions, customer billing data, or internal corporate financial ledgers? | **Core Regulatory & Financial Impact** | Yes = Add 3 Points<br>No = 0 Points |
| **Q4:** If this vendor suffers a total infrastructure outage exceeding 4 continuous hours, will the customer's primary business operations freeze? | **Business Continuity & Resilience Impact** | Yes = Add 2 Points<br>No = 0 Points |

---

## ⚙️ Inherent Risk Score Tier Escalation Paths

By accumulating the values derived from the intake matrix, the TPRM team maps the vendor to one of three specific operational tracking paths:

### 🔴 Tier 1: High Inherent Risk (Score: 7 - 12 Points)
* **Definition:** The vendor interacts directly with sensitive customer PII, holds production cloud parameters, or impacts financial flow.
* **GRC Mandate:** Full comprehensive audit required. The vendor must provide a current **SOC 2 Type II report** (with clean, unmodified auditor opinions) or undergo a formal **SIG Core Questionnaire assessment**. Must be reviewed and signed off by the CISO.

### 🟡 Tier 2: Medium Inherent Risk (Score: 3 - 6 Points)
* **Definition:** The vendor accesses internal company information, but does not interact with production infrastructure, financial data, or external user PII.
* **GRC Mandate:** Standard audit required. The vendor must submit an **ISO 27001 certification** or complete a localized internal security questionnaire. Reviewed quarterly.

### 🟢 Tier 3: Low Inherent Risk (Score: 0 - 2 Points)
* **Definition:** Internal non-critical productivity tools that hold zero access to corporate databases, source code, or personal datasets.
* **GRC Mandate:** Simplified vetting. Verification of standard Terms of Service and automated public vulnerability checks.
