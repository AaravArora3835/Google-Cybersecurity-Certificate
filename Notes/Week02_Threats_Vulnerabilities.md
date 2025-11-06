# Week 02 – Threats, Vulnerabilities & Tools

**Date Range:** Nov 3 – Nov 10, 2025
**Total Hours:** ~3 hrs (Modules 3–4 Progress + Tools Practice)
**Phase:** Google Cybersecurity Certificate

---

## Topics Covered

### 2025-11-03 — Module 3: *Protect Against Threats, Risks & Vulnerabilities*

**Key Concepts**

* **Threats, risks, and vulnerabilities** are interrelated: threats exploit vulnerabilities to cause harm, and risk measures the likelihood and impact of that harm.
* **Threat actors** include individuals or groups (hacktivists, cybercriminals, insiders, nation-states) who attempt to exploit weaknesses for financial, political, or personal gain.
* **Vulnerability** → flaw or weakness; **Exploit** → technique used to take advantage of that flaw.
* **Risk Formula:** `Risk = Likelihood × Impact` — helps prioritize mitigation efforts.
* **Defense Strategies:** patch management, least privilege, firewalls, IDS/IPS, regular vulnerability scans, and user training.
* **Incident Lifecycle:** Identify → Contain → Eradicate → Recover → Lessons Learned.

**Important Terms**

* **Threat Actor:** A person or entity intentionally causing harm to digital assets.
* **Vulnerability:** A flaw in hardware, software, or procedure that could be exploited.
* **Exploit:** A specific method or tool that takes advantage of a vulnerability.
* **Risk:** The probability and potential impact of a threat exploiting a vulnerability.
* **Mitigation:** Steps taken to reduce risk through technical or administrative controls.

**Screenshots**

* `2025-11-03_Module3_Completed.png` — Coursera completion screen for Module 3.

---

### 2025-11-04 — Module 4: *Cybersecurity Tools & Local Practice*

**Key Concepts / Tools Practiced**

* **Nmap (network discovery):** `nmap -sn 127.0.0.1` — local ping scan to confirm host is up.
* **Linux identity:** `whoami` — confirms current user context for privilege awareness.
* **File inspection:** `grep "root" /etc/passwd` — locates root account entries and demonstrates how to read system account files.
* Emphasis on safe, local testing (Host-Only Kali VM) and interpreting command outputs for reconnaissance.

**Important Terms**

* **Enumeration:** The process of collecting information from systems and services to identify potential attack vectors.
* **Host-Only Network:** VM networking mode used for isolated, safe testing without touching external networks.
* **Privilege Escalation (concept):** Moving from a lower-privilege user to root/admin by exploiting system weaknesses (studied conceptually here).

**Screenshots**

* `2025-11-04_Tool_Commands_Tested.png` — terminal showing `nmap`, `whoami`, and `grep` outputs.

**Reflection**
This activity reinforced how fundamental security tools operate at the system level. I practiced scanning localhost using Nmap, identifying the active host, verifying my current user, and exploring user privileges through `/etc/passwd`. These are foundational steps analysts use during reconnaissance and vulnerability assessments. Understanding them helps build intuition for network discovery and system enumeration—skills I’ll reuse in later labs and in SecureScholar’s *Network Threats* lesson.

---

## Key Takeaways

1. The link between threats, vulnerabilities, and risk drives all security decisions.
2. Tools like **Nmap**, **grep**, and **whoami** give analysts direct visibility into systems and networks.
3. Safe testing environments (Kali + Metasploitable) are essential for hands-on learning.
4. The risk formula provides measurable logic for prioritizing mitigation strategies.
5. Even small local scans teach the mindset of ethical testing and system analysis.

---

## Hands-On Labs

**Lab Name:** Module 4 – Local Tool Practice
**Activity Type:** Command-line simulation inside Kali VM
**Outcome:** Verified that system-level security tools are correctly installed and functioning. Practiced basic enumeration and output interpretation.

**Evidence**

* `2025-11-03_Module3_Completed.png`
* `2025-11-04_Tool_Commands_Tested.png`

---

## Questions / Confusion

* How do security teams automate repetitive tasks like scanning or parsing logs with scripts or cron jobs?
* Which additional Nmap flags are safe to test in a localhost-only environment?
* How can these same commands integrate into larger vulnerability assessment workflows?

---

## Next Steps

* Begin **Module 5 – Cybersecurity Tools & Programming (continued)**.
* Start **SecureScholar Module 2** — finalize HTML skeleton and begin Lesson 1 content.
* Run full **Vulnerability Scan Lab (Thursday)** against Metasploitable 2 in host-only mode and document findings.
* Keep screenshots + notes consistent with `YYYY-MM-DD_Description` format and commit with `doc:` / `feat:` prefixes.

---

**Status:** Module 3 complete; Module 4 (first half) complete — strong grasp of risks, vulnerabilities, and introductory tool usage. Ready to begin SecureScholar coding and local vulnerability scanning.
