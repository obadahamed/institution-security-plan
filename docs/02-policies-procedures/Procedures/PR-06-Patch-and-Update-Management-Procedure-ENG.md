Patch and Update Management Procedure

|||
|---|---|
|**Procdure Number**|PR-06|
|**Related Policy**|P-06— Patch and Update Management Policy|
|**Version**|1.0|
|**Release Date**|02/05/2026|
|**Next Review Date**|02/05/2027|
|**Procedure Owner**|Information Security Manager|
|**Classification**|Internal|

---

## 1. Objective

To ensure that all electronic devices receive the latest and correct updates as soon as possible to patch existing vulnerabilities and achieve better security.

---

## 2. Scope

This procedure applies to all devices and technical assets of the bank, including:

- Operating Systems (Windows, Linux, macOS).

- Applications, Office Software, and Middleware.

- Network devices (routers, switches, firewalls).

- Database management systems and cloud platforms.

---

## 3. Detailed Steps

### Step 1 — Inventory & Discovery

- **Asset Inventory:** Create a comprehensive list of all devices (computers, servers), software, and operating systems on the network.

- **Check for Updates:** Monitor manufacturer alerts (e.g., Microsoft, Adobe, Cisco) or use vulnerability scanners to identify updates.

### Step 2 — Categorization

- **Risk Classification:** Based on security alerts, the update is categorized as:

- **Critical:** A vulnerability that is currently being exploited (requiring an immediate update within 24-48 hours).

- **Important:** A security vulnerability, but no active exploitation (within 7-14 days).

- **Routine:** Performance improvements or new features (involved in routine maintenance).

### Step 3 — Testing Phase

- **Staging Environment:** First, apply the update to a small group of non-critical machines or in an isolated (lab) environment.

- **Compatibility Check:** Ensure that the update does not cause disruptions to essential business applications or conflicts with security software.

### Step 4 — Pre-Deployment Backup

- **Restore Point:** Before updating servers or sensitive systems, ensure that a recent backup (snapshot) exists to restore to in case the update fails.

### Step 5 — Deployment

- **Automation:** Use centralized tools (such as WSUS for Windows or ManageEngine) to distribute updates to all devices simultaneously.

- **Execution Time:** Schedule updates outside of regular business hours to minimize the impact on productivity, especially if the update requires a device restart.

### Step 6 — Verification

- **Success Report:** Generate a report from the management system to confirm that all devices have successfully received the update.

- **Post-Scan:** Perform a new vulnerability scan to ensure that the vulnerability has been patched.

### Step 7 — Documentation

- Record the update KB number, installation date, updated devices, and any issues encountered during the process for future reference.

---

## 4. Responsibilities

| Entity | Responsibility |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| **Information Security Team** | **:** Monitor global security bulletins (such as CVEs) and alert the technical team to new vulnerabilities as soon as they are discovered. |
| **Systems Administration Team** | Responsible for testing updates in an isolated environment to ensure they do not cause system crashes. |
| **All Employees** | Responsible for restarting the device when the system requests it to complete the installation, and not delaying updates beyond the allowed time (e.g., 24 hours). |

---

## 5. Required Documents and Records

| Document | Responsible Party for Storage |
| ----------------------------- | ----------------------- |
| Asset Inventory Record | Information Security Manager |
| Vulnerability Assessment Report After Update | Information Security Manager |

---

## 6. Review

- This procedure is reviewed **annually** or immediately after any security incident related to human error.

Any modification requires the approval of the Information Security Manager and must be documented in the changelog.

---

Al-Noor Bank for Finance and Investment — Confidential Internal Document
- ...
