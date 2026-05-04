# Network and Communications Security Policy

| | |
| -------------------------- | ------------------ |
| **Policy Number** | P-13 |
| **Version** | 1.0 |
| **Release Date** | 02/05/2026 |
| **Next Revision Date** | 02/05/2027 |
| **Policy Owner** | Information Security Manager |
| **Classification** | Internal |

---

## 1. Purpose

To provide a comprehensive security framework to protect the network infrastructure (wired and wireless), ensure data confidentiality during transmission, and prevent unauthorized access to internal network resources.

---

## 2. Scope

This policy covers all components of the organization's network, including:

- Network devices (routers, switches, firewalls).

- Wireless networks (Wi-Fi).

- Third-party communications and remote access (VPN).

- Internet Connection Points

---

## 3. Policy Provisions

### - **Network Segmentation:**
The network must be divided into secure, isolated zones (e.g., isolating the guest network from the management network, and the development environment from the production environment).

### - **Firewalls:**
Firewalls must be enabled at all internet connection points, with the "Deny by Default" rule applied, allowing only essential traffic.

### - **Wireless Network Security:**
The use of weak encryption protocols (e.g., WEP or WPA) is prohibited. WPA3 or WPA2 Enterprise must be used with strong authentication.

### - **Data Encryption in Transmission:**
All sensitive data exchanged over the network must be encrypted using secure protocols (e.g., TLS/SSL or SSH). ### - **Intrusion Detection and Prevention (IDS/IPS):**
Systems must be deployed to monitor network traffic and automatically detect and respond to suspicious activity or cyberattacks.

---

## 4. Responsibilities

| Entity | Responsibility |
| --------------- | ------------------------------------------------------------------------------------------------------------- |
| Network Engineers | Responsible for the technical management of devices, updating their firmware, and configuring security settings. |
| Cybersecurity | Responsible for monitoring network logs, conducting periodic penetration tests, and ensuring the effectiveness of firewall policies. |
| Users | Required to refrain from connecting any unauthorized devices (such as personal routers) to the internal network. |


---

## 5. Penalties

- Tampering with network settings, attempting to break encryption, or performing vulnerability scanning without authorization is a serious security violation. - Penalties range from a final warning to termination of service, with legal liability in case of network disruption or data leaks.

---

## 6. Review

Firewall rules are reviewed every six months, and the policy is updated annually to keep pace with developments in communication technologies and related threats.

---

*Al Noor Bank for Finance and Investment — Confidential Internal Document*

*Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)*
