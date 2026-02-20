# Attack Scenarios  
## Southern Cross Capital Pty Ltd  
### Cloud Risk Simulation – Financial Services Environment

---

## Purpose of This Document

This document simulates realistic cyber attack scenarios that could impact Southern Cross Capital during or after its migration to AWS.

Each scenario includes:

- Attack flow description  
- Technical pathway  
- Business impact  
- Financial consequences  
- Regulatory implications  

These scenarios will later be converted into formal risk entries in the risk register.

---

# SCENARIO 1 — Public S3 Bucket Data Exposure

## Scenario Description

An S3 bucket storing customer transaction history is misconfigured during cloud migration.

Public read access is mistakenly enabled.

An external attacker discovers the exposed bucket using automated cloud scanning tools.

Sensitive data is downloaded and later sold on dark web marketplaces.

---

## Attack Flow

1. Cloud engineer creates S3 bucket.
2. Public access block settings are not enforced.
3. Bucket policy allows public read access.
4. Automated scanning tools detect exposed bucket.
5. Attacker downloads transaction history files.
6. Data appears for sale online.

---

## Assets Impacted

- Customer financial data
- Personal identity information
- Transaction history
- Corporate reputation

---

## Business Impact

- Immediate data breach declaration
- Customer notification requirement
- Media exposure
- Loss of customer confidence

---

## Financial Impact

- Regulatory penalties under Privacy Act
- APRA CPS 234 compliance investigation
- Incident response and forensic costs
- Customer compensation claims
- Potential class-action lawsuits

Impact Severity: Severe

---

## Regulatory Impact

- Mandatory breach notification under Australian Notifiable Data Breaches (NDB) Scheme
- APRA supervisory review
- Increased regulatory oversight
- Board accountability review

---

# SCENARIO 2 — IAM Credential Compromise & Ransomware Deployment

## Scenario Description

An employee receives a phishing email disguised as an internal AWS alert.

The employee unknowingly enters credentials into a fake login page.

The attacker uses stolen IAM credentials to access the AWS environment.

Privileges are escalated due to over-permissive IAM roles.

Backups are deleted, and ransomware is deployed on EC2 instances.

---

## Attack Flow

1. Phishing email sent to privileged employee.
2. Employee submits credentials to fake portal.
3. Attacker logs into AWS console.
4. Privilege escalation via weak IAM policies.
5. Backup deletion in S3.
6. Ransomware deployed on EC2 servers.
7. Trading platform becomes unavailable.

---

## Assets Impacted

- Cloud infrastructure
- EC2 trading servers
- Backup systems
- Customer transaction services

---

## Business Impact

- Complete service outage
- Trading suspension during market hours
- Operational shutdown
- Emergency incident response activation

---

## Financial Impact

- Direct revenue loss
- Customer compensation claims
- Recovery infrastructure costs
- Potential ransom payment
- Long-term reputational damage

Impact Severity: Severe

---

## Regulatory Impact

- APRA review for insufficient security controls
- Investigation into MFA enforcement failure
- Questions regarding IAM governance
- Potential enforcement action

---

# SCENARIO 3 — Insider Data Theft

## Scenario Description

A privileged system administrator exports a high-value customer investment list.

The data includes client financial profiles and investment strategies.

The employee sells this information to a competitor.

The breach is later discovered during an internal audit.

---

## Attack Flow

1. Admin accesses customer database.
2. Data exported without detection.
3. Data transferred externally.
4. Competitor gains sensitive insights.
5. Incident identified during periodic review.

---

## Assets Impacted

- Customer financial data
- Investment strategy data
- Confidential internal business information

---

## Business Impact

- Competitive disadvantage
- Customer distrust
- Internal investigation
- Legal escalation

---

## Financial Impact

- Loss of high-value clients
- Legal defence costs
- Regulatory fines
- Shareholder impact

Impact Severity: High to Severe

---

## Regulatory Impact

- Privacy breach obligations
- Internal governance review
- APRA compliance investigation
- Increased monitoring requirements

---

# SCENARIO 4 — Distributed Denial of Service (DDoS) on Trading Platform

## Scenario Description

A botnet targets the online trading platform during peak market hours.

The web application becomes overwhelmed by traffic.

Customers are unable to execute trades.

---

## Attack Flow

1. Botnet sends large volume of requests.
2. Web application servers become overloaded.
3. System response times degrade.
4. Trading platform becomes unavailable.
5. Customers experience financial losses.

---

## Assets Impacted

- Online trading platform
- Customer access portal
- Revenue-generating services

---

## Business Impact

- Trading disruption
- Customer dissatisfaction
- Emergency mitigation response
- Media coverage

---

## Financial Impact

- Direct transaction revenue loss
- Customer compensation claims
- SLA penalties
- Reputational damage affecting future growth

Impact Severity: High

---

## Regulatory Impact

- Investigation into resilience controls
- Business continuity plan review
- Board-level scrutiny

---

# Strategic Insight

These attack scenarios demonstrate:

- Cloud misconfiguration risk
- Identity governance weaknesses
- Insider threat exposure
- Availability and resilience challenges

In financial services, cyber incidents are not just technical failures — they are business and regulatory crises.

These scenarios will now be used to:

- Assign likelihood and impact scores
- Calculate inherent risk
- Design control strategies
- Measure residual risk

Next Phase:  
➡️ Risk Methodology & Risk Register Construction
