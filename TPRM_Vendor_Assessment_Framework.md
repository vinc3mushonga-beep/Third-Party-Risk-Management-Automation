# Third-Party Risk Management (TPRM) Assessment Framework
## Methodology & Compliance Integration

### 1. Vendor Tiering & Categorisation Methodology
ApexVault Digital Ltd. categorizes all vendors into three clear tiers to optimize audit cycles and risk-mitigation enforcement:

*   **Tier 1: Critical ICT Third-Party Providers (CITPP)**
    *   *Definition*: Software, cloud, or infrastructure vendors whose prolonged disruption would immediately paralyze ApexVault's core payment processing services or cause catastrophic financial systemic risk.
    *   *Assessment Frequency*: Semi-annual continuous auditing + automated daily external attack surface scans via Qualys VMDR.
*   **Tier 2: Important Providers**
    *   *Definition*: Vendors supporting operations that do not impact live real-time settlement but control corporate workflows or access non-production codebases.
    *   *Assessment Frequency*: Annual review.
*   **Tier 3: General Providers**
    *   *Definition*: Commodity utilities, administrative SaaS applications, or marketing tools processing minimal or non-critical asset records.
    *   *Assessment Frequency*: Initial intake vetting only.

### 2. Regulatory Interoperability Matrix
To prevent auditing duplication, this framework leverages regulatory cross-mapping between data privacy regimes and infrastructure resilience frameworks:

| Assessment Domain | DORA Regulation Requirement | GDPR Compliance Requirement | ISO/IEC 27701 Reference | Cloud Controls Integration (CCSK) |
| :--- | :--- | :--- | :--- | :--- |
| **Risk Management** | Article 8: ICT Risk Framework | Article 32: Security of Processing | Clause 5.4: Information Security Risk Assessment | AIS-01: Application & Interface Security |
| **Data Protection** | Article 12: Cryptographic Controls | Article 25 & 32: Pseudonymization | Clause 7.3: PII Protection by Design/Default | DSI-03: Encryption & Key Management |
| **Vulnerability Lifecycle**| Article 11: System Vulnerability Testing | Article 32: Routine Testing Enforcements | Clause 6.12: Vulnerability Management Operations | TVM-02: Remediation & Patching SLAs |
| **Supply Chain Assurance** | Article 30: Contractual Minimum Terms | Article 28: Data Processing Agreements (DPA) | Clause 7.5: PII Sharing & Transfers | BCR-01: Business Continuity Management |

### 3. The Implications of DORA on TPRM
Under traditional GRC approaches, third-party vetting relied on point-in-time SOC 2 Type II reports. DORA fundamentally transforms this landscape through three legally binding operational implications:

1.  **Mandatory Unrestricted Audit Rights (DORA Article 30)**: Contracts must explicitly grant ApexVault and its competent financial regulators unconditional rights to conduct physical inspections, on-site audits, and real-time security log reviews of vendor assets.
2.  **Systemic Concentration Risk Management**: ApexVault is legally obligated to analyze if it is overly reliant on a singular vendor infrastructure network. If a vendor creates a single point of catastrophic failure, alternate contingency paths must be formally documented.
3.  **Compulsory Multi-Vendor Exit Strategies**: For every Tier 1 Critical Provider, ApexVault must write and run testing on a clear, comprehensive exit strategy. This plan must prove ApexVault can migrate core services to an in-house architecture or backup vendor seamlessly if the provider suffers a prolonged systemic outage.
