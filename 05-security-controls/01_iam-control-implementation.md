# IAM Control Implementation  
## Southern Cross Capital Pty Ltd  
### AWS Security Hardening – Identity & Access Governance

---

## 1. Purpose

This document describes the implementation of Identity and Access Management (IAM) security controls to mitigate High and Critical risks identified in the risk register.

Primary risks addressed:

- R2 – IAM Privilege Escalation  
- R4 – No MFA on Admin Accounts  
- R10 – Misconfigured Access Exposure  

Identity governance is the most critical security control domain in cloud environments.

---

# 2. Identified IAM Weaknesses (Before Hardening)

During initial review, the following weaknesses were identified:

- Root account accessible without MFA
- IAM users with excessive permissions (AdministratorAccess)
- No structured least-privilege policy
- Shared IAM usage patterns
- Limited monitoring of privileged activity

These weaknesses increased the risk of:

- Account takeover
- Privilege escalation
- Insider abuse
- Ransomware deployment

---

# 3. Control Implementation Steps

---

## ✔ Control 1 — Enable MFA for Root Account

### Risk Addressed:
R4 – Account Takeover

### Action Taken:
- Logged into AWS Console
- Navigated to IAM → Security Credentials
- Enabled Multi-Factor Authentication (MFA) for root account
- Configured virtual MFA device

### Why This Reduces Risk:
Even if root credentials are stolen, attacker cannot log in without MFA token.

### Governance Impact:
Reduces likelihood of full cloud compromise.

---

## ✔ Control 2 — Enforce MFA for IAM Users

### Risk Addressed:
R2 – IAM Privilege Escalation  
R4 – Credential Theft

### Action Taken:
- Created IAM policy requiring MFA for console login
- Attached policy to privileged IAM users
- Tested login without MFA (denied)

### Why This Reduces Risk:
Prevents simple phishing-based credential compromise from succeeding.

---

## ✔ Control 3 — Implement Least Privilege IAM Roles

### Risk Addressed:
R2 – Privilege Escalation

### Before:
- Users had AdministratorAccess policy
- Broad permissions across services

### Action Taken:
- Created custom IAM role:
  - Limited EC2 permissions
  - Limited S3 access to specific buckets
  - No privilege escalation rights
- Removed unnecessary admin privileges

### After:
Access restricted based on job function.

### Why This Reduces Risk:
Limits blast radius if account is compromised.

---

## ✔ Control 4 — Remove Unnecessary Admin Accounts

### Risk Addressed:
R2 – Excessive Privilege

### Action Taken:
- Reviewed IAM user list
- Deleted unused accounts
- Disabled inactive credentials
- Rotated access keys

### Why This Reduces Risk:
Reduces attack surface and credential exposure.

---

## ✔ Control 5 — Avoid Use of Root Account

### Risk Addressed:
Critical governance risk

### Action Taken:
- Restricted root usage to billing only
- Created separate admin role for operations
- Documented root access governance policy

### Why This Reduces Risk:
Root account compromise would result in total control loss.
Minimising usage reduces exposure probability.

---

# 4. Residual Risk Evaluation

| Risk ID | Before | After | Explanation |
|----------|--------|--------|-------------|
| R2 – IAM Privilege Escalation | High | Medium | Least privilege reduces exploitation surface |
| R4 – No MFA | Critical | Medium | MFA significantly lowers credential abuse likelihood |

Impact remains high because:

- Financial data remains sensitive
- Administrative compromise still severe

However, likelihood has decreased.

Residual risk is now within acceptable tolerance for monitored environments.

---

# 5. Governance Reflection

IAM hardening is not a one-time task.

Ongoing requirements:

- Quarterly access review
- Privilege re-certification
- Access key rotation
- Continuous monitoring of IAM changes

In financial services, identity governance is a board-level control expectation.

Cloud security maturity begins with IAM discipline.
