# Password Policy

|||
|---|---|
|**Procedure Number**|PR-03|
|**Related Policy**|P-03 — Password Policy|
|**Version**|1.0|
|**Release Date**|02/05/2026|
|**Next Review Date**|02/05/2027|
|**Procedure Owner**|Information Security Manager|
|**Classification**|Internal|

---

## 1. Objective

To ensure strong and difficult-to-guess passwords.

---

## 2. Scope

This procedure applies to the Information Security Manager and all employees with access to the bank's network.

---

## 3. Detailed Steps

### Step 1 — Strength Criteria Settings

- **Minimum Length:** 12 to 14 characters.


- **Variety:** Must contain uppercase letters, lowercase letters, numbers, and special characters such as @, #, and $.

- **Smart Blocking:** Prevent the use of common words (such as Admin123) or personal information (employee name or date of birth).

### Step 2 — Password Change Procedures and Expiration Period

- **Recurring Change:** Require employees to change their passwords every 90 days for standard systems and every 60 days for sensitive systems.

- **Prevent Duplication:** Maintain a "password history" to prevent employees from reusing their last 5 to 10 passwords.

- **Mandatory First Change:** Upon creating a new account, employees must change their temporary password immediately upon logging in for the first time.

### Step 3 — Account Lockout Procedures

To protect the account from brute-force attacks:

- **Number of Attempts:** Automatically lock the account after 5 failed login attempts.

- **Lockdown Duration:** The account will remain locked for 30 minutes before another attempt is allowed, or until the employee contacts technical support.

### Step 4 — Reset Procedures

- **Identity Verification:** Before providing a new password, the technical support staff member must verify the employee's identity (via a security question or video call).

- **Self-Service Reset Procedure (SSPR):** Provide a portal that allows employees to reset their own passwords via a backup email or a code sent to their phone, to reduce the burden on technical support.

### Step 5 — Storage and Security Procedures

- **Encryption:** Passwords must be stored in the database using strong encryption algorithms (hashing) such as Argon2 or bcrypt.

- **No Writing:** Employees are prohibited from writing passwords on pieces of paper and sticking them on screens or desks (this is checked periodically as part of physical security audits).

Step 6 — Awareness of Supporting Tools

- **Password Manager:** Encourage or require employees to use tools such as LastPass or Bitwarden to store complex passwords instead of memorizing them in a browser or on paper.

---

4. Responsibilities

| Entity | Responsibility |
| ------------------------- | ----------------------------------------------------------- |
| **Information Security Manager** | Oversee all steps, review reports, and approve reports |
| **Line Supervisors** | Ensure their team performs the correct tasks |
| **All Employees** | Follow guidelines and regulations and maintain password confidentiality |
| **Cybersecurity Team** | Monitor login logs |

---

5. Required Documents and Records

| Document | Responsible Entity for Storage |
| -------------------------- | ----------------------- |
| Record Monitoring and Evaluation Report | Information Security Manager |
| Red Team Annual Report | Information Security Manager |

---

## 6. Review

- This procedure is reviewed **annually** or immediately following any security incident related to human error.

- Any modification requires the approval of the Information Security Manager and must be documented in the change log.

---

_Al Noor Bank for Finance and Investment — Confidential Internal Document_ _Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)_
