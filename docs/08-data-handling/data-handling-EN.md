# **Data Handling**

---
## 1. Objective

To collect, store, and analyze customer and transaction data to extract strategic insights, while ensuring its complete confidentiality and protection in accordance with global security standards.

---

## 2. Scope

This includes all types of data owned or handled by the bank, regardless of its format:

- **Digital Data:** Data stored on servers, in cloud accounts, and in databases.

- **Physical Data:** Paper documents, signed contracts, and archived files in the bank's repositories.

- **Audio and Video Data:** Recordings from surveillance cameras in branches and recordings of telephone calls with customer service.

---

## 3. Data Classification

1. Highly Confidential Data

- **Concept:** Highly sensitive information whose leakage would cause financial and legal disasters and completely destroy the bank's reputation.

- **Examples:**

- Passwords, security codes (PINs), and one-time passwords (OTPs).

- Encryption keys for the bank's systems.

- Customer biometric data (fingerprints and facial recognition).

2. Confidential/Restricted Data

- **Concept:** Data related to customers or internal bank operations, accessible only to authorized personnel for their specific job duties.

- **Examples:**

- Customer personal information (full name, ID number, address, and phone number).

- Financial transactions, account records, and credit card records.

- Payroll and internal employee records.

3. Internal Data (Internal Use Only)

- **Concept:** Information not intended for public consumption, circulated only among bank employees for daily operations. While its disclosure does not pose a destructive risk, it does violate organizational privacy.

- **Examples:**

- The internal organizational structure, detailed policies, and procedures. - Internal emails and interdepartmental memos.

4. Public Data

- **Concept:** Information available to everyone, the dissemination of which poses no risk to the bank or the customer. The bank aims to publish it for marketing and transparency purposes.

- **Examples:**

- Current interest rates and published exchange rates.

- Branch and ATM locations.

---
## 4. Data Lifecycle

1. Creation/Collection

- **What Happens:** Data enters the bank for the first time.

- **Examples:** A customer filling out an account opening form, recording an ATM withdrawal, or taking an ID photo.

2. Storage

- **What Happens:** Data is stored in a secure digital or physical environment immediately after collection.

- **Examples:** Data is encrypted and stored in the bank's central databases or the cloud, with immediate backups implemented to prevent data loss.

3. Usage/Processing

- **What happens:** Data is read, modified, or used to complete daily banking transactions.

- **Examples:** Updating account balances after a transfer, or using artificial intelligence systems to examine transactions and ensure there is no fraud.

4. Sharing/Distribution

- **What happens:** Data is sent to authorized parties, both inside and outside the bank, while adhering to confidentiality requirements.

- **Examples:** Sending account statements to the customer's email, sharing credit data with payment networks such as Visa/MasterCard, or providing reports to the central bank.

5. Archiving

- **What happens:** Data that is no longer active or used daily is transferred to a long-term storage environment, due to the bank's legal obligation to retain records for several years (often 5 to 10 years). - **Examples:** Moving old, closed customer account records to slower, separate archiving servers to reduce costs and protect them.

6. Destruction/Disposal

- **What Happens:** The final and secure disposal of data after the legal archiving period has expired, ensuring it can never be recovered.

- **Examples:** Shredding and destroying paper documents, or using digital degaussing software to destroy data from old hard drives.

---
## 5. Security Controls for Each Level

1. Highly Confidential Data Controls

This level requires the highest levels of technical and physical security and is subject to strict controls:

- **Comprehensive and End-to-End Encryption:** Encrypting data in transit and at rest using the strongest encryption algorithms (such as AES-256).

- **Strict Multi-Factor Authentication (MFA):** This data can only be accessed by enabling three levels of verification (password, temporary code, and biometric fingerprint).

- **Need-to-Know Principle:** Access is granted to a very limited number of people (such as the CISO or Chief Security Officer) for limited and monitored periods.

- **Air-Gapping:** Servers containing encryption keys or biometric data are isolated on internal networks completely separate from the internet to prevent remote access.

- **Real-time Auditing:** Every second of every login or modification to this data is recorded, with an immediate alert issued to cybersecurity departments upon any unauthorized access attempt.

2. Confidential/Restricted Data Controls

This data is protected to ensure customer privacy and secure financial transactions:

