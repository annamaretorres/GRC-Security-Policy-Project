# Acceptable Use Policy v1.0

**Author:** Anna Marie Torres  
**Date:** June 2026  
**Framework:** NIST SP 800-53  
**Scope:** Fintech organization handling customer PII, financial transactions, and regulated business data

---

## Purpose
This policy defines acceptable use of company systems, devices, and data to protect the organization from security risks and ensure compliance with applicable regulations including FCRA, SBA guidelines, and internal fintech compliance standards.

---

## Scope
This policy applies to:
- All employees and contractors with system access
- Third party vendors handling customer PII
- Any individual accessing company financial systems, case management tools, or customer data

---

## Acceptable Use

Users MAY:
- Access systems and data required for their specific job duties only
- Use company tools including Salesforce, Jira, and internal platforms for business purposes
- Report suspicious activity, account anomalies, or policy violations to the compliance team immediately
- Request documentation from customers when identity verification fails during onboarding

---

## Unacceptable Use

Users MAY NOT:
- Share login credentials or access another employee's account
- Access customer PII outside of assigned case work
- Export or share customer data outside of authorized internal systems
- Attempt to override identity verification controls without documented lead approval
- Take action on accounts with Frozen, Suspected, or Deactivated status without following escalation procedures

**Why this matters in fintech:** At a company processing hundreds of thousands of customer accounts, a single unauthorized access incident can trigger FCRA violations, regulatory fines, and customer harm. These restrictions are not bureaucratic — they exist because the consequences of violations are severe and immediate.

---

## Identity Verification & Data Protection Rules

All customer identity data must be handled as follows:

| Data Type | Handling Requirement |
|-----------|---------------------|
| SSN | Never stored in unsecured systems, cross-referenced against verified records only |
| DOB | Verified against government-issued ID before any account action |
| EIN/TIN | Confirmed via SS-4 or IRS documentation before business account approval |
| IP Address | Logged and cross-referenced against known device history for fraud detection |
| Account PII | Accessible only to authorized agents on assigned cases |

**Real world context:** These controls directly reflect the identity verification procedures used during Square Banking KYC/CIP onboarding — where mismatches in any of these data points triggered mandatory manual review before any account action could be taken.

---

## Violation Consequences

| Severity | Example | Consequence |
|----------|---------|-------------|
| Minor | Accessing a case outside your queue | Written warning and retraining |
| Moderate | Sharing login credentials | Suspension pending investigation |
| Serious | Unauthorized PII access or export | Immediate termination and legal referral |
| Critical | Deliberate fraud or regulatory violation | Termination, legal action, regulatory reporting |

---

## Regulatory Alignment

| Regulation | Relevance to This Policy |
|-----------|--------------------------|
| FCRA | Customer data accuracy and dispute handling requirements |
| NIST SP 800-53 | Access control and identity management framework |
| SBA Guidelines | PPP loan documentation and fraud prevention standards |
| Internal Compliance Standards | Case management, escalation, and documentation procedures |

---

## Key Decision: What This Policy Excludes
This policy does not govern third party vendor access controls or supply chain risk — those require a separate vendor risk management framework. Scope boundaries are documented intentionally to avoid creating false compliance coverage.

---

## Author Note
This policy was developed using NIST SP 800-53 access control guidelines and reflects real compliance experience managing customer data at Block Inc across Cash App and Square Banking. The identity verification controls, violation consequences, and data handling requirements are directly informed by operational procedures used daily in a regulated fintech environment processing 500+ cases monthly.
