# Al Noor Bank Network Documentation and Security

| | |
| --- | --- |
| **Document Number** | NET-01 |
| **Version** | 1.0 |
| **Release Date** | 05/13/2026 |
| **Document Owner** | IT Manager |
| **Classification** | Internal Confidential |

---

## 1. Overview

This document describes the infrastructure of Al Noor Bank for Finance and Investment's network, including the logical network design, Virtual Network Interfaces (VLANs), and security mechanisms implemented according to ISO 27001.

The network consists of three locations:

- **Head Office** in As-Suwayda

- **Branch 1**

- **Branch 2**

Each branch is connected to the Head Office via an encrypted Site-to-Site VPN tunnel.

---

## 2. Logical Design

The network is based on three separate security zones:

| Zone | Description | Security Level |
| --- | --- | --- |
| **DMZ** | Hosts exposed internet services (Web Server, ATM GW) | Medium (50) |
| **Internal Network** | Internal staff network segmented by VLANs | High (100) |
| **Secure Zone** | Sensitive servers and databases | Very High |

---

## 3. Hardware Used

| Device | Model | Role |
| --- | --- | --- |
| Firewall | Cisco ASA 5506-X | Separates internet, DMZ, and internal network |
| Multilayer Switch (x2) | Cisco 3650-24PS | Routing between VLANs + Redundancy |
| Distribution Switch (x2) | Cisco 2960-24TT | Distributes VLANs to access switches |
| Access Switch (x7) | Cisco 2960-24TT | One per VLAN |
| Secure Zone Switch | Cisco 2960-24TT | Connects sensitive servers |
| DMZ Router | Cisco 2911 | Connects the Web Server and ATM GW to the ASA |

---

## 4. VLAN Table

| VLAN ID | Name | Network | Gateway | Secure Zone Access |
| --- | --- | --- | --- | --- |
| 10 | IT | 192.168.10.0/24 | 192.168.10.1 | ✅ Full |
| 20 | Security | 192.168.20.0/24 | 192.168.20.1 | ✅ Full |
| 30 | Finance | 192.168.30.0/24 | 192.168.30.1 | ✅ DB + HR only |
| 40 | HR| 192.168.40.0/24 | 192.168.40.1 | ✅ HR Server only |
| 50 | CustomerService | 192.168.50.0/24 | 192.168.50.1 | ✅ DB Server only |
| 60 | Management | 192.168.60.0/24 | 192.168.60.1 | ❌ Forbidden |
| 70 | Reception | 192.168.70.0/24 | 192.168.70.1 | ❌ Forbidden |
| 80 | Servers | 192.168.80.0/24 | 192.168.80.1 | — |
| 90 | DMZ | 192.168.90.0/24 | 192.168.90.1 | ❌ Prohibited |

---

## 5. Server Table

| Server | IP | VLAN | Description |
| --- | --- | --- | --- |
| DB-Server | 192.168.80.3 | 80 | Customer and Transaction Database |
| HR-Server | 192.168.80.2 | 80 | Employee Data |
| Security-Server | 192.168.80.4 | 80 | Security Records and Logs |
| Backup-Server | 192.168.80.5 | 80 | Backups |
| DHCP Server | 192.168.80.10 | 80 | Automatic IP Allocation |
Web Server | 192.168.92.10 | DMZ | Bank Website |
ATM GW | 192.168.91.10 | DMZ | ATM Gateway |

---

## 6. Implemented Services

### 6.1 DHCP
- Centralized DHCP server in the Secure Zone (192.168.80.10)
- DHCP requests are routed via `ip helper-address` on each SVI in MS1
- Each VLAN has a separate pool

### 6.2 OSPF - Dynamic Routing Protocol used between MS1 ​​and MS2
- Ensures automatic route conversion when any link fails
- MS1: Router-ID 1.1.1.1 | MS2: Router-ID 2.2.2.2

### 6.3 VTP
- MS1 is operating as a VTP Server
- All Distribution Switches are operating as VTP Clients
- Domain: BankNoor

### 6.4 SSH
- SSH v2 is enabled on all devices
- Telnet is disabled to prevent data transmission (clear text)

---

## 7. Access Policy (ACLs)

Extended ACLs have been implemented on the SVIs in MS1 ​​to control access between VLANs and the Secure Zone:

| VLAN | Policy |
| --- | --- |
| IT (10) | Full access to all servers |
| Security (20) | Full access to all servers |
| Finance (30) | Access to DB-Server and HR-Server only |
| HR (40) | Access to HR-Server only 
| CustomerService (50) | Access to DB-Server only |
| Management (60) | Completely blocked from the Secure Zone |
| Reception (70) | Completely blocked from the Secure Zone |

---

## 8. Firewall (ASA 5506-X)

| Interface | Name | IP | Security Level |
| --- | --- | --- | --- |
| Gig1/1 | inside | 10.0.0.1 | 100 |
| Gig1/2 | dmz | 192.168.90.1 | 50 |
| Gig1/3 | outside | 203.0.113.1 | 0 |


**Applicable Policies:**
- The DMZ is only allowed to receive HTTP/HTTPS from the internet.
- The DMZ is blocked from accessing the Secure Zone.
- The Internal Network is allowed to access the DMZ.

> Note: The ASA is fully configured with security levels and ACLs. Some ICMP tests are limited due to Packet Tracer emulator limitations on the ASA 5506-X model.

---

## 9. Branches

Each branch is connected to the main server via an encrypted **Site-to-Site VPN**. Each branch contains:
- A router managing the VPN tunnel.
- A switch for internal distribution.
- Employee devices.

The same VLAN and ACL policies apply to branches as to the main server.

---

## 10. Strengths and Proposed Improvements

**Strengths:**
- Network segmentation into clearly defined security zones
- Precise ACLs implementing the Least Privilege principle
- Centralized DHCP in the Secure Zone
- Redundancy across MS1 and MS2

**Proposed Future Improvements:**
- Adding a standalone IDS/IPS
- Implementing 802.1X device authentication before network connection
- Database encryption

---

*Al-Noor Bank for Finance and Investment — Confidential Internal Document*

*Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)*
