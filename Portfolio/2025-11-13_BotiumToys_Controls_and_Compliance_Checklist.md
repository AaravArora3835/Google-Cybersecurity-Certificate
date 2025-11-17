# **Botium Toys — Internal Security Audit: Controls & Compliance Checklist**

This document contains a completed controls and compliance checklist for the fictional company **Botium Toys**, based on their scope, goals, and risk assessment report.
It follows NIST Cybersecurity Framework (CSF) categories: Identify, Protect, Detect, Respond, and Recover.

---

## **1. Identify Controls**

| Control                                | Meets Control? | Notes                                                                    |
| -------------------------------------- | -------------- | ------------------------------------------------------------------------ |
| Asset inventory maintained and updated | **No**         | Inventory is incomplete and lacks ongoing update procedures.             |
| Data classification performed          | **No**         | No documented classification for customer, payment, or EU-specific data. |
| Business environment defined           | **Yes**        | Roles and operational structure for IT exist and are described.          |
| Risk assessment conducted regularly    | **Yes**        | An initial risk assessment was completed.                                |
| Risk management strategy documented    | **No**         | No long-term, repeatable risk management plan exists.                    |

---

## **2. Protect Controls**

| Control                                                           | Meets Control? | Notes                                                          |
| ----------------------------------------------------------------- | -------------- | -------------------------------------------------------------- |
| Access control policies implemented                               | **No**         | No formal role-based access or least-privilege enforcement.    |
| Training and security awareness program                           | **No**         | Employees are not routinely trained on security or compliance. |
| Data security protections implemented                             | **No**         | No documented encryption standards or data handling processes. |
| Maintenance performed on systems                                  | **Yes**        | IT maintains systems but lacks standardized patch management.  |
| Protective technology in place (firewalls, filtering, monitoring) | **Yes**        | Firewalls exist, but monitoring is limited.                    |

---

## **3. Detect Controls**

| Control                        | Meets Control? | Notes                                                             |
| ------------------------------ | -------------- | ----------------------------------------------------------------- |
| Anomalies and events monitored | **No**         | Logging and monitoring are minimal; no SIEM or alerting in place. |
| Security continuous monitoring | **No**         | No proactive or automated detection solutions used.               |
| Detection processes documented | **No**         | No official detection procedures exist.                           |

---

## **4. Respond Controls**

| Control                                | Meets Control? | Notes                                                       |
| -------------------------------------- | -------------- | ----------------------------------------------------------- |
| Response planning established          | **No**         | No incident response plan (IRP) documented.                 |
| Communications process documented      | **No**         | No internal or external communication plan for incidents.   |
| Analysis processes established         | **No**         | Incidents are not formally analyzed or logged.              |
| Mitigation activities defined          | **No**         | No formal steps for containment, eradication, and recovery. |
| Improvements performed after incidents | **No**         | No continuous improvement process for incident response.    |

---

## **5. Recover Controls**

| Control                                 | Meets Control? | Notes                                                                    |
| --------------------------------------- | -------------- | ------------------------------------------------------------------------ |
| Recovery planning documented            | **No**         | No business continuity or disaster recovery plans in place.              |
| Improvements incorporated post-incident | **No**         | No structured lessons-learned process.                                   |
| Communications managed after recovery   | **No**         | No guidelines for notifying customers or stakeholders after an incident. |

---

## **6. Compliance Best Practices**

| Compliance Requirement                           | Meets Control? | Notes                                                               |
| ------------------------------------------------ | -------------- | ------------------------------------------------------------------- |
| PCI DSS controls in place for payment processing | **No**         | No evidence of PCI compliance; high financial risk.                 |
| GDPR requirements met for EU customers           | **No**         | No DPO, no data processing agreements, no documented GDPR controls. |
| Legal and regulatory mandates reviewed regularly | **No**         | No process for tracking regulatory changes.                         |
| Policies documented and reviewed                 | **No**         | Core policies (security, access, IRP, DRP) do not exist.            |

---

## **Recommendations (Optional)**

1. **Establish a formal asset inventory program** with automated asset-tracking tools.
2. **Create a full risk management strategy** that aligns with NIST CSF.
3. **Implement security awareness training** for all employees.
4. **Develop and enforce access control policies**, including least privilege and periodic access reviews.
5. **Document and implement an Incident Response Plan (IRP)** and Disaster Recovery Plan (DRP).
6. **Adopt logging and monitoring tools**, such as SIEM or centralized log management.
7. **Begin PCI DSS and GDPR compliance initiatives immediately**, given the payment processing and EU customer risks.
8. **Schedule quarterly internal audits** to track improvements and compliance status.

---

## **Self-Assessment (5 Points Total)**

| Statement                                                   | Yes/No  |
| ----------------------------------------------------------- | ------- |
| 1. I selected yes/no for every control                      | **Yes** |
| 2. I selected yes/no for every compliance best practice     | **Yes** |
| 3. I reviewed the Botium Toys scope and risk report         | **Yes** |
| 4. I used the Control Categories document to decide answers | **Yes** |
| 5. My checklist is complete and ready for portfolio use     | **Yes** |

**Score: 5/5 (100%)**
