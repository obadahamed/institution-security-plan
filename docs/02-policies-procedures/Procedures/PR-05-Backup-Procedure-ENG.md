Backup Procedure

|||
|---|---|
|**Procedure Number**|PR-05|
|**Associated Policy**|P-05—Backup Policy|
|**Version**|1.0|
|**Release Date**|02/05/2026|
|**Next Revision Date**|02/05/2027|
|**Procedure Owner**|Information Security Manager|
|**Classification**|Internal|

---

## 1. Purpose

To ensure data recovery in the event of a disaster.

---

## 2. Scope

This procedure applies to the Information Security Manager, the IT Department, and the Information Security Department.

---

## 3. Detailed Steps

### Step 1 — Identification & Scheduling

- **Data Classification:** Identify data (sensitive, critical, public) to determine backup frequency.

- **Defining Copy Types:**

- **Full Copy:** Performed weekly (e.g., every Friday).

- **Incremental Copy:** Performed daily (copies only modifications to save space).

- **Defining Retention Periods:** Configure the system to automatically delete old copies (e.g., after 30 days for daily copies, and 12 months for monthly copies).

### Step 2 — Technical Implementation Procedures

- **Automating Operations:** Configure the backup software (e.g., Veeam or Veritas) to run automatically during off-peak hours (often at night).

- **Applying the 3-2-1 Rule:**

- Maintain **3** copies of the data.

- On two types of media (**2**) (e.g., on-premises server and cloud).

- **1** off-site copy for protection against fire or physical disasters affecting the building.

### Step 3 — Security Measures

- **Encryption:** Encrypt backups with strong encryption keys before transferring them to storage.

- **Air-Gapping:** Completely isolate one backup from the network to prevent ransomware from reaching it.

- **Access Control:** Restrict access to backups to the "Backup Administrator" only.

### Step 4 — Testing & Validation

- **Daily Auditing:** Review system logs every morning to ensure the backup process was successful and address any errors immediately.

- **Periodic Recovery Testing:**

- **Monthly:** Simulate the recovery of random files to verify their integrity.

- **Quarterly:** Simulate the recovery of a full server or a large database to test the plan's readiness.

### Step 5 — Physical Storage and Handling Procedures

- **Suitable Environment:** If backups are on tapes or physical hard drives, they must be stored in a fireproof safe and away from magnetic fields.

- **Labeling:** Place clear labels on the physical media indicating the date, content, and security classification.

### Step 6 — Emergency and Restoration Procedures

- **Restore Request:** Establish an official form for employees to complete when they need to restore a lost file, with their manager's approval.

- **Priority:** In the event of a complete system failure, restore critical systems first (such as payroll or sales) and then less critical systems.

---

## 4. Responsibilities

| Entity | Responsibility |
| ------------------------- | ----------------------------------------------------------------------- |
| **Cybersecurity Officer:** | Ensure backups are encrypted and cannot be read by anyone if stolen. |
| **Senior Management** | Approval to purchase sufficient storage space and advanced backup software. |
| **All Employees** | Employees are responsible for saving work files on the bank's server or cloud storage. |

---

## 6. Review

- This procedure is reviewed **annually** or immediately following any security incident related to human error.

- Any modification requires the approval of the Information Security Manager and documentation in the change log.

---

_Al Noor Bank for Finance and Investment — Confidential Internal Document_ _Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)_
