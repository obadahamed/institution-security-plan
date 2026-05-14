# **BIA**

---
## 1. Objective

This analysis aims to identify Al Noor Bank's critical operations and estimate the impact of their disruption, enabling management to develop effective recovery plans and ensure business continuity.

---

## 2. Scope

This analysis encompasses all critical operations at Al Noor Bank, including banking services, payments, ATMs, and the IT infrastructure at the head office and branches.

---

## 3. **Methodology:** How the BIA was conducted

This analysis was prepared in the following stages:

**Stage 1 — Identifying Critical Operations:** The bank's core operations were identified through an analysis of daily workflows and a review of systems and IT infrastructure, focusing on operations whose disruption would have a direct impact on customers or financial obligations.

**Stage 2 — Determining RTO and RPO:** For each critical operation, the maximum acceptable downtime (RTO) and maximum potential data loss (RPO) were determined, based on the nature of the operation and the expected extent of the damage.

**Stage 3 — Estimating Losses:** Potential losses for each transaction were categorized into four types: direct financial, reputational and trust losses, cumulative operational losses, and legal and regulatory losses.

**Phase 4 — Defining the Recovery Strategy:** Based on the results of the previous phases, a clear recovery plan was developed for each transaction, outlining the procedures, responsibilities, and timelines.

---

## 4. Critical Operations + RTO/RPO

| Service | RTO | RPO |
| ------------------------------- | ------- | ------ |
| Core Banking Services | 2 hours | 1 hour |
| Payment Systems | 3 hours | 1 hour |
| ATM Network | 5 hours | 2 hours |
| Inter-Branch Communication | 1 day | 1 hour |
| Databases and Backup | 1 hour | 1 hour |

---

## 5. Loss Estimation

### 1. Core Banking Services

1. Direct Financial Losses

- **Compensation Benefits:** The bank's obligation to pay interest or late payment penalties on investment transactions and corporate transfers. Major breaches that were not completed on time.

1. Reputational Losses

- **Digital Panic:** Two hours is enough for the news to spread like wildfire on social media. Customers will assume a "massive cyberattack," damaging the bank's public image.

- **Churn Rate Loss:** New customers or companies that have experienced previous disruptions may immediately decide to transfer their accounts and credit facilities to competing banks that offer greater stability.

3. Operational Backlog Losses

- **Transaction Backlog:** A long queue of pending financial transactions (deposits, loans, settlements) will accumulate within two hours.

4. Regulatory Penalties

- **Service Agreement (SLA) Violation:** Banks are bound by specific operational ratios (typically 99.9%) to central banks and regulatory bodies.

- **Immediate Fines:** The central bank may impose direct financial penalties on a bank for failing to provide continuous service.

### 2. Payment Systems

- **Immediate Liquidity Crisis:** A RTGS outage prevents banks from exchanging cash with each other, potentially leading to the bank defaulting on its daily obligations to the central bank.

- **Business Paralysis:** Businesses stop receiving payments for their sales or paying suppliers, disrupting supply and shipping chains.

- **Salary Freeze and Government Transactions:** An ACH network outage delays the salaries of thousands of employees and prevents the collection of taxes or vital government payments.

### 3. ATM Network

- **Bank Run:** People's inability to withdraw their money immediately generates rumors of bank failure or a catastrophic breach, prompting customers to rush to branches for cash.

- **Loss of Interchange Fees:** The bank loses the fees earned when customers of other banks use its network and incurs additional costs if its customers are forced to withdraw from competing banks.

- **SLA Penalties:** ATMs are bound by strict maintenance and operation contracts; a mass outage means a failure of the operational indicators agreed upon with the service providers and the central bank.

### 4. Branch Communication

- **Core Banking System Freeze:** Tellers cannot see customers' current balances, completely preventing withdrawals or deposits.

- **Check Issuance and Transfers Halted:** Clearing requests and instant transfers cannot be processed due to the inability to verify signatures or balances.

- **Account and Loan Opening Halted:** KYC (Know Your Customer) and credit systems linked to the head office are down.

- **Surveillance Cameras and Security Systems Failed:** Central security loses the ability to monitor the branch via live feed, creating a serious physical security vulnerability.

### 5. Databases and Backup

- **Impossibility of Restoring Trust:** If customer balance data is lost, even for a few hours, the bank's reputation is permanently damaged and cannot be compensated with any amount of money.

- **Criminal Penalties Supervision: Central banks and compliance authorities impose very strict penalties (which may include suspending the bank's license) if negligence is found in data protection and historical data retention.

---

## 6. Recovery Strategy

Recovery Strategy Matrix

| Banking Operation | Recovery Strategy | Owner | Expected RTO |
| :--- | :--- | :--- | :--- |
| **Core Banking Services** | Automatically divert traffic to the backup server (failover) and verify the integrity of accounting entries. | Chief Information Officer (CIO) | 2 Hours |
|**Payment Systems and Swift** | Activate the alternative payment processor and freeze low-value transactions (ACH) to focus on large transfers. | Chief Operating Officer (COO) | 30 minutes |
| **ATM Network** | Temporarily suspend the central network and direct customers to branches via instant SMS notifications to prevent panic. | Digital Channels Manager | 45 minutes |
| **Branch Connectivity** | Activate emergency lines (MPLS backup or 5G VPN) and operate branches offline in the event of a complete outage. | Networks and Infrastructure Manager | 1 minute (automatic) |
| **Databases and Backup** | Restore data from immutable backups and perform instant reconciliation. | Chief Information Security Officer (CISO) | 1 hour |


---

## 7. Review

1. Periodic Review (Normal Situation)

- **Annually:** This is the standard practice in the banking sector and is recommended under ISO 22301 (Business Continuity Management). It ensures that figures (such as RTO and loss levels) remain realistic and aligned with inflation and the bank's balance sheet.

2. Exceptional Review (Emergency Situation)

The BIA must be updated immediately, without waiting for the annual review, in the following cases:

- **Introduction of New Systems:** When the bank's core banking system is changed, or when cloud technologies or new payment applications are adopted.

- **Structural Changes in the Bank:** Such as merging departments, closing major branches, or expanding into new markets.

- **After a Real-Life Disaster:** If the bank experiences a major outage or cyberattack, the BIA must be reviewed to compare "expected losses" with "actual losses" and adjust the strategy based on lessons learned. - **Updates to Laws and Regulations:** If the Central Bank issues new instructions requiring banks to meet faster recovery targets or more complex security standards.

---

_Al Noor Bank for Finance and Investment — Confidential Internal Document_ _Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)_
