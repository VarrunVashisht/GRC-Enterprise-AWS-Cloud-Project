# Lessons Learned  
## IAM Credential Compromise & Ransomware Deployment  
### Southern Cross Capital Pty Ltd – Post-Incident Review

---

# 1️⃣ Purpose

This document captures lessons learned from the simulated IAM credential compromise and ransomware incident.

The objective is to:

- Identify root causes
- Strengthen preventive controls
- Improve detection capability
- Enhance governance oversight
- Update risk posture

In financial services, post-incident review is a regulatory expectation.

---

# 2️⃣ Root Cause Analysis

---

## Primary Root Cause

Over-permissive IAM role combined with credential compromise.

The compromised user had:

- Excessive administrative privileges
- No enforced phishing-resistant MFA
- Broad access across AWS services

---

## Contributing Factors

- Human susceptibility to phishing
- Lack of automated IAM anomaly detection
- Insufficient backup immutability controls
- No formal phishing simulation program
- Limited segregation of duties

---

# 3️⃣ Control Gaps Identified

The incident exposed weaknesses in:

---

## Identity Governance

- Privilege creep over time
- Lack of strict least-privilege enforcement
- No periodic access recertification

---

## Backup Protection

- Backups could be deleted without additional approval
- No immutable storage configuration

---

## Monitoring Maturity

- Alerts existed but required manual interpretation
- No automated response playbooks

---

# 4️⃣ What Worked Well

Despite weaknesses, several controls were effective:

- CloudTrail logging enabled detection
- CloudWatch alerts triggered quickly
- Incident response team activated promptly
- Backup restoration capability existed
- Executive escalation process was structured

Detection occurred within one hour.

Containment occurred within two hours.

This limited overall damage.

---

# 5️⃣ Improvement Actions

---

## Identity Hardening

- Enforce phishing-resistant MFA (hardware token)
- Implement Privileged Access Management (PAM)
- Introduce just-in-time (JIT) administrative access
- Conduct quarterly IAM access review

---

## Backup Resilience

- Enable S3 object lock (immutability)
- Separate backup account (cross-account backup)
- Implement MFA delete enforcement

---

## Monitoring Automation

- Implement automated anomaly detection
- Enable GuardDuty for threat detection
- Introduce automated containment workflows

---

## Human Risk Reduction

- Conduct regular phishing simulation exercises
- Implement mandatory security awareness training
- Establish reporting culture for suspicious emails

---

# 6️⃣ Risk Register Updates

Post-incident updates required:

- Increase likelihood rating for IAM compromise
- Add new risk: "Backup immutability failure"
- Adjust residual risk for ransomware scenario
- Increase monitoring maturity priority

Incident-driven recalibration improves governance accuracy.

---

# 7️⃣ Regulatory & Governance Reflection

Under Australian regulatory expectations:

- Board accountability for cybersecurity is explicit.
- Incident documentation must be retained.
- Remediation plans must be formally tracked.
- Control effectiveness must be demonstrable.

Post-incident improvement demonstrates governance maturity.

Failure to learn would increase regulatory scrutiny.

---

# 8️⃣ Cultural & Strategic Insight

Key insight:

Technology was not primary failure.
Human + governance gap enabled incident.

Security maturity requires:

People  
Process  
Technology  
Oversight  

Financial institutions must assume breach and design for resilience.

---

# 9️⃣ Executive Summary

The incident demonstrated:

- Identity remains highest cloud risk domain.
- Backup resilience is critical in ransomware scenarios.
- Detection capability reduces damage window.
- Governance oversight must be continuous.

Improvements implemented post-incident significantly strengthen security posture.

True security maturity is measured not by avoiding incidents,
but by learning, adapting, and reducing future exposure.
