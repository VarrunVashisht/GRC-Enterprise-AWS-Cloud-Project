# Control Effectiveness Evaluation  
## Southern Cross Capital Pty Ltd  
### AWS Security Hardening – Risk Reduction Assessment

---

## 1. Purpose

This document evaluates the effectiveness of implemented security controls in reducing identified cloud risks.

It connects:

- Inherent Risk (before controls)
- Implemented Controls
- Residual Risk (after controls)
- Governance impact

The objective is to demonstrate measurable risk reduction and validate that controls align with financial sector expectations.

---

# 2. Risk-to-Control Mapping

Below is a structured evaluation of how implemented controls reduced risk exposure.

---

## R1 — Public S3 Exposure

**Inherent Risk:** Critical (20)  
Likelihood: 4  
Impact: 5  

### Controls Implemented:
- S3 Block Public Access enforced
- Default encryption enabled
- S3 access logging enabled
- CloudTrail monitoring active

### Risk Reduction Logic:

- Misconfiguration likelihood reduced due to enforced block settings.
- Detection capability improved via logging.
- Encryption reduces impact severity of exposure.

### Residual Risk:
Likelihood: 2  
Impact: 4  
Residual Score: 8 (Medium)

### Control Effectiveness Assessment:
High effectiveness in reducing probability.
Impact remains significant due to financial data sensitivity.

---

## R2 — IAM Privilege Escalation

**Inherent Risk:** High (15)

### Controls Implemented:
- Least privilege IAM policies
- Removal of unnecessary admin roles
- MFA enforcement
- IAM activity monitoring

### Risk Reduction Logic:

- Reduces excessive permissions.
- Limits privilege escalation path.
- Improves detection of suspicious access.

### Residual Risk:
Reduced from High → Medium

### Control Effectiveness Assessment:
Moderate to High effectiveness.
Identity governance remains ongoing risk area in financial institutions.

---

## R3 — Ransomware on EC2

**Inherent Risk:** High (15)

### Controls Implemented:
- Patch management process
- EBS encryption
- Backup isolation
- CloudTrail monitoring

### Risk Reduction Logic:

- Reduces exploitability of known vulnerabilities.
- Ensures recovery capability.
- Improves detection time.

### Residual Risk:
High → Medium

### Control Effectiveness Assessment:
Moderate effectiveness.
Zero-day and advanced attacks remain possible.

---

## R4 — No MFA on Admin Accounts

**Inherent Risk:** Critical (16)

### Controls Implemented:
- Mandatory MFA enforcement
- Root account monitoring
- Privileged access restriction

### Risk Reduction Logic:

- Eliminates simple credential-only compromise.
- Reduces account takeover probability.

### Residual Risk:
Critical → Medium

### Control Effectiveness Assessment:
High effectiveness.
MFA significantly reduces likelihood of administrative compromise.

---

## R5 — CloudTrail Disabled

**Inherent Risk:** High (12)

### Controls Implemented:
- Multi-region CloudTrail enabled
- Log retention policy implemented
- Alert configuration established

### Risk Reduction Logic:

- Eliminates blind spots.
- Enables rapid detection of compromise.

### Residual Risk:
High → Low

### Control Effectiveness Assessment:
Very High effectiveness.
Detection maturity significantly improved.

---

# 3. Quantitative Risk Reduction Overview

| Risk ID | Inherent Level | Residual Level | Risk Reduction |
|----------|---------------|----------------|----------------|
| R1 | Critical | Medium | Significant |
| R2 | High | Medium | Moderate |
| R3 | High | Medium | Moderate |
| R4 | Critical | Medium | Significant |
| R5 | High | Low | Significant |

Overall outcome:

- All Critical risks reduced to Medium.
- No residual risks remain Critical.
- Detection capability significantly improved.

---

# 4. Governance & Financial Sector Perspective

In financial services:

- Risk cannot be eliminated.
- Risk must be controlled within tolerance.
- Controls must be monitored continuously.
- Identity and logging are priority control domains.

Control implementation demonstrates:

- Reduction of attack likelihood.
- Improved detection capability.
- Enhanced compliance posture.
- Alignment with APRA CPS 234 expectations.

---

# 5. Residual Risk Governance Position

Residual Medium risks require:

- Continuous monitoring
- Quarterly IAM review
- Configuration audits
- Annual penetration testing
- Board visibility if risk increases

Residual Low risks require:

- Periodic review
- Automated monitoring validation

---

# 6. Strategic Security Maturity Assessment

Security posture maturity has moved from:

Reactive & exposed  
to  
Structured & controlled

However:

- Identity governance remains highest residual exposure.
- Human error risk persists.
- Cloud misconfiguration risk requires automation investment.

True risk maturity requires:

- Automation
- Continuous review
- Executive oversight
- Cultural security awareness

---

# Executive Summary

Control implementation successfully reduced:

- Critical risk exposure
- Undetected breach probability
- Identity compromise likelihood
- Cloud misconfiguration severity

This demonstrates:

Risk identification → Control implementation → Risk reduction → Governance validation

This is the full professional risk lifecycle.

Security effectiveness is measured not by absence of risk,
but by controlled, monitored, and justified exposure.
