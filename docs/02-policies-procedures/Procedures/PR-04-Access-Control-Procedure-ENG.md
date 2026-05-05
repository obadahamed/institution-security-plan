Access Control Procedure

|||
|---|---|
|**Procedure Number**|PR-04|
|**Associated Policy**|P-04—Access Control Policy|
|**Version**|1.0|
|**Release Date**|02/05/2026|
|**Next Revision Date**|02/05/2027|
|**Procedure Owner**|Information Security Manager|
|**Classification**|Internal|

---

## 1. Objective

To control how and when public and private data is accessed, and by whom, ensuring that everyone accessing the system is the correct person.

---

## 2. Scope

This procedure applies to the Information Security Manager and all employees with access to the bank's network.

---

## 3. Detailed Steps

### Step 1 — Provisioning Procedures

- **Provisioning:** Determine the number of employees and categorize them according to their roles within the bank.

- **Reference Job Assignment (RBAC):** Link permissions to job roles (e.g., an accountant automatically receives access to the financial system, while an engineer does not).

- **Background Check:** Ensure that the employee has completed the HR procedures (signed a confidentiality agreement) before any account is opened for them.

- **Request Form:** Access is granted only upon a formal request approved by the direct manager and the data owner. ### Step 2 — Periodic Access Review Procedures

- **Quarterly Audits:** Review the user list every 3 months to ensure that granted permissions still align with their current responsibilities.

- **Permission Corrections:** Immediately revoke any excess permissions (e.g., an employee transferred from sales to purchasing should have their sales permissions revoked).

### Step 3 — Deprovisioning Procedures

- **Immediate Termination:** Upon an employee's resignation or termination, all their accounts (email, VPN, systems) should be closed immediately and automatically, if possible.

- **Asset Recovery:** Do not release an employee until they have returned their physical access keys and any devices in their possession.

### Step 4 — Privilegeed Access Procedures

- **Administrator Accounts:** Use separate accounts for administrative tasks (one for daily use and one for higher-level privileges).

- **The "Two" Principle:** For highly sensitive operations (such as deleting a database), the procedure may require the approval of two technical personnel to execute the order.

### Step 5 — Physical Access Procedures

- **Security Gates:** Use magnetic cards that record the time an employee enters and exits sensitive rooms (such as server rooms).

- **Escorts:** Require visitors or external contractors to be accompanied by a member of the organization's staff at all times while in restricted areas.

### Step 6 — Documentation and Monitoring Procedures

- **Access Log:** Record every entry and exit, and record changes to permissions (who granted permissions to whom? and when?).

- **Failure Alerts:** Enable immediate alerts when unauthorized individuals attempt to access "Top Secret" files.

---

## 4. Responsibilities

| Entity | Responsibility |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| **Information Security Department** | - Policy Writing: Drafting rules and technical requirements.|
| **IT Department** | Creating accounts for new employees and closing accounts for those who have resigned. |
| **All Employees** | Principal responsible for compliance |

---

## 5. Required Documents and Records

| Document | Responsible Party for Filing |
| ---------------------------------- | ----------------------- |
| Records Follow-up Evaluation Report | Information Security Manager |
| Annual Red Team Report | Information Security Manager |
| Number of Accounts and Settings for Each Account | **Information Technology Department** |

---

## 6. Review

- This procedure is reviewed **annually** or immediately following any security incident related to human error.

- Any modification requires the approval of the Information Security Manager and documentation in the Change Log.


---

_Al Noor Bank for Finance and Investment — Confidential Internal Document_ _Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)_
