---
name: finance-audit-support
description: Support SOX 404 compliance with control testing methodology, sample selection, and documentation standards. Use when generating testing workpapers, selecting audit samples, classifying control deficiencies, or preparing for internal or external audits.
author: Perplexity
version: '1.0'
---

# Audit Support

SOX 404 control testing methodology, sample selection approaches, testing documentation standards, control deficiency classification, and common control types.

## SOX 404 Control Testing Methodology

### Overview

SOX Section 404 requires management to assess the effectiveness of internal controls over financial reporting (ICFR):

1. **Scoping:** Identify significant accounts and relevant assertions
2. **Risk assessment:** Evaluate the risk of material misstatement
3. **Control identification:** Document the controls that address each risk
4. **Testing:** Test the design and operating effectiveness of key controls
5. **Evaluation:** Assess whether any deficiencies exist and their severity
6. **Reporting:** Document the assessment and any material weaknesses

## Scoping Significant Accounts

**Quantitative factors:**
- Account balance exceeds materiality threshold (typically 3-5%)
- Transaction volume is high
- Account is subject to significant estimates or judgment

**Qualitative factors:**
- Complex accounting (revenue recognition, derivatives, pensions)
- Susceptible to fraud (cash, revenue, related-party transactions)
- Prior misstatements or audit adjustments
- New account or significantly changed process

## Sample Selection Approaches

### Random Selection
- Default method for transaction-level controls with large populations
- Use a random number generator to select sample items
- Advantages: Statistically valid, defensible, no selection bias

### Targeted (Judgmental) Selection
- High dollar amount, unusual transactions, period-end transactions
- Related-party, manual or override transactions
- Advantages: Focuses on highest-risk items

### Sample Size Guidance

| Control Frequency | Low Risk | Moderate Risk | High Risk |
|---|---|---|---|
| Annual | 1 | 1 | 1 |
| Quarterly | 2 | 2 | 3 |
| Monthly | 2 | 3 | 4 |
| Weekly | 5 | 8 | 15 |
| Daily | 20 | 30 | 40 |
| Per-transaction (large pop.) | 25 | 40 | 60 |

## Control Deficiency Classification

### Deficiency
A gap in control design or operation that doesn't allow timely prevention or detection of misstatements.

### Significant Deficiency
A deficiency less severe than a material weakness yet important enough to merit attention by governance.

### Material Weakness
A deficiency where there is a reasonable possibility that a material misstatement will not be prevented or detected on a timely basis.

**Indicators of Material Weakness:**
- Identification of fraud by senior management
- Restatement of previously issued financial statements
- Identification by the auditor of a material misstatement not detected by controls
- Ineffective oversight by the audit committee

## Common Control Types

### IT General Controls (ITGCs)
- **Access Controls**: User access provisioning/de-provisioning, privileged access, periodic reviews
- **Change Management**: Change requests, testing, separation of dev/prod environments
- **IT Operations**: Batch job monitoring, backup and recovery, incident management

### Manual Controls
Performed by people using judgment - review and approval:
- Management review of financial statements
- Supervisory approval of journal entries above a threshold
- Three-way match verification (PO, receipt, invoice)
- Account reconciliation preparation and review

### Automated Controls
Enforced by IT systems without human intervention:
- System-enforced approval workflows
- Duplicate payment detection
- Credit limit enforcement
- Automated calculations (depreciation, amortization)
