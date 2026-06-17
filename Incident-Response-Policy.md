# Incident Response Policy v1.0

**Author:** Anna Marie Torres  
**Date:** June 2026  
**Framework:** NIST SP 800-61r2  
**Scope:** Fintech environment handling customer PII, financial transactions, and regulated data

---

## Purpose
This policy establishes structured procedures for identifying, managing, and responding to cybersecurity incidents to minimize operational, financial, and reputational impact.

---

## Incident Classification

| Tier | Severity | Example | Response |
|------|----------|---------|----------|
| Tier 1 | Critical | Data breach, ransomware, legal exposure, unauthorized PII access | Legal + Management notified immediately |
| Tier 2 | High | Phishing attempt, unauthorized login, suspicious account activity | Senior Analyst investigates within 24 hours |
| Tier 3 | Low | Spam emails, minor policy violations, non-malicious anomalies | Junior Analyst logs and monitors |

**Why this classification matters:** In a high-volume fintech environment processing 500+ complaints monthly, misclassifying a Tier 1 incident as Tier 3 creates direct FCRA and regulatory exposure. The tiering system exists to protect the organization legally, not just operationally.

---

## Incident Response Lifecycle (NIST SP 800-61r2)

### 1. Detect
Analyst reviews incoming case and assesses severity based on complaint language, account history, and identity indicators. In practice this means reading between the lines — a customer saying "someone changed my email" is not a Tier 3 complaint.

### 2. Contain
Flag the account, halt suspicious transactions, and prevent further access pending investigation. No action taken on accounts with Frozen or Suspected status until status is resolved.

### 3. Eradicate
Remove unauthorized access, reverse fraudulent transactions where applicable, and document all actions taken with timestamps in the case management system.

### 4. Recover
Restore account access only after identity is re-verified. Communicate resolution to affected customer per FCRA guidelines and internal SLA requirements.

### 5. Report
Document every step — what was found, what decision was made, why, and what the outcome was. In a regulated environment, undocumented decisions are treated as no decision at all.

---

## Escalation Procedures

| Tier | Escalation Path | Timeframe |
|------|----------------|-----------|
| Tier 1 | Legal team + Senior Management notified immediately | Within 1 hour |
| Tier 2 | Senior Analyst assigned, escalation if unresolved | Within 24 hours |
| Tier 3 | Logged in case management, reviewed in routine audit | Within 5 business days |

---

## Identity Verification Controls
During any incident involving account access, the following must be cross-referenced before any account action is taken:

- SSN match against verified records
- DOB match against government-issued ID
- EIN/TIN match for business accounts
- IP address origin vs known device history
- Alias and name variant review

**Real world context:** These controls directly mirror the KYC/CIP verification procedures used during Square Banking onboarding — where a single SSN or DOB mismatch was sufficient to halt an application pending documentation review.

---

## Regulatory Alignment

| Regulation | Relevance |
|-----------|-----------|
| NIST SP 800-61r2 | Incident response lifecycle framework |
| FCRA | Customer dispute and data accuracy requirements |
| SBA Guidelines | PPP loan compliance and fraud documentation standards |
| Internal Compliance Standards | Tier classification and escalation procedures |

---

## Key Decision: What This Policy Excludes
This policy does not cover third-party vendor incidents or supply chain risk — those require a separate vendor risk management framework. Acknowledging scope boundaries is part of credible GRC documentation.

---

## Author Note
This policy was developed using NIST SP 800-61r2 as the foundational framework and reflects real incident triage decisions made while reviewing 25+ cases daily at Block Inc. The Tier classification system, escalation timeframes, and identity verification controls are directly informed by operational experience — not templated from a course.
