# Residual Risk Analysis  
## Southern Cross Capital Pty Ltd  
### AWS Cloud Migration – Post-Control Risk Evaluation

---

## 1. Purpose of Residual Risk Analysis

Residual risk represents the level of risk remaining **after existing controls have been implemented**.

While inherent risk assumes no mitigation, residual risk reflects:

- Control effectiveness  
- Governance maturity  
- Monitoring capability  
- Ongoing exposure  

In financial services, risk is rarely eliminated — it is reduced to an acceptable level aligned with regulatory and board risk appetite.

This document evaluates residual exposure and determines which risks require:

- Ongoing monitoring  
- Additional investment  
- Executive oversight  
- Board-level visibility  

---

# 2. Overview of Residual Risk Position

After applying identified controls, the majority of previously Critical risks have been reduced to Medium or High.

However, due to the sensitive nature of financial services operations, **some residual risk remains unavoidable**.

| Risk ID | Inherent Level | Residual Level |
|----------|----------------|----------------|
| R1 – Public S3 Exposure | Critical | Medium |
| R4 – No MFA | Critical | Medium |
| R10 – Security Group Misconfig | Critical | Medium |
| R2 – IAM Privilege Escalation | High | Medium |
| R3 – Ransomware on EC2 | High | Medium |

---

# 3. Analysis of Key Residual Risks

---

## R1 — Public S3 Exposure (Residual: Medium)

### Why Residual Risk Remains

Controls implemented:
- Block Public Access enforced
- Encryption enabled
- Logging enabled

Residual likelihood reduced significantly.

However:

- Human configuration error is still possible
- Cloud complexity increases over time
- New buckets may be created without governance oversight

### Governance View

Residual impact remains high due to data sensitivity.

Even with strong controls, continuous monitoring and periodic audits are required.

Executive monitoring: Required  
Board-level reporting: Not required unless risk increases

---

## R4 — No MFA on Admin Accounts (Residual: Medium)

### Why Residual Risk Remains

Controls implemented:
- Mandatory MFA
- Conditional access policies

Residual likelihood reduced.

However:

- MFA fatigue attacks possible
- Phishing-resistant MFA not yet deployed
- Privileged accounts remain high-value targets

### Governance View

Identity risk remains one of the most critical exposure areas in financial institutions.

Continuous identity governance and access reviews required.

Executive oversight: Required

---

## R10 — Security Group Misconfiguration (Residual: Medium)

### Why Residual Risk Remains

Controls implemented:
- Restricted inbound rules
- Configuration review process

Residual exposure exists due to:

- Infrastructure scaling changes
- Rapid deployment cycles
- Human error during changes

### Governance View

This risk requires automated configuration monitoring tools to reduce likelihood further.

Technology investment recommended for long-term maturity.

---

## R3 — Ransomware on EC2 (Residual: Medium)

### Why Residual Risk Remains

Controls implemented:
- Patch management
- Endpoint protection
- Backup isolation

However:

- Zero-day vulnerabilities remain possible
- Sophisticated attackers evolve tactics
- Insider-assisted ransomware risk persists

### Governance View

Financial services firms must assume ransomware remains a persistent threat.

Resilience strategy (tested backups, recovery time objectives) must be continuously validated.

Board awareness: Recommended

---

## R2 — IAM Privilege Escalation (Residual: Medium)

### Why Residual Risk Remains

Controls implemented:
- Least privilege IAM
- Role reviews
- Monitoring

Residual exposure remains because:

- Access creep may occur over time
- Emergency access privileges may be misused
- Complex cloud environments create visibility gaps

### Governance View

Identity and privilege governance is a continuous process.

Quarterly access reviews recommended.

---

# 4. Risk Appetite & Governance Alignment

In financial services, acceptable risk tolerance is lower than in many industries due to:

- Direct financial transaction exposure  
- Regulatory scrutiny (APRA CPS 234)  
- Privacy Act obligations  
- Customer trust dependency  

Residual Medium risks are acceptable only if:

- Continuous monitoring exists  
- Regular audit reviews occur  
- Incident response plans are tested  
- Executive visibility is maintained  

No residual risks remain in the Critical category — this reflects strong initial control implementation.

---

# 5. Strategic Recommendations

To further reduce residual exposure:

1. Implement automated cloud configuration monitoring.
2. Deploy phishing-resistant MFA for privileged users.
3. Introduce privileged access management (PAM).
4. Conduct quarterly cloud security audits.
5. Perform annual ransomware simulation exercises.

These measures reduce likelihood rather than impact, which is critical in financial services.

---

# 6. Executive Summary

Residual risk analysis confirms:

- High inherent risks can be reduced through structured controls.
- Identity and cloud configuration remain primary exposure areas.
- Financial sector context amplifies impact severity.
- Continuous governance is required — controls are not one-time solutions.

Cyber risk in financial services is dynamic.

Residual risk management is an ongoing governance responsibility, not a completed task.

Risk maturity is demonstrated not by eliminating risk, but by controlling it within defined tolerance boundaries.
