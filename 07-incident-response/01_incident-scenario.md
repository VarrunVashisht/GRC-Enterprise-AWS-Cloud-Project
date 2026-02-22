# Incident Scenario  
## IAM Credential Compromise & Ransomware Deployment  
### Southern Cross Capital Pty Ltd – Simulated Incident

---

# 1️⃣ Incident Overview

**Incident Type:** IAM Credential Compromise + Ransomware  
**Date:** Simulated  
**Environment:** AWS Production  
**Assets Impacted:**  
- Trading Platform EC2 Instance  
- S3 Backup Storage  
- IAM Administrative Role  

This incident simulates a targeted phishing attack resulting in cloud account compromise and ransomware deployment.

The scenario demonstrates structured incident response aligned with financial services governance expectations.

---

# 2️⃣ Attack Timeline

---

## 1️⃣ Phishing Email Delivered

An employee with privileged IAM access receives a phishing email disguised as an AWS security notification.

The email contains a link to a fake login page.

---

## 2️⃣ IAM Credentials Captured

Employee enters credentials into fake portal.

Attacker obtains:

- IAM username
- Password
- (MFA not enforced in this simulated scenario)

---

## 3️⃣ Attacker Accesses AWS Console

CloudTrail logs later confirm:

- Login from foreign IP address
- Login outside normal business hours
- First-time access from unusual geographic location

---

## 4️⃣ Privilege Escalation

The compromised IAM account has over-permissive AdministratorAccess policy.

Attacker escalates privileges and gains broad control of:

- EC2
- S3
- IAM roles
- Backup configurations

---

## 5️⃣ Backup Deletion

Attacker deletes:

- Recent S3 backup objects
- EC2 snapshots

CloudTrail records delete API calls.

---

## 6️⃣ Ransomware Deployment

Attacker:

- Accesses EC2 trading instance
- Installs malicious encryption script
- Encrypts application data

Trading platform becomes unavailable.

---

## 7️⃣ Service Disruption

Customers unable to access trading portal.

Customer support receives outage complaints.

Operational disruption escalates to IT leadership.

---

# 3️⃣ Detection

Incident detected through multiple signals:

---

### CloudTrail Alerts

- Unusual login from foreign IP
- IAM role modifications
- Backup deletion API calls

---

### CloudWatch Monitoring

- EC2 CPU spike
- Unusual file modification patterns
- Service health check failures

---

### Business Signal

- Customer complaints about trading platform outage
- Internal system alerts

Detection time: Within 30–60 minutes of compromise.

---

# 4️⃣ Immediate Containment Actions

Upon confirmation of incident:

---

## Account Containment

- Disabled compromised IAM account
- Revoked active sessions
- Rotated IAM credentials

---

## Infrastructure Containment

- Isolated affected EC2 instance from network
- Blocked suspicious IP addresses
- Disabled API keys

---

## Evidence Preservation

- Preserved CloudTrail logs
- Preserved EC2 instance snapshot for forensic review
- Exported relevant monitoring logs

---

# 5️⃣ Eradication

Once containment confirmed:

- Removed malicious scripts
- Conducted malware scan
- Reviewed IAM policies
- Patched identified vulnerabilities
- Enforced MFA on all privileged accounts

Compromised credentials fully revoked.

---

# 6️⃣ Recovery

---

## System Restoration

- Restored EC2 instance from secure, clean image
- Restored S3 backups (if available)
- Revalidated encryption and configuration settings

---

## Validation

- Conducted integrity checks
- Confirmed no persistence mechanisms
- Verified IAM policy corrections

---

## Service Resumption

- Trading platform brought back online
- Customer notification issued
- System monitored continuously for 72 hours

---

# 7️⃣ Escalation & Governance

Given this is a financial services environment:

- Incident escalated to Executive Leadership
- Board notified of potential regulatory impact
- Legal team consulted regarding breach notification obligations
- Regulatory impact assessment initiated (Privacy Act + APRA CPS 234)

---

# 8️⃣ Incident Severity Classification

Severity: Critical

Justification:

- Production trading platform outage
- Backup compromise
- Financial data exposure risk
- Regulatory reporting implications

---

# 9️⃣ Incident Response Lifecycle Demonstrated

Identification  
→ Containment  
→ Eradication  
→ Recovery  
→ Post-Incident Review  

This structured approach reflects mature incident response governance aligned with financial sector expectations.

Security maturity is not measured by absence of incidents,
but by structured and disciplined response.
