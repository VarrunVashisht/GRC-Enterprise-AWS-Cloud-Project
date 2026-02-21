# Risk Assessment Methodology  
## Southern Cross Capital Pty Ltd  
### AWS Cloud Migration – Financial Services Risk Model

---

## 1️⃣ Risk Assessment Approach

Southern Cross Capital adopts a **qualitative risk scoring model** aligned with enterprise risk management practices commonly used in financial services.

The core formula used is:

> **Risk = Likelihood × Impact**

This model enables structured evaluation of cyber risks associated with cloud migration.

The purpose of this methodology is to:

- Ensure consistent risk scoring  
- Prioritise mitigation efforts  
- Support executive decision-making  
- Align with regulatory expectations (APRA CPS 234)  
- Enable transparent governance reporting  

---

### Scoring Range

Both Likelihood and Impact are scored on a scale of **1 to 5**.

This produces a total risk score range of:

**Minimum:** 1  
**Maximum:** 25  

This approach supports structured categorisation into Low, Medium, High, and Critical risk tiers.

---

## 2️⃣ Likelihood Scale (1–5)

Likelihood measures the probability of a threat exploiting a vulnerability within the cloud environment.

In the context of AWS cloud security, likelihood considers:

- Exposure level  
- Ease of exploitation  
- Industry attack frequency  
- Existing control maturity  
- Historical breach trends  

---

### Likelihood Rating Definitions

| Score | Description | Cloud Context Interpretation |
|-------|-------------|-----------------------------|
| 1 | Rare | Highly unlikely to occur. Strong controls exist and no known similar incidents in comparable organisations. |
| 2 | Unlikely | Possible but not expected. Controls are generally strong with limited exposure. |
| 3 | Possible | Has occurred in similar organisations. Some weaknesses or exposure exist. |
| 4 | Likely | Regularly observed in the industry. Controls are weak or inconsistently enforced. |
| 5 | Almost Certain | Frequently occurring in financial services. Vulnerability is exposed or easily exploitable. |

---

### Example in Cloud Context

**Likelihood = 4 (Likely)**

Example: Public S3 bucket exposure.

Cloud misconfiguration is one of the most common causes of data breaches globally.  
If automated scanning tools are widespread and no monitoring exists, exploitation is considered likely.

---

## 3️⃣ Impact Scale (1–5)

Impact measures the business consequence if the risk materialises.

Impact is assessed across four dimensions:

- Financial loss  
- Regulatory penalties  
- Operational downtime  
- Reputational damage  

The highest severity category determines the overall impact score.

---

### Impact Rating Definitions

| Score | Description | Business Impact Interpretation |
|-------|-------------|--------------------------------|
| 1 | Minimal | Minor inconvenience. No financial loss. No regulatory involvement. |
| 2 | Minor | Limited operational disruption. Small financial cost. No regulatory reporting required. |
| 3 | Moderate | Noticeable financial loss. Limited customer impact. Possible regulatory inquiry. |
| 4 | Major | Significant financial loss. Service disruption. Regulatory investigation likely. |
| 5 | Severe | Multi-million dollar impact. Mandatory regulatory breach notification. Major reputational damage. Board-level crisis. |

---

### Example in Financial Services Context

**Impact = 5 (Severe)**

Example: Exposure of customer financial records.

Consequences may include:

- Regulatory breach under Privacy Act  
- APRA CPS 234 investigation  
- Customer lawsuits  
- Loss of investor confidence  
- Long-term revenue decline  

This qualifies as Severe due to regulatory, financial, and reputational magnitude.

---

## 4️⃣ Risk Rating Categories

After calculating:

> Risk Score = Likelihood × Impact

The resulting value is categorised as follows:

| Risk Score | Risk Level | Governance Action |
|------------|------------|------------------|
| 1–5 | Low | Acceptable risk. Monitor periodically. |
| 6–10 | Medium | Mitigation recommended. Management oversight required. |
| 11–15 | High | Action required. Senior management review. |
| 16–25 | Critical | Immediate remediation required. Board-level visibility. |

---

### Example Calculation

If:

Likelihood = 4 (Likely)  
Impact = 5 (Severe)

Risk Score = 4 × 5 = 20  

Risk Level = Critical  

This requires immediate mitigation and executive reporting.

---

## Governance Principle

This structured methodology ensures that:

- Risks are prioritised based on business impact, not technical fear.
- Control investments align with risk severity.
- Executive leadership can make informed decisions.
- Regulatory scrutiny can be addressed with documented methodology.

Risk assessment must be:

Consistent.  
Repeatable.  
Defensible.  

This methodology will now be applied to all identified attack scenarios to calculate:

- Inherent Risk  
- Control Effectiveness  
- Residual Risk  

Quantification transforms threat awareness into governance action.
