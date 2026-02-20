# Data Classification Model  
## Southern Cross Capital Pty Ltd

---

## 1. Purpose of Data Classification

The purpose of this data classification model is to categorise information assets based on sensitivity, regulatory requirements, and business impact if compromised.

Data classification supports:

- Risk prioritisation  
- Access control decisions  
- Encryption requirements  
- Monitoring intensity  
- Regulatory compliance  
- Incident response severity determination  

Proper classification ensures that the most sensitive data receives the highest level of protection.

---

## 2. Data Classification Levels

Southern Cross Capital adopts a four-tier data classification model:

1. Public  
2. Internal  
3. Confidential  
4. Highly Confidential  

Each level determines required security controls and handling procedures.

---

## 3. Classification Levels Defined

---

### 3.1 Public

**Definition:**  
Information approved for public release that does not cause harm if disclosed.

**Examples:**
- Marketing website content  
- Public product brochures  
- Press releases  
- Public investor announcements  

**Security Requirements:**
- Integrity protection  
- Basic access control  
- Monitoring for defacement  

**Business Impact if Compromised:**
Low (primarily reputational)

---

### 3.2 Internal

**Definition:**  
Information intended for internal organisational use that is not publicly distributed but does not cause severe harm if exposed.

**Examples:**
- Employee directory  
- Internal policies  
- Internal meeting notes  
- Non-sensitive operational documentation  

**Security Requirements:**
- Role-based access control  
- Internal network restriction  
- Basic logging  

**Business Impact if Compromised:**
Moderate (operational disruption or reputational concern)

---

### 3.3 Confidential

**Definition:**  
Sensitive business information that could cause financial, operational, or regulatory impact if disclosed without authorisation.

**Examples:**
- Internal audit reports  
- Risk assessment reports  
- Financial forecasts  
- Vendor contracts  
- Security architecture documentation  

**Security Requirements:**
- Strict access control (least privilege)  
- Encryption at rest and in transit  
- Access logging and monitoring  
- Regular review of permissions  

**Business Impact if Compromised:**
High (financial, regulatory, or competitive damage)

---

### 3.4 Highly Confidential

**Definition:**  
Critical data that would cause severe financial loss, regulatory penalties, or major reputational damage if compromised.

This classification applies to data protected under Australian Privacy and financial regulations.

**Examples:**
- Customer financial data  
  - Bank account details  
  - Investment balances  
  - Transaction history  
- Personal identity information (PII)  
- Authentication credentials  
- API keys  
- IAM access keys  
- Database encryption keys  
- Payroll-linked financial records  

**Security Requirements:**
- Multi-factor authentication (MFA)  
- Strict least-privilege IAM controls  
- Encryption at rest and in transit  
- Continuous monitoring and logging  
- Data loss prevention controls  
- Backup protection and isolation  

**Business Impact if Compromised:**
Severe  
- Financial fraud  
- Regulatory penalties  
- APRA CPS 234 compliance review  
- Mandatory data breach notification  
- Customer trust erosion  

---

## 4. Data Classification Mapping for Southern Cross Capital

| Data Type | Classification Level |
|------------|---------------------|
| Marketing Website Content | Public |
| Employee Directory | Internal |
| Internal Audit Reports | Confidential |
| Risk Assessment Reports | Confidential |
| Vendor Security Contracts | Confidential |
| Customer Financial Data | Highly Confidential |
| Authentication Credentials | Highly Confidential |
| API Keys & Access Tokens | Highly Confidential |
| Payroll-Linked Investment Data | Highly Confidential |
| Cloud Infrastructure Secrets | Highly Confidential |

---

## 5. Why Data Classification Matters

Data classification is a foundational component of enterprise risk management.

It ensures:

### 1. Risk-Based Protection
Resources are allocated according to data sensitivity.  
Highly Confidential data receives the strongest controls.

### 2. Regulatory Compliance
Australian regulations require enhanced protection of personal and financial data.  
Classification ensures compliance obligations are met.

### 3. Access Governance
Only authorised individuals can access sensitive data, reducing insider threat risk.

### 4. Encryption & Control Prioritisation
Encryption policies and monitoring levels are determined based on classification.

### 5. Incident Severity Determination
If a Highly Confidential asset is breached, incident response escalates immediately to executive level.

---

## 6. Strategic Importance

In a financial services organisation, most core operational data falls under the "Highly Confidential" category.

This means:

- Cloud configuration errors pose serious risk.
- IAM mismanagement can have severe consequences.
- Backup security must match primary system sensitivity.
- Continuous monitoring is mandatory.

This classification model will directly inform the next phase:
Threat Modeling and Risk Assessment.

Data classification ensures that risk scoring reflects true business impact.
