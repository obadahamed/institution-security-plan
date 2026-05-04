# Multi-Factor Authentication Procedure

|||
|---|---|
|**Procedure Number**|PR-02|
|**Associated Policy**|P-02 — Multi-Factor Authentication Policy|
|**Version**|1.0|
|**Release Date**|02/05/2026|
|**Next Revision Date**|02/05/2027|
|**Procedure Owner**|Information Security Manager|
|**Classification**|Internal|

---

## 1. Objective

To define the detailed practical steps for implementing and applying a multi-factor authentication system.


---

## 2. Scope

This procedure applies to the Information Security Manager and all employees with access to the bank's network.

---

## 3. Detailed Steps

### Step 1 — Planning and Preparation Phase

1. Identify all applications and services that require MFA (email, VPN, cloud, administrator dashboards).

2. Define the authorized authentication methods that will be used by the relevant parties.

3. **Target Groups**: Start with administrators and employees with high privileges (IT Admins) as a top priority.

### Step 2 — Technical Activation Procedures

1. **Initial Setup**: The IT department activates the MFA feature at the server-side level or with the Identity Provider.

2. **Grace Period**: Give employees a grace period (e.g., 3 days) to register their devices before access is blocked.

3. **Generating Emergency Codes:** Providing the user with one-time recovery codes.

### Step 3 — Registration Procedures

1. **User Guide:** Sending a step-by-step guide (images or video) explaining how to link the phone to the account.

2. **Technical Support:** Setting up a helpdesk to address issues.

### Step 4 — Administration and Daily Operation Procedures

1. **Device Change:** When an employee receives a new phone, a "Reset MFA" procedure is performed after personal identity verification.

2. **Revocation of Access:** If an employee resigns or their device is lost, the MFA sessions associated with their account are immediately revoked.

3. **Monitoring:** Reviewing login logs to detect repeated failed MFA attempts.

### Step 5 — Exception Handling Procedures

1. **Exception Request:** If an employee's device malfunctions, they are granted a temporary bypass for 24 hours only, subject to approval by their direct supervisor. Step 6 — Review and Audit

1. Compliance Check: Generate a monthly report showing the percentage of employees who successfully completed the MFA.


4. Responsibilities

| Entity | Responsibility |
| ------------------------- | ----------------------------------------------------------- |
| **Information Security Manager** | Oversee all steps, review reports, and approve reports |
| **Line Supervisors** | Ensure their team performs the correct tasks |
| **All Employees** | Follow guidelines and regulations and maintain confidentiality |
| **Cybersecurity Team** | Monitor login logs |

---

5. Required Documents and Records

| Document | Responsible Party for Records |
| -------------------------- | ----------------------- |
| Records Follow-up Assessment Report | Information Security Manager |
| Annual Red Team Report | Information Security Manager |

## 6. Review

- This procedure is reviewed **annually** or immediately following any security incident related to human error.

- Any modification requires the approval of the Information Security Manager and documentation in the change log.

--

_Al Noor Bank for Finance and Investment — Confidential Internal Document_ _Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)_
