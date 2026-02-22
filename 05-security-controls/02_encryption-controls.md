# Encryption Control Implementation  
## Southern Cross Capital Pty Ltd  
### AWS Data Protection Hardening

---

## 1. Purpose

This document outlines encryption controls implemented to reduce risk related to:

- R1 – Public S3 Data Exposure  
- R3 – Ransomware on EC2  
- R6 – Backup Data Loss  
- R9 – Third-Party API Exposure  

In financial services, encryption is a regulatory expectation under:

- Australian Privacy Act  
- APRA CPS 234  
- Financial data protection standards  

Encryption protects data confidentiality even if access controls fail.

---

# 2. Identified Weaknesses (Before Hardening)

Initial cloud review identified:

- S3 buckets without enforced encryption
- EC2 volumes not encrypted by default
- No HTTPS enforcement on public endpoints
- No defined key management governance

These weaknesses increase risk of:

- Data theft
- Backup compromise
- Compliance violations
- Credential interception

---

# 3. Control Implementation Steps

---

## ✔ Control 1 — Enable S3 Encryption at Rest

### Risk Addressed:
R1 – Public S3 Exposure  
R6 – Backup Data Loss

### Action Taken:
- Navigated to S3 → Bucket Properties
- Enabled **Default Encryption**
- Selected SSE-S3 (AES-256) encryption
- Verified encryption status

### Why This Reduces Risk:
Even if bucket access is compromised, stored data remains encrypted.

Encryption reduces impact severity of data exposure.

---

## ✔ Control 2 — Enable EC2 EBS Volume Encryption

### Risk Addressed:
R3 – Ransomware / Data Theft

### Action Taken:
- Enabled “Encrypt EBS volumes by default”
- Verified encryption during instance creation
- Confirmed volume encryption status

### Why This Reduces Risk:
Prevents direct disk extraction attacks.
Protects data at rest within compute environment.

---

## ✔ Control 3 — Enforce HTTPS (Encryption in Transit)

### Risk Addressed:
Credential interception  
API data exposure

### Action Taken:
- Ensured web application configured with HTTPS
- Enforced TLS encryption
- Redirected HTTP traffic to HTTPS

### Why This Reduces Risk:
Prevents man-in-the-middle attacks.
Protects customer credentials and transaction data in transit.

---

## ✔ Control 4 — Basic Key Management Governance

### Risk Addressed:
Improper encryption key handling

### Action Taken:
- Reviewed AWS-managed keys
- Restricted KMS key access via IAM policy
- Ensured least privilege for key usage

### Why This Reduces Risk:
Encryption without key governance creates new vulnerabilities.
Restricted key access prevents misuse.

---

# 4. Residual Risk Impact

| Risk ID | Inherent Level | Post-Encryption Residual |
|----------|---------------|---------------------------|
| R1 – Public S3 Exposure | Critical | Medium |
| R3 – Ransomware | High | Medium |
| R6 – Backup Failure | Medium | Low |
| R9 – Vendor API Exposure | Medium | Medium |

Impact remains high for financial data exposure,
but encryption reduces data usability in case of breach.

Likelihood of successful data exploitation decreases.

---

# 5. Governance Reflection

Encryption is mandatory but not sufficient.

Key considerations:

- Key rotation policy required
- Access logging for key usage required
- Encryption must be enforced automatically
- Backup encryption must match production standards

In financial services, encryption failure is considered governance failure.

Data protection must assume breach and reduce impact severity.

Encryption shifts risk from catastrophic to manageable.
