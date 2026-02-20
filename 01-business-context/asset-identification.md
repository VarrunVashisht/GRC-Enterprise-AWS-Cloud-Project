# Asset Identification & Criticality Assessment  
## Southern Cross Capital Pty Ltd

---

## 1. Critical Business Assets

This document identifies and evaluates the most critical assets of Southern Cross Capital Pty Ltd as part of the enterprise cloud risk assessment process.

Each asset is assessed based on:

- Business importance  
- Impact if compromised  
- Financial consequences  
- Regulatory implications  
- Overall criticality level  

The purpose of this assessment is to support structured risk analysis in later phases of the project.

---

## A. Customer Financial Data  
**Criticality: Very High**

### Description

Customer Financial Data includes:

- Bank account details  
- Investment balances  
- Transaction history  
- Personal identity information (PII)  
- Tax file numbers and financial identifiers  

This data is stored within cloud-hosted databases and accessed via the online trading platform.

---

### Why This Asset Is Important

This is the core business asset of the organisation.  
Without customer financial data, the company cannot operate its trading, investment, or advisory services.

Customer trust is directly linked to the protection of this information.

---

### What Happens If Compromised

If exposed or manipulated:

- Unauthorised financial transactions may occur  
- Identity theft risks increase  
- Fraudulent trading activity may be executed  
- Data integrity may be questioned  
- Customer confidence may collapse  

This would trigger immediate crisis management and regulatory reporting.

---

### Financial Impact

- Direct financial losses due to fraud  
- Compensation to affected customers  
- Legal costs  
- Incident response and forensic investigation expenses  
- Increased cyber insurance premiums  
- Potential long-term loss of revenue due to customer churn  

Impact level: Severe

---

### Regulatory Impact

- Mandatory reporting under the Australian Notifiable Data Breaches (NDB) Scheme  
- Potential penalties under the Privacy Act  
- APRA CPS 234 compliance review  
- Increased regulatory oversight  

This type of breach would attract regulatory scrutiny at board level.

---

## B. Trading Platform Application  
**Criticality: Very High**

### Description

The trading platform consists of:

- Web servers (EC2 instances)  
- Backend API services  
- Authentication and access control services  
- Real-time market data integrations  

This platform enables customers to execute trades and manage portfolios.

---

### Why This Asset Is Important

The trading platform is the primary revenue-generating system.

If the platform is unavailable or compromised, customers cannot execute trades, leading to financial loss and reputational damage.

---

### What Happens If Compromised

- Trading manipulation or fraud  
- Platform downtime  
- Denial-of-service attacks  
- Customer account takeover  
- Market integrity risks  

Even short downtime can result in financial and legal consequences.

---

### Financial Impact

- Loss of transaction revenue  
- SLA penalties  
- Customer compensation  
- Business interruption losses  

Impact level: Severe

---

### Regulatory Impact

- APRA information security review  
- Market conduct investigations  
- Potential financial regulatory penalties  

Given the financial services environment, availability and integrity are legally significant.

---

## C. Cloud Infrastructure  
**Criticality: High**

### Description

Cloud infrastructure includes:

- AWS account configuration  
- IAM roles and permission structures  
- S3 storage  
- VPC networking  
- Security groups and firewall rules  
- CloudTrail logging  

This infrastructure supports all production systems.

---

### Why This Asset Is Important

Cloud infrastructure is the foundation of all digital operations.

Misconfiguration at this layer can expose multiple systems simultaneously.

---

### What Happens If Compromised

- Cloud account takeover  
- Data exfiltration  
- Ransomware deployment  
- Infrastructure manipulation  
- Loss of system visibility  

Compromise at infrastructure level can cascade across all services.

---

### Financial Impact

- Full operational shutdown  
- System rebuild costs  
- Extended downtime  
- Incident response expenses  

Impact level: High to Severe

---

### Regulatory Impact

- Breach notification obligations  
- APRA scrutiny for inadequate security controls  
- Compliance failure under CPS 234  

Cloud governance is therefore a critical control area.

---

## D. Internal Administrative Systems  
**Criticality: Medium–High**

### Description

Internal systems include:

- HR management platform  
- Payroll data  
- Employee identity credentials  
- Internal audit and compliance documentation  

These systems are used by internal staff and management.

---

### Why This Asset Is Important

Although not customer-facing, internal systems support business continuity and regulatory compliance.

Compromised employee credentials can become attack entry points.

---

### What Happens If Compromised

- Insider threat risk  
- Privilege escalation  
- Social engineering attack leverage  
- Disruption of payroll operations  

Internal system compromise can indirectly impact customer-facing services.

---

### Financial Impact

- Payroll errors  
- Investigation costs  
- Operational disruption  

Impact level: Moderate to High

---

### Regulatory Impact

- Potential employee data breach reporting  
- Internal audit non-compliance findings  

While not as severe as customer data compromise, this still carries regulatory exposure.

---

## E. Backup & Disaster Recovery Systems  
**Criticality: Very High**

### Description

Backup and disaster recovery systems include:

- Automated database backups  
- S3 backup storage  
- Recovery testing procedures  
- Business continuity planning documentation  

These systems ensure operational resilience.

---

### Why This Asset Is Important

Backups are the last line of defence against ransomware, system failure, or data corruption.

Without reliable backups, recovery may be impossible.

---

### What Happens If Compromised

- Permanent data loss  
- Inability to restore systems  
- Extended service outage  
- Regulatory investigation for lack of resilience  

Backup compromise significantly increases business risk.

---

### Financial Impact

- Extended downtime costs  
- Revenue loss  
- Recovery infrastructure expenses  
- Potential business collapse in extreme cases  

Impact level: Severe

---

### Regulatory Impact

- APRA CPS 234 failure due to inadequate resilience  
- Increased supervisory scrutiny  
- Board accountability implications  

Backup governance is therefore classified as a board-level risk control requirement.

---

## Summary of Asset Criticality

| Asset | Criticality Level |
|-------|-------------------|
| Customer Financial Data | Very High |
| Trading Platform Application | Very High |
| Cloud Infrastructure | High |
| Internal Administrative Systems | Medium–High |
| Backup & Disaster Recovery Systems | Very High |

This structured asset identification provides the foundation for the next phase: Threat Modeling and Risk Assessment.
