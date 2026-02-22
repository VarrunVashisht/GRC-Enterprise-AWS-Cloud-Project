# Executive Risk Summary  
## Southern Cross Capital Pty Ltd  
### Cloud Migration Security Assessment

---

# 1️⃣ Objective

The objective of this assessment was to evaluate cybersecurity risks associated with the migration of core trading and financial systems to AWS cloud infrastructure.

The assessment examined:

- Identity and access controls  
- Data protection measures  
- Monitoring capabilities  
- Incident response readiness  
- Regulatory alignment (Australian context)  

The goal was to determine current exposure levels and evaluate whether implemented controls sufficiently reduce risk in line with financial regulatory expectations.

---

# 2️⃣ Key Findings

- 3 Critical Risks identified during initial assessment  
- 4 High Risks identified  
- IAM misconfiguration and S3 exposure represented the highest enterprise risk  
- Logging and encryption controls significantly reduced residual risk  
- No Critical risks remain after remediation  

Primary exposure areas:

- Identity & Access Governance  
- Cloud configuration management  
- Backup resilience  

Control implementation materially improved overall security posture.

---

# 3️⃣ Top 3 Enterprise Risks

## 1. IAM Privilege Escalation

**Business Impact:**  
If administrative credentials are compromised, attackers may gain full control of cloud infrastructure. This could result in trading platform outage, data exposure, and regulatory escalation.

**Why It Matters:**  
Financial institutions rely heavily on cloud identity controls. Administrative compromise directly affects operational continuity and regulatory compliance.

---

## 2. Public Data Exposure (S3 Misconfiguration)

**Business Impact:**  
Misconfigured storage could expose customer financial information, triggering mandatory regulatory reporting and reputational damage.

**Why It Matters:**  
Customer trust and regulatory compliance depend on strict protection of financial data.

---

## 3. Backup Integrity Failure

**Business Impact:**  
If backups are deleted or compromised during ransomware attack, recovery time increases significantly, impacting revenue and customer confidence.

**Why It Matters:**  
Resilience is critical in financial services. Recovery capability directly affects market credibility.

---

# 4️⃣ Risk Reduction Outcome

Following control implementation:

- All Critical risks reduced to Medium  
- Identity governance strengthened  
- Encryption implemented across critical assets  
- Monitoring and alerting improved detection speed  
- Backup resilience enhanced  

Estimated Critical Risk Reduction: Significant (Critical risk count reduced from 3 → 0)

Additional outcomes:

- Improved regulatory alignment (Privacy Act, CPS 234)  
- Reduced likelihood of large-scale data breach  
- Improved executive visibility into cyber exposure  

---

# 5️⃣ Overall Security Posture

Post-remediation security posture is assessed as:

Moderate-to-Strong

Key strengths:

- Structured risk management framework  
- Formal vulnerability lifecycle  
- Documented incident response capability  
- Compliance alignment with ISO & NIST  

Ongoing requirement:

Continuous monitoring and governance oversight.

Cyber risk remains dynamic and requires executive attention.

---

# Executive Conclusion

The cloud migration introduces elevated cyber risk exposure, particularly in identity governance and configuration management.

However, implemented controls significantly reduced residual risk.

Continued investment in identity security, monitoring automation, and resilience testing is recommended to maintain strong governance posture.

Cybersecurity should remain a board-visible risk category due to regulatory accountability and financial exposure.
