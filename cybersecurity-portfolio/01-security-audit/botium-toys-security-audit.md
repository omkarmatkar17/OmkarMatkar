# Botium Toys: Internal Security Audit

## Scope and Goals of the Audit

**Scope:** The scope of this audit covers Botium Toys' entire security program. This includes all employee equipment and devices, the internal network, and internal systems, processes, and data across the organisation.

**Goals:** The goal is to assess existing assets and complete the controls and compliance checklist to determine which controls and compliance best practices need to be implemented to improve Botium Toys' overall security posture.

## Current Assets

Assets managed by the IT department include:

- On-premises equipment supporting in-office business needs
- Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables, keyboards, mice, docking stations, surveillance cameras, etc.
- Storefront products available for retail sale on site and online, stored in the company's adjoining warehouse
- Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management
- Internet access and internal network
- Data retention and storage
- Legacy system maintenance: end-of-life systems that require human monitoring

## Risk Assessment Summary

Botium Toys currently lacks adequate asset management practices. Effective controls are not fully in place, and the company does not meet the compliance requirements of U.S. and international regulations. Existing assets are not appropriately classified, and customer credit card and PII/SPII data is not encrypted. Access controls are missing, and all 50 employees currently have access to internally stored data, including cardholder data and customer PII/SPII. The risk score is 8 out of 10 (high), driven primarily by inadequate asset management and the absence of controls needed to protect assets and meet compliance obligations. The likelihood of a breach involving company or customer data is high, and fines from regulatory bodies are a realistic possibility given current gaps against GDPR and PCI DSS.

## Controls Assessment Checklist

| Control | Yes / No | Explanation |
|---|---|---|
| Least privilege | No | All 50 employees currently have access to customer data, including PII and cardholder data. Access needs to be restricted based on job role to reduce the risk of a breach. |
| Disaster recovery plans | No | No disaster recovery plan exists. One is needed to ensure business continuity in the event of an incident. |
| Password policies | No | A nominal password policy exists, but the requirements are minimal and do not meet current best practice standards, putting identity and access management at risk. |
| Separation of duties | No | The CEO currently manages daily operations and runs payroll. These responsibilities should be split to reduce the risk of fraud and abuse of privilege. |
| Firewall | Yes | A firewall is in place and blocks traffic based on appropriately defined security rules. |
| Intrusion detection system (IDS) | No | No IDS is installed. The IT department needs one to identify possible intrusions by threat actors. |
| Backups | No | Critical data is not backed up. Backups are essential to restore operations and maintain continuity after an incident. |
| Antivirus software | Yes | Antivirus software is installed and monitored regularly by the IT team. |
| Manual monitoring, maintenance, and intervention for legacy systems | No | Legacy systems are monitored and maintained, but there is no regular schedule for intervention, and procedures for handling issues are unclear. |
| Encryption | No | Data at rest and in transit is not encrypted. Encryption is required to protect the confidentiality of sensitive customer data, including credit card information. |
| Password management system | No | No password management system is in place. Implementing one would improve IT and security team productivity when handling resets and access issues. |
| Locks (offices, storefront, warehouse) | Yes | Physical locks protect the office, storefront, and warehouse. |
| Closed-circuit television (CCTV) surveillance | Yes | CCTV is installed and operational at the premises. |
| Fire detection/prevention (fire alarm, sprinkler system, etc.) | Yes | Fire detection and prevention systems are functional at the physical location. |

## Compliance Checklist

### Payment Card Industry Data Security Standard (PCI DSS)

| Best practice | Yes / No | Explanation |
|---|---|---|
| Only authorized users have access to customers' credit card information | No | All employees currently have access to internally stored data, including cardholder information. |
| Credit card information is accepted, processed, transmitted, and stored internally, in a secure environment | No | Credit card data is not encrypted, and access is not restricted to authorised users, so the environment is not secure. |
| Implement data encryption procedures to better secure credit card transaction touchpoints and data | No | No encryption is currently in place for cardholder data. |
| Adopt secure password management policies | No | Password policies are minimal and no password management system exists. |

### General Data Protection Regulation (GDPR)

| Best practice | Yes / No | Explanation |
|---|---|---|
| E.U. customers' data is kept private/secured | No | Data at rest and in transit is not encrypted, so E.U. customer data is not adequately protected. |
| There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/breached | Yes | A breach notification plan exists to inform E.U. customers within 72 hours of a breach. |
| Ensure data is properly classified and inventoried | No | Current assets have been inventoried, but data is not properly classified. |
| Enforce privacy policies, procedures, and processes to properly document and maintain data | Yes | Privacy policies, procedures, and processes have been developed and are enforced among the IT team and other employees where applicable. |

### System and Organization Controls (SOC type 1, SOC type 2)

| Best practice | Yes / No | Explanation |
|---|---|---|
| User access policies are established | No | Least privilege and separation of duties are not implemented; all employees can access internal data. Access policies based on role need to be established. |
| Sensitive data (PII/SPII) is confidential/private | No | Sensitive data is not encrypted and access is not restricted, so confidentiality is not assured. |
| Data integrity ensures the data is consistent, complete, accurate, and has been validated | Yes | Data integrity is currently maintained. |
| Data is available to individuals authorized to access it | No | While data is available, it is accessible to all employees rather than only those authorised to use it. Access needs to be limited appropriately. |

## Recommendations to Stakeholders

To reduce the current risk score of 8 and address compliance gaps, the IT manager recommends implementing the following controls as a priority. First, enforce least privilege and separation of duties so that access to sensitive data, including customer PII/SPII and cardholder information, is limited to employees who require it for their role. Second, implement encryption for data at rest and in transit to protect the confidentiality of customer data and move toward PCI DSS and GDPR compliance. Third, deploy an intrusion detection system to help the IT team identify potential intrusions in a timely manner. Fourth, establish disaster recovery plans and regular backups of critical data to safeguard business continuity. Fifth, strengthen the password policy to align with current NIST-recommended complexity standards and implement a centralised password management system to reduce operational overhead. Finally, properly classify all data assets and define a regular schedule and clear procedures for legacy system maintenance and intervention. Implementing these controls will significantly lower the likelihood and impact of a breach, reduce exposure to regulatory fines, and improve Botium Toys' overall security posture as the business continues to grow its online presence.