- **Role-Based Access Control (RBAC):** Employees are granted access to only the data they need to perform their duties (e.g., a cashier sees only the balance, not the full credit card number).

- **Data Masking:** Concealing portions of sensitive data when displayed on employee screens (e.g., showing only the last four digits of a card).
The credit note is formatted as follows: `**** **** **** 1234`).

- **Data Leakage Prevention (DLP):** Implementing systems that prevent employees from copying this data to a USB flash drive, sending it to an external email address, or printing it without prior authorization.

- **Standard Encryption:** Encrypting customer databases and account transactions permanently.

3. Internal Data Controls (Internal Use Only)

The goal here is to prevent the dissemination of the bank's confidential documents to the public:

- **Standard Authentication:** Access to data requires the employee's standard login via the bank's internal network or via a secure virtual private network (VPN) if working remotely.

- **Digital Watermarking:** Placing a watermark with the employee's name and the date they accessed the documents and internal policies makes it easy to trace the source of a leak if they are published outside the bank.

- **Non-Disclosure Agreements (NDAs):** Employees and contractors sign legally binding agreements that prevent them from sharing the bank's internal processes with any external party.

4. Public Data Controls

This data requires a different type of protection. The goal is not to hide it, but to **protect its integrity and prevent its corruption**:

- **Integrity Protection and Verification:** Ensuring that the prices displayed (such as exchange rates and interest rates) on the bank's website or branch screens have not been altered or falsified through cyberattacks.

- **Website and Application Firewalls (WAFs):** Protecting the bank's public web servers from downtime due to DDoS attacks.

- **Strict Change Management:** No public information (such as updating a branch website or adding a promotional offer) is modified without a formal approval process from the Compliance and Marketing Department.


## 6. Responsibilities

1. Board of Directors and Senior Management

- **Responsibility:** Strategic governance and oversight.

- **Tasks:**

- Approving the general policy for handling and classifying data.

- Providing the necessary budgets for purchasing security systems and training staff. - Bears ultimate legal responsibility to the central bank in the event of a large-scale data leak.

2. Data Owner

- **Who is this:** Typically the head of the department that generates the data (e.g., Retail Banking Manager, Human Resources Manager).

- **Responsibilities:**

- Determining the sensitivity level and classification of the data within their department.

- Determining who has access to this data (granting and revoking permissions).

- Reviewing access permissions periodically to ensure there is no over-reliance on permissions.

3. Data Custodian/IT Department

- **Who is this:** The IT department and database administrators.

- **Responsibilities:**

- Technical implementation of the Data Owner's decisions.

- Responsible for data storage, backups, and ensuring system integrity.

- Implementing encryption techniques, data masking, and archiving or destroying data according to established policy.

4. Information/Cyber ​​Security Team

- **Who is it:** Led by the Chief Information Security Officer (CISO).

- **Responsibilities:**

- Establishing technical protection standards and controls for each classification level.

- Monitoring systems around the clock to detect hacking attempts or real-time data leaks.

- Managing Data Leakage Prevention (DLP) programs and verifying the implementation of Multi-Factor Authentication (MFA).

5. Compliance & Risk Management

- **Responsibility:** Legal and regulatory oversight.

- **Responsibilities:**

- Ensuring that data handling mechanisms are fully compliant with central bank regulations and international legislation (such as GDPR).

- Assessing risks arising from dealings with third parties and reviewing their security contracts.

6. Data User

- **Who is it:** Any bank employee authorized to access data to perform their duties (such as a customer service representative or teller). - **Responsibilities:**

- Strict adherence to confidentiality policies and non-sharing of personal accounts or passwords.

- Immediate reporting to the Cybersecurity Department in case of suspected breaches, leaks, or phishing emails.

---

## 7. Review

1. Periodic Access Review

- **Objective:** To ensure that employees only have the access they currently need (minimum access principle).

2. Independent Internal Data Audit

- **Objective:** To examine the efficiency of systems and departments' compliance with the bank's internal policies (third line of defense).

3. External Audit & Compliance

- **Objective:** To obtain international security certifications and demonstrate compliance with regulatory authorities.

---

_Al Noor Bank for Finance and Investment — Confidential Internal Document_ _Prepared by: XENOS | [github.com/obadahamed](https://github.com/obadahamed)_
