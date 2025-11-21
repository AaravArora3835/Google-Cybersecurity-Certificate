# Week 03 — Course 2: Risk Management Foundations

**Date Range:** Nov 10 – Nov 16, 2025  
**Status:** ✅ Completed

---

## 2025-11-10 — Course 2 Modules 1 & 2: Risk Management Foundations

**Status:** ✅ Completed  
**Modules:**
1. Understanding Risk Management Concepts
2. Identifying and Assessing Risks

---

### **Overview**

Began *Course 2 – Play It Safe: Manage Security Risks* on Coursera.
Focused on how cybersecurity professionals define, categorize, and evaluate risk using structured frameworks such as **NIST SP 800-30** and the **Risk Management Framework (RMF)**.
These modules connect the abstract idea of "risk" with measurable processes and real-world examples.

---

### **Key Concepts**

**Risk Formula:**
> Risk = Likelihood × Impact

**Terminology**

| Term              | Definition                                                                   | Example                                    |
| ----------------- | ---------------------------------------------------------------------------- | ------------------------------------------ |
| **Threat**        | Potential event or actor that can cause harm                                 | Hacker, malware, insider                   |
| **Vulnerability** | Weakness an attacker can exploit                                             | Unpatched software, reused passwords       |
| **Risk**          | Probability that a threat will exploit a vulnerability × impact of the event | 70% chance of credential theft → High risk |
| **Control**       | Safeguard reducing likelihood or impact                                      | MFA, security policy, firewall             |

**Control Types**
* **Administrative:** Policies, training, background checks
* **Technical:** Firewalls, encryption, access controls
* **Physical:** Locks, cameras, secure facilities

---

### **NIST SP 800-30 Process**

1. Identify assets and system boundaries
2. Identify threats and vulnerabilities
3. Determine likelihood and impact
4. Calculate overall risk
5. Recommend and implement controls
6. Monitor and update continuously

```text
Assets → Threats → Vulnerabilities → Risk → Controls
```

**Example:**
A school's Wi-Fi network (asset) uses default passwords (vulnerability).
If a student runs a network-sniffing tool (threat), the likelihood = high, impact = moderate, producing a medium-to-high risk.
Applying WPA3 + unique passphrase (control) reduces the risk.

---

### **Risk Management Framework (RMF)**

The NIST RMF organizes risk work into seven recurring phases:

1. **Prepare** – Set context, assign roles, define risk tolerance
2. **Categorize** – Determine system criticality and sensitivity
3. **Select** – Choose appropriate NIST SP 800-53 controls
4. **Implement** – Apply and configure controls
5. **Assess** – Evaluate control effectiveness
6. **Authorize** – Approve operation and formally accept risk
7. **Monitor** – Continuously track and update as threats evolve

---

### **CIS Controls (Practical Perspective)**

Reviewed **CIS v8** to map enterprise controls to personal digital safety:

* **CIS 1 – Inventory Assets:** Know what devices/accounts exist.
* **CIS 5 – Account Management:** Use unique credentials + 2FA.
* **CIS 8 – Malware Defense:** Keep devices patched and antivirus enabled.

---

## 2025-11-10 — Course 2 Modules 3 & 4: Security Controls & Incident Response

**Status:** ✅ Completed  
**Modules:**
3. Security Frameworks and Controls
4. Incident Response and Risk Mitigation

---

### **Overview**

Completed remaining modules covering security frameworks (NIST CSF, OWASP), the CIA triad, risk mitigation strategies, and the incident response lifecycle. Applied concepts through the Botium Toys security audit capstone project.

---

### **Key Concepts**

**CIA Triad:**
* **Confidentiality:** Only authorized users access data
* **Integrity:** Data remains accurate and unaltered  
* **Availability:** Systems remain accessible when needed

**Risk Mitigation Strategies:**
* **Acceptance** — Acknowledge risk, take no action (low likelihood × low impact)
* **Avoidance** — Eliminate the activity causing risk
* **Transference** — Shift risk to another party (insurance, outsourcing)
* **Mitigation** — Implement controls to reduce likelihood or impact

**Incident Response Lifecycle:**
1. Preparation
2. Detection & Analysis
3. Containment
4. Eradication
5. Recovery
6. Post-Incident Activity (lessons learned)

---

### **Reflection**

Today's lessons reframed risk as a measurable process rather than intuition.
Understanding how *likelihood* and *impact* interact made cybersecurity feel analytical instead of abstract.
The RMF clarified that security is continuous — each stage feeds the next.

Course 2 built directly on Course 1's foundations, showing how the CIA Triad and threat concepts translate into structured risk management frameworks that organizations use daily.

---

### **Evidence**

* `Screenshots/2025-11-10_Course2_Completed.png` — Coursera completion certificate

---

**Status:** Course 2 Complete ✅  
**Next:** Course 3 – Connect and Protect: Networks and Network Security
