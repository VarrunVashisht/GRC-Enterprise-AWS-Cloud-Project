# Logging & Monitoring Control Implementation  
## Southern Cross Capital Pty Ltd  
### AWS Security Monitoring & Detection Hardening

---

## 1. Purpose

This document outlines monitoring and logging controls implemented to reduce risks related to:

- R5 – CloudTrail Disabled (Undetected Breach)
- R2 – IAM Privilege Escalation
- R1 – Public S3 Exposure
- R3 – Ransomware Deployment
- R10 – Security Group Misconfiguration

In financial services, **undetected breaches are considered governance failure**.

Monitoring converts:

Undetected compromise → Detectable incident

---

# 2. Identified Monitoring Gaps (Before Hardening)

Initial review revealed:

- CloudTrail not fully enabled
- No log retention policy
- No alerting for IAM changes
- No S3 access logging
- No security event monitoring

These weaknesses increased risk of:

- Delayed breach detection
- Insider abuse going unnoticed
- Ransomware persistence
- Regulatory non-compliance

---

# 3. Control Implementation Steps

---

## ✔ Control 1 — Enable AWS CloudTrail

### Risk Addressed:
R5 – Undetected Breach  
R2 – IAM Privilege Escalation  

### Action Taken:
- Enabled CloudTrail across all regions
- Configured trail to log:
  - Management events
  - IAM changes
  - API calls
- Stored logs in dedicated encrypted S3 bucket

### Why This Reduces Risk:
CloudTrail provides visibility into:

- Who accessed what
- What changes were made
- When activity occurred

This significantly reduces likelihood of prolonged undetected compromise.

---

## ✔ Control 2 — Enable S3 Access Logging

### Risk Addressed:
R1 – Public S3 Exposure  

### Action Taken:
- Enabled S3 server access logging
- Directed logs to central logging bucket
- Restricted access to log bucket

### Why This Reduces Risk:
Provides audit trail for:

- Object access
- External access attempts
- Suspicious download patterns

Supports forensic investigation and compliance audits.

---

## ✔ Control 3 — Configure Basic Security Alerts

### Risk Addressed:
R2 – Privilege Escalation  
R10 – Security Group Changes  

### Action Taken:
- Enabled AWS CloudWatch monitoring
- Configured alerts for:
  - IAM policy changes
  - Root login attempts
  - Security group modifications
  - Failed login attempts

### Why This Reduces Risk:
Early detection reduces attacker dwell time.

In financial institutions, rapid detection is critical to reduce financial and reputational damage.

---

## ✔ Control 4 — Log Retention Policy

### Risk Addressed:
Compliance failure

### Action Taken:
- Configured log retention for 365 days
- Ensured logs stored in encrypted bucket
- Restricted deletion permissions

### Why This Reduces Risk:
Supports:

- Regulatory investigations
- Incident response
- Forensic analysis

APRA expects adequate log retention capability.

---

## ✔ Control 5 — Monitor Root Account Activity

### Risk Addressed:
Critical governance risk

### Action Taken:
- Created CloudWatch alert for root login
- Tested alert functionality
- Documented emergency access process

### Why This Reduces Risk:
Root account compromise represents total control loss.

Immediate detection is mandatory.

---

# 4. Residual Risk Evaluation

| Risk ID | Inherent Level | Post-Monitoring Residual |
|----------|---------------|---------------------------|
| R5 – CloudTrail Disabled | High | Low |
| R2 – IAM Privilege Escalation | High | Medium |
| R10 – Security Group Changes | Critical | Medium |
| R1 – S3 Exposure | Critical | Medium |

Monitoring does not eliminate risk.

Monitoring reduces:

- Detection time
- Incident severity
- Regulatory exposure

Impact may remain high, but likelihood of prolonged breach decreases.

---

# 5. Governance Reflection

Monitoring transforms security posture from:

Reactive → Proactive  

Financial institutions are judged not only by whether breaches occur, but by:

- How quickly they detect them
- How effectively they respond
- Whether logging supports investigation

Security maturity requires:

- Continuous monitoring
- Alert validation testing
- Quarterly log review
- Incident simulation exercises

Logging is not optional in regulated industries.

Without monitoring, all other controls lose value.
