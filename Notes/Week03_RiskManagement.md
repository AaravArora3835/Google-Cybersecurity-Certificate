### 2025-11-10 — Course 2 Modules 1 & 2 : Risk Management Foundations

**Status:** ✅ Completed
**Modules:**

1. Understanding Risk Management Concepts
2. Identifying and Assessing Risks

---

#### **Overview**

Began *Course 2 – Play It Safe: Manage Security Risks* on Coursera.
Focused on how cybersecurity professionals define, categorize, and evaluate risk using structured frameworks such as **NIST SP 800-30** and the **Risk Management Framework (RMF)**.
These modules connect the abstract idea of “risk” with measurable processes and real-world examples.

---

#### **Key Concepts**

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

#### **NIST SP 800-30 Process**

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
A school’s Wi-Fi network (asset) uses default passwords (vulnerability).
If a student runs a network-sniffing tool (threat), the likelihood = high, impact = moderate, producing a medium-to-high risk.
Applying WPA3 + unique passphrase (control) reduces the risk.

---

#### **Risk Management Framework (RMF)**

The NIST RMF organizes risk work into seven recurring phases:

1. **Prepare** – Set context, assign roles, define risk tolerance
2. **Categorize** – Determine system criticality and sensitivity
3. **Select** – Choose appropriate NIST SP 800-53 controls
4. **Implement** – Apply and configure controls
5. **Assess** – Evaluate control effectiveness
6. **Authorize** – Approve operation and formally accept risk
7. **Monitor** – Continuously track and update as threats evolve

**Evidence:**
`Screenshots/2025-11-10_RiskFrameworks.png` — Coursera slide showing the seven RMF steps.

---

#### **CIS Controls (Practical Perspective)**

Reviewed **CIS v8** to map enterprise controls to personal digital safety:

* **CIS 1 – Inventory Assets:** Know what devices/accounts exist.
* **CIS 5 – Account Management:** Use unique credentials + 2FA.
* **CIS 8 – Malware Defense:** Keep devices patched and antivirus enabled.

---

#### **Guardians Issue #1 Outline Draft**

**Title:** *Play It Safe at Home — 3 Ways to Lower Your Digital Risk*

1. Why “Risk” isn’t a Scary Word (L × I in plain English)
2. Three Common Threats (Phishing, Password Reuse, Weak Wi-Fi)
3. Simple Controls (Password Managers, 2FA, Updates)
   *File:* `Guardians/2025-11-12_Issue01_PlayItSafe.md`

---

#### **Reflection**

Today’s lessons reframed risk as a measurable process rather than intuition.
Understanding how *likelihood* and *impact* interact made cybersecurity feel analytical instead of abstract.
The RMF clarified that security is continuous — each stage feeds the next.
Translating those ideas into the Guardians outline proved I can teach them simply, a key step toward my outreach goals.
