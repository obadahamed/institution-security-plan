Audit and Log Review Procedure

|||
|---|---|
|**Procedure Number**|PR-15|
|**Related Policy**|P-15—Audit and Log Review Policy|
|**Version**|1.0|
|**Release Date**|02/05/2026|
|**Next Review Date**|02/05/2027|
|**Procedure Owner**|Information Security Manager|
|**Classification**|Internal|

---

## 1. Objective

To ensure that all significant activities and events are logged on the organization's systems, providing accurate and comprehensive logs that enable monitoring of usage, detection of suspicious activity, and facilitating digital forensics investigations when necessary.

---

## 2. Scope

This policy covers all technical systems, including:

- Operating Systems (Servers & Workstations).

- Business Applications and Databases.

- Network Devices (Firewalls, Routers). - Access Control Systems and Cloud Services

---

## 3. Detailed Steps

### Step 1 — **Logging Configuration:**

- Enable logging at all system levels (applications, databases, servers, network devices).

- Configure systems to log only critical events to avoid filling up storage space (e.g., login, permission changes, access to sensitive data).

### Step 2 — **Log Protection:**

- Immediately send logs to a centralized log server to ensure they cannot be deleted by an attacker who gains control of the original machine.

- Encrypt the logs and prevent anyone (including the system administrator) from modifying or deleting them (WORM - Write Once Read Many).

### Step 3 — **Monitoring & Review:**

- Daily review of "critical" logs using automated alert systems.

- Random weekly or monthly review of regular logs to ensure there are no suspicious patterns.

### Step 4 — **Time Synchronization Implementation:**

- Mandatory connection of all devices to a unified timing source (NTP Server) to ensure that event times match when investigating a specific incident.

### Step 5 — **Archiving and Destruction Implementation:**

- Retain active (online) logs for 90 days, archive old (offline) logs for one year or more as required by law, and then destroy them securely.

---

## 4. Responsibilities

| Entity | Responsibility |
| ------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| **Systems and Network Administrators:** | Technical responsibility for enabling logging, ensuring storage availability, and time synchronization. |
| **Cybersecurity Team (SOC Analyst):** | Analyze logs using SIEM systems, investigate security alerts, and write audit reports. |
| **Application Owners:** | Ensure their applications support the logging feature and provide sufficient information for auditing (such as user ID and activity). |

---

## 5. Required Documents and Records

| Document | Responsible Party |
| ------------------------------ | ---------------------------- |
| **System Logs** | IT Department |
| **Periodic Audit Reports** | Cybersecurity Team |
| **Log Server Access Log** | Security Admin |

---

## 6. Review

- This procedure is reviewed **annually** or immediately following any security incident related to human error.

- Any modification requires the approval of the Information Security Manager and documentation in the change log.

---

_Al Noor Bank for Finance and Investment — Confidential Internal Document_ _Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)_
