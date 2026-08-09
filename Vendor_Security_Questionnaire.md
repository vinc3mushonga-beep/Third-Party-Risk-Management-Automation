# Unified Vendor Security Due-Diligence Questionnaire
### Regulatory Target Scope: DORA, GDPR, ISO 27701, CCSK, Qualys VMDR

*Instructions to Vendor: Complete all sections truthfully. Provide referenced policy document titles and supporting evidence where requested. Responses will be reviewed using strict verification metrics.*

---

### Section A: Digital Operational Resilience (DORA Framework Core)
1. **[DORA Art. 9]** Does your organization maintain a documented ICT Risk Management Framework that is reviewed, updated, and approved by your executive board at least annually?
2. **[DORA Art. 11]** Detail your vulnerability disclosure and penetration testing schedule. Do you perform independent, threat-led penetration testing (TLPT) at least every 3 years?
3. **[DORA Art. 14]** What is your documented Maximum Tolerable Downtime (MTD) and Recovery Time Objective (RTO) for core systems processing financial data stream integration?
4. **[DORA Art. 30]** Do you explicitly agree to grant unrestricted on-site inspection, audit, and log access rights to our GRC personnel and European Financial Supervisory Authorities?

### Section B: Data Privacy & Protection (GDPR / ISO 27701)
5. **[GDPR Art. 28 / ISO 27701 7.2]** Do you guarantee that all customer Personally Identifiable Information (PII) is cryptographically isolated and processed exclusively within the geographic boundaries of the European Economic Area (EEA)?
6. **[GDPR Art. 32 / ISO 27701 7.3]** Detail your cryptographic standards for PII. Are data sets encrypted at rest using AES-256 and in transit using TLS 1.3 with Perfect Forward Secrecy (PFS)?
7. **[GDPR Art. 33]** Do you maintain a contractually binding SLA to notify our GRC Incident Response Team within a maximum of 24 hours of detecting any confirmed or suspected data breach?
8. **[ISO 27701 7.5]** Do you utilize fourth-party subcontractors to process or store any PII provided by our organization? If yes, provide your full Vendor Management validation process.

### Section C: Cloud Architecture & Tenant Isolation (CSA CCSK Matrix)
9. **[CCSK DSI-01]** Describe your multi-tenant isolation architecture. How do you prevent logical data leakage and cross-tenant hopping across shared physical compute engines?
10. **[CCSK IAM-02]** Is administrative access to production infrastructure restricted using Zero Trust Network Access (ZTNA), Multi-Factor Authentication (MFA), and Just-In-Time (JIT) privileged access management?
11. **[CCSK EKM-04]** Are cryptographic key management hierarchies isolated completely from the host cloud service provider layer? Who retains custody of root key material?
12. **[CCSK IVS-03]** Are your microservice orchestration layers (e.g., Kubernetes namespaces) segmented using strict network security policies and ingress/egress filtering rules?

### Section D: Vulnerability Management & Threat Exposure (Qualys VMDR Metric Alignment)
13. **[VMDR Asset Discovery]** Do you operate automated asset discovery tools continuously? What is your maximum delta time to detect a newly provisioned public-facing endpoint?
14. **[VMDR Prioritization]** Do you utilize CVSS v3.1 scoring alongside active threat intelligence context to prioritize vulnerabilities? How do you account for TruRisk or active exploit availability?
15. **[VMDR SLA Enforcement]** Do you commit to a remediation/patching SLA of a maximum of 14 calendar days for critical vulnerabilities (CVSS 9.0+) and 30 days for high vulnerabilities (CVSS 7.0 - 8.9)?
16. **[VMDR Configuration Baseline]** Are all production servers hardened according to Center for Internet Security (CIS) Benchmarks? How frequently do you run automated drift audits against these baselines?

### Section E: Continuous Incident Resilience & Operations
17. **[Harvard VPAL Risk Model]** Provide your historical operational availability metrics for the preceding 24 months. Document any systemic outages, root cause analyses, and business continuity activations.
18. **[DORA Art. 12]** Detail your backup isolation strategy. Are backups stored in a mutable format, or are they maintained in air-gapped, immutable, read-only structures protected from ransomware propagation?
19. **[GDPR Art. 17]** Describe your technical workflow to execute a "Right to Be Forgotten" data erasure request across all production caches, database tables, and cold storage configurations.
20. **[DORA Art. 30]** In the event of contract termination, what is your documented decommissioning timeline to safely extract, return, and definitively sanitize all corporate data assets via cryptographic erasure (Crypto-Shredding)?
