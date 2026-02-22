# ISO 27001 Control Mapping  
## Southern Cross Capital Pty Ltd  
### Information Security Management System (ISMS) Alignment

---

# 1️⃣ Purpose

This document maps implemented security controls to ISO/IEC 27001 Annex A control domains.

The objective is to demonstrate that:

- Risk management activities align with structured ISMS principles
- Implemented controls support internationally recognised security standards
- Governance processes reflect compliance maturity

This mapping strengthens audit readiness and regulatory credibility.

---

# 2️⃣ ISO 27001 Control Mapping

---

# 1️⃣ Access Control (Annex A – Access Control)

### Your Implementation

- IAM least-privilege policies
- Removal of unnecessary AdministratorAccess
- MFA enforcement for root and privileged users
- Periodic IAM access review
- Privileged activity monitoring via CloudTrail

### Risks Addressed

- IAM privilege escalation
- Account compromise
- Insider misuse
- Unauthorized administrative access

### ISO Alignment Rationale

ISO 27001 requires:

- Controlled access to information systems
- Role-based access restriction
- Periodic access review
- Strong authentication mechanisms

Your IAM hardening directly aligns with ISO access control requirements.

---

# 2️⃣ Cryptography Controls (Annex A – Cryptography)

### Your Implementation

- S3 encryption at rest (AES-256)
- EBS encryption by default
- HTTPS/TLS enforcement for web application
- Key management access restriction

### Risks Addressed

- Data exposure
- Financial information breach
- Backup compromise
- Man-in-the-middle interception

### ISO Alignment Rationale

ISO requires:

- Protection of confidentiality and integrity
- Encryption of sensitive information
- Key management governance

Financial data encryption demonstrates compliance with cryptographic control objectives.

---

# 3️⃣ Logging & Monitoring (Annex A – Logging and Monitoring)

### Your Implementation

- Multi-region CloudTrail enabled
- CloudWatch alert configuration
- Log retention policy (365 days)
- Root login monitoring
- S3 access logging

### Risks Addressed

- Undetected breach
- Delayed incident response
- Insider activity concealment
- Regulatory non-compliance

### ISO Alignment Rationale

ISO requires:

- Event logging
- Monitoring of system activity
- Protection of log integrity
- Incident traceability

Your monitoring controls support auditability and forensic capability.

---

# 4️⃣ Incident Management (Annex A – Incident Management)

### Your Implementation

- Documented Incident Response lifecycle
- Containment, eradication, recovery process
- Impact analysis documentation
- Lessons learned procedure
- Governance escalation model

### Risks Addressed

- Regulatory reporting failure
- Extended operational disruption
- Repeated control weaknesses

### ISO Alignment Rationale

ISO requires:

- Formal incident management process
- Reporting mechanisms
- Post-incident review
- Continuous improvement

Your incident documentation demonstrates structured response governance.

---

# 5️⃣ Risk Management (ISO 27001 Clause 6 – Planning)

### Your Implementation

- Formal risk register
- Likelihood × Impact scoring model
- Risk categorisation (Low–Critical)
- Residual risk calculation
- Risk heat map visualization
- Control effectiveness evaluation

### Risks Addressed

- Unstructured risk decision-making
- Inconsistent prioritisation
- Lack of executive oversight

### ISO Alignment Rationale

ISO requires:

- Risk identification
- Risk assessment
- Risk treatment
- Ongoing review

Your structured risk lifecycle directly aligns with ISO risk management principles.

---

# 3️⃣ ISMS Principles Demonstrated

This project reflects core ISO 27001 ISMS principles:

✔ Risk-based approach  
✔ Documented controls  
✔ Continuous improvement  
✔ Executive oversight  
✔ Monitoring and measurement  
✔ Corrective actions  

The lifecycle followed:

Risk Identification  
→ Control Implementation  
→ Monitoring  
→ Incident Response  
→ Post-Incident Review  
→ Governance Update  

This mirrors ISO’s Plan–Do–Check–Act (PDCA) model.

---

# 4️⃣ Governance Maturity Assessment

Your project demonstrates:

- Structured access governance
- Encryption enforcement
- Monitoring capability
- Incident lifecycle management
- Risk documentation discipline
- Remediation tracking

This aligns with foundational ISO 27001 compliance expectations.

While not a full certification-ready ISMS, the framework demonstrates strong alignment with ISO Annex A controls and Clause 6 risk management requirements.

---

# 5️⃣ Executive Summary

This cloud security program aligns with ISO 27001 principles by:

- Managing risk systematically
- Implementing preventive and detective controls
- Maintaining audit evidence
- Enforcing governance oversight
- Demonstrating continuous improvement

Compliance maturity is not achieved by documentation alone.

It is achieved through risk-driven, measurable, and monitored security governance.

This project reflects structured ISMS thinking aligned with international best practice.
