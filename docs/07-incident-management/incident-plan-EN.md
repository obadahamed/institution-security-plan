# Incident Response Plan

| Document Information | Details |
| :--- | :--- |
| **Institution** | Al Noor Bank |
| **Document Number** | IR-PLAN-V1.0 |
| **Standard** | NIST SP 800-61 Rev. 2 |
| **Document ztatus** | Approved |

---

## 1. Purpose
This document aims to establish a formal and structured framework to enable Al Noor Bank to rapidly detect, contain, and recover from cybersecurity incidents with minimal impact. The plan seeks to protect the bank's financial assets, secure customer data, and ensure the continuity of critical banking services in accordance with banking laws and regulations.


---

## 2. Scope
This plan applies to all cybersecurity incidents targeting Al Noor Bank's infrastructure, including, without exception:

* All banking systems, networks, and applications (mobile app, website, Core Banking).

* Devices, data, and digital documents owned by the bank.

* All employees, consultants, contractors, and third parties with access to the bank's network.

---

## 3. Incident Classification
At Al Noor Bank, incidents are classified based on the **Impact** and **Urgency** matrix into four main levels to determine response speed and resource allocation:

| Level | Severity | Response Time |
| --- | --- | --- |
| P1 | Critical | 15 minutes |
| P2 | High | 30 minutes |
| P3 | Medium | 2 hours |
| P4 | Low | 12 hours |

### 3.1 Critical Incidents (P1)

* **Description:** A widespread breach that cripples critical services or threatens the bank's financial solvency and legal reputation.

* **Examples:** A ransomware attack that encrypts branch systems, leaks the bank's customer database, or compromises the SWIFT network.

* **Target Response Time (SLA):** Within 15 minutes.

### 3.2 High Incidents (P2)

* **Description:** A breach affecting a broad sector or critical services, with a high risk of threat escalation.

* **Examples:** A distributed denial-of-service (DDoS) attack that disables the mobile banking application or detects administrator privileges created without authorization.

* **Target Response Time (SLA):** Within 30 minutes.

### 3.3 Medium-Severity Incidents (P3)

* **Description:** An incident with a limited impact, confined to a narrow scope, that does not directly affect customer financial transactions.

* **Examples:** A single employee's email account was compromised, or a non-sensitive computer was infected with a partially quarantined virus.

* **Target Response Time (SLA):** Within 2 hours.

### 3.4 Low-Severity Incidents (P4)

* **Description:** Suspicious activity or an isolated security event that does not pose a real, immediate threat to the bank's systems.

* **Examples:** An attempt to randomly scan ports from outside the organization, or an employee mistakenly sending a non-sensitive file to someone inside the organization.

* **Target Response Time (SLA):** Within 12 hours.

---

## 4. The Six Phases of the NIST SP 800-61 Standard

### Phase 1: Preparation
Preparing the bank defensively **before** any incident occurs through:

* Regularly training the Crisis Response Team (CSIRT) and clearly assigning roles.

* Activating and securing centralized monitoring tools and logs.

* Maintaining encrypted and protected backups off-network.

### Phase 2: Detection and Analysis
This phase begins immediately upon detecting an indication of an attack:

* Monitoring alerts from the Security Operations Center (SOC) and SIEM systems.

* Analyzing the alert to verify and avoid false positives.

* Determining the extent of the breach and the type of threat (e.g., malware, phishing, data breach).

### Phase 3: Containment
Immediately prevent the spread of the attack and minimize damage:
* **Short-term containment:** Isolate infected devices or disconnect the affected subnet from the rest of the bank's systems.

* **Long-term containment:** Apply temporary security patches and close targeted ports while maintaining the functionality of other services.

* **Evidence collection:** Take snapshots of RAM and save logs for digital forensics.

### Phase 4: Eradication
Eradicating the threat after containment:

* Completely remove all malware and tools planted by the attacker.

* Delete compromised or illegally created accounts and change all passwords.

* Patch the security vulnerabilities exploited by the attacker in the systems.

### Phase 5: Recovery
Restore banking systems and services to normal operation:

* Restore affected data and systems from healthy and verified backups.

* Examine the restored systems to ensure they are free of any remaining vulnerabilities.

* Activate intensive monitoring of the systems that have returned to service to detect any rebound activity by the attacker.

### Phase 6: Lessons Learned
Developing the Defense System **Post-** Incident Closure:

* Hold a meeting to review the details of the incident: How did it happen? How was it addressed?

* Write the final incident report (Post-Incident Report).

* Modify this plan and update firewalls and security policies based on the identified gaps.

---

## 5. Responsibilities

The Security Incident Response Team (CSIRT) is responsible for the following tasks:

* **CIO:** Leading the incident, making strategic decisions (such as shutting down critical systems), and communicating with the bank's executive management.

* **IR Team Lead:** Managing field coordination among analysts and distributing technical tasks during the containment and recovery phases.
  
* **Cybersecurity Analysts (SOC/IR Analysts):** Detecting threats, analyzing digital evidence, and implementing technical steps to isolate and contain affected systems.

* **Legal and Public Relations Team:** Managing legal drafting and communicating with regulatory bodies (such as the central bank), and handling public statements in the event of a data breach to protect the bank's reputation.

* **IT/Network Team:** Assisting the security team in isolating networks, changing settings, and restoring systems from backups.

---

## 6. Review
This document undergoes regular periodic review to ensure its effectiveness:

* **Review Periodicity:** The document is reviewed and updated annually (every 12 months).

* **Emergency Review:** The plan is updated immediately in the event of a major change to the bank's infrastructure, or based on recommendations and lessons learned following a "critical" or "high" security incident.
  
---

-Al Noor Bank for Finance and Investment — Confidential Internal Document — Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)
