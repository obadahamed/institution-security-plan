# Audit and Log Review Policy

| | |
| -------------------------- | ------------------ |
| **Policy Number** | P-15 |
| **Version** | 1.0 |
| **Release Date** | 02/05/2026 |
| **Next Review Date** | 02/05/2027 |
| **Policy Owner** | Information Security Manager |
| **Classification** | Internal |

---

## 1. Purpose

The purpose of this policy is to ensure that all significant activities and events are logged on the organization's systems, providing accurate and comprehensive logs that enable monitoring of usage, detection of suspicious activity, and facilitating digital forensics investigations when necessary.

---

## 2. Scope

This policy covers all technical systems, including:

- Operating Systems (Servers & Workstations).

- Business Applications and Databases.

- Network Devices (Firewalls, Routers).

- Access Control Systems and Cloud Services

---

## 3. Policy Provisions

### - **Activities to be Logged:** Successful and unsuccessful login attempts, permission changes, access to sensitive data, system modifications, and log deletions must be logged.

### - **Log Details:** Each log must include the date and time, user ID, activity type, IP address, and outcome (success/failure).

### - **Log Protection:** Audit logs must be encrypted, preventing any user (including system administrators) from modifying or deleting them.

### - **NTP Time Synchronization:** All devices must be synchronized with a unified time source to ensure the accuracy of the incident timeline.

### - **Retention Period:** Active logs must be retained for a minimum of 90 days, and historical logs must be archived for at least one year (or as required by law).

---

## 4. Responsibilities

| Entity | Responsibility |
| -------------------- | --------------------------------------------------------------------------------------------------- |
System Administrators | Responsible for enabling logging features on all devices and applications. |
Cybersecurity Team | Responsible for the periodic review of logs, analysis of security alerts, and use SIEM systems to automate monitoring. |
Auditors | Conduct independent audits to ensure policy compliance and that logs are not being tampered with. |

--

## 5. Penalties

- Disabling, attempting to modify, or deleting logging features is a serious security violation that may result in termination of service.

- Negligence in reviewing logs that results in the failure to detect an ongoing security breach subjects the responsible party to administrative accountability.

--

## 6. Review

This policy is reviewed annually to ensure its comprehensiveness across all new systems and compliance with evolving legal standards.

---

*Al Noor Bank for Finance and Investment — Confidential Internal Document*

*Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)*
