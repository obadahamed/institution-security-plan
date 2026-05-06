Network and Communications Security Procedure

|||

|---|---|

|**Procedure Number**|PR-13|
|**Attached Policy**|P-13— Network and Communications Security Policy|
|**Version**|1.0|
|**Release Date**|02/05/2026|
|**Next Revision Date**|02/05/2027|
|**Procedure Owner**|Information Security Manager|
|**Classification**|Internal|

---

## 1. Purpose

To protect the network infrastructure (wired and wireless) and ensure the confidentiality of data in transmission, and to prevent unauthorized access to internal network resources.

---

## 2. Scope

All network components of the organization, including:

- Network devices (routers, switches, firewalls).

- Wireless networks (Wi-Fi).

- Third-party communications and remote access (VPN).

- Internet access points.
---

## 3. Detailed Steps

### Step 1 — Implement Network Segmentation:

- Divide the network into VLANs to isolate administrative traffic from employee traffic, and completely isolate the guest Wi-Fi network.

- Place sensitive systems (such as servers) in a protected area behind a DMZ.

### Step 2 — Implement Firewall Management:

- Implement a "Deny All" rule and allow only essential services (such as email or secure browsing).

- Review firewall rules every 6 months to delete outdated or unused rules.

### Step 3 — Implement Wi-Fi Security:

- Use strong encryption protocols (such as WPA3 or WPA2-Enterprise) and disable older protocols (such as WEP).

- Hide the network name (SSID) of sensitive systems and change Wi-Fi passwords regularly.

### Step 4 — Implementing Encryption in Transit (EFT):

- Mandatory use of encrypted protocols for all operations (e.g., HTTPS for websites, SSH for administration, and TLS for email).

### Step 5 — Implementing Intrusion Detection and Prevention (IDS/IPS):

- Activate live monitoring systems that analyze data packets, detect suspicious patterns (e.g., hacking attempts), and automatically block them.

---

## 4. Responsibilities

| Entity | Responsibility |
| ------------------------- | ----------------------------------------------------------------------------------------------------- |
| **Employees** | Connecting personal routers or unauthorized access points to the internal network is strictly prohibited. |
| **Cybersecurity Team:** | Review network logs to identify vulnerabilities and conduct regular penetration testing. |
| **Network Engineer** | Responsible for technical settings, hardware firmware updates, and ensuring stable connectivity |

---

## 5. Required Documents and Records

| Document | Responsible Party |
| --------------------------------------- | ----------------------- |
| Network Diagram | Network Engineer |
| Network Hardware Inventory Log | IT Team |
| Firewall Change Log | Network/Security Administrator |

---

## 6. Review

- This procedure is to be reviewed **annually** or immediately following any security incident related to human error.

- Any modification requires the approval of the Information Security Manager and documentation in the change log.

---

_Al Noor Bank for Finance and Investment — Confidential Internal Document_ _Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)_
