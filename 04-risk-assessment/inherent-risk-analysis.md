# Inherent Risk Analysis  
## Southern Cross Capital Pty Ltd  
### AWS Cloud Migration – Financial Services Risk Evaluation

---

## 1. Purpose of This Analysis

This document evaluates the **top five highest inherent risks** identified in the cloud risk register before additional mitigation controls are applied.

Inherent risk represents the level of exposure assuming no new controls are introduced beyond the current baseline.

The objective is to:

- Highlight board-level risk exposure  
- Explain why certain risks are classified as Critical  
- Demonstrate business impact in financial services context  
- Prioritise mitigation strategy  

---

# Top 5 Highest Inherent Risks

Based on risk scoring (Likelihood × Impact), the highest risks identified are:

| Risk ID | Risk Description | Score | Risk Level |
|---------|------------------|-------|------------|
| R1 | Public S3 Data Exposure | 20 | Critical |
| R4 | No MFA on Admin Accounts | 16 | Critical |
| R10 | Misconfigured Security Groups | 16 | Critical |
| R2 | IAM Privilege Escalation | 15 | High |
| R3 | Ransomware on EC2 | 15 | High |

---

# R1 — Public S3 Data Exposure (Score: 20 – Critical)

## Why It Is Critical

Likelihood: 4 (Likely)  
Cloud misconfiguration is one of the most common causes of financial sector breaches globally.

Impact: 5 (Severe)  
Exposure of customer financial data triggers mandatory breach notification and regulatory investigation.

---

## Business Impact

- Immediate regulatory notification
- Customer trust erosion
- Potential class-action lawsuits
- Executive and board accountability review

---

## Why Financial Sector Increases Severity

Financial institutions store highly sensitive customer identity and financial records.

Unlike many industries, exposure directly enables fraud, identity theft, and financial crime.

Regulatory bodies (APRA, Privacy Commissioner) impose strict scrutiny on financial data protection.

Severity in financial services is significantly higher than in non-regulated sectors.

---

# R4 — No MFA on Admin Accounts (Score: 16 – Critical)

## Why It Is Critical

Likelihood: 4 (Likely)  
Credential theft via phishing is common in financial institutions.

Impact: 4 (Major)  
Admin account compromise can lead to full cloud takeover.

---

## Business Impact

- Full AWS account compromise
- Service disruption
- Data exfiltration
- Ransomware deployment

---

## Financial Sector Severity Amplifier

Administrative control in financial services environments governs:

- Trading platforms
- Customer records
- Financial transactions

Loss of administrative control can halt operations during market hours, creating immediate financial loss.

---

# R10 — Misconfigured Security Groups (Score: 16 – Critical)

## Why It Is Critical

Likelihood: 4 (Likely)  
Open ports (0.0.0.0/0 exposure) are frequently detected in cloud audits.

Impact: 4 (Major)  
External attackers can exploit exposed services.

---

## Business Impact

- Remote exploitation of EC2 servers
- Malware injection
- Data compromise
- Service outage

---

## Financial Sector Severity Amplifier

Public-facing financial systems must maintain strong perimeter security.

Exposure can lead to:

- Unauthorised access to trading systems
- Transaction manipulation
- Financial fraud

Given regulatory expectations, perimeter misconfiguration is unacceptable at board level.

---

# R2 — IAM Privilege Escalation (Score: 15 – High)

## Why It Is High

Likelihood: 3 (Possible)  
Over-permissive IAM roles are common in growing cloud environments.

Impact: 5 (Severe)  
Privilege escalation enables system-wide compromise.

---

## Business Impact

- Data exfiltration
- Infrastructure manipulation
- Backup deletion
- Fraudulent activity

---

## Financial Sector Severity Amplifier

Financial systems rely heavily on strict access governance.

Weak IAM controls undermine segregation of duties, a key regulatory requirement.

APRA explicitly requires strong access governance controls under CPS 234.

---

# R3 — Ransomware on EC2 (Score: 15 – High)

## Why It Is High

Likelihood: 3 (Possible)  
Ransomware targeting financial institutions remains common.

Impact: 5 (Severe)  
System encryption leads to operational shutdown.

---

## Business Impact

- Trading disruption
- Customer transaction delays
- Revenue loss
- Recovery and rebuild costs

---

## Financial Sector Severity Amplifier

Financial services operate in time-sensitive environments.

Even short service interruptions may cause:

- Missed market opportunities
- Direct financial losses for customers
- Compensation obligations

Resilience expectations are significantly higher than in many other industries.

---

# Executive Summary

The top inherent risks share common themes:

- Identity and access governance weaknesses
- Cloud misconfiguration exposure
- Monitoring and detection gaps
- Infrastructure resilience risk

In financial services, cyber risk is not simply an IT concern — it is:

- A regulatory compliance issue  
- A financial stability issue  
- A shareholder confidence issue  
- A board-level accountability issue  

These risks demand immediate prioritisation and structured mitigation planning.

The next step is to evaluate:

- Existing control effectiveness  
- Residual risk after mitigation  
- Control investment prioritisation  

In financial institutions, unmanaged cyber risk directly translates into financial and regulatory consequences.

Risk discipline is therefore not optional — it is a governance requirement.
