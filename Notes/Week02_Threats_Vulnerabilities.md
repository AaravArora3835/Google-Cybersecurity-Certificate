# Week 02 – Threats, Vulnerabilities & Tools

**Date Range:** Nov 3 – Nov 10, 2025
**Total Hours:** ~9.5 hrs (Modules 3–4 + Labs Complete)
**Phase:** Google Cybersecurity Certificate — Course 1 Completed

---

## Topics Covered

### 2025-11-03 — Module 3: Protect Against Threats, Risks & Vulnerabilities

**Key Concepts**

* **Threats, risks, and vulnerabilities** are interrelated. Threats exploit vulnerabilities to cause harm; risk measures likelihood × impact.
* **Threat actors** include cybercriminals, hacktivists, insiders, and nation-states, each with distinct motives.
* **Vulnerability → Exploit:** a flaw vs. the technique used to take advantage of it.
* **Risk formula:** `Risk = Likelihood × Impact` to prioritize mitigation.
* **Defensive measures:** patch management, least privilege, firewalls, IDS/IPS, and security training.
* **Incident Lifecycle:** Identify → Contain → Eradicate → Recover → Lessons Learned.

**Evidence**

* `Screenshots/2025-11-03_Module3_Completed.png` — Coursera completion screen for Module 3.

---

### 2025-11-04 — Module 4: Cybersecurity Tools & Local Practice

**Commands Tested**

```bash
nmap -sn 127.0.0.1
whoami
grep "root" /etc/passwd
```

**Purpose**

| Command                   | Function                                     | Result                               |
| ------------------------- | -------------------------------------------- | ------------------------------------ |
| `nmap -sn 127.0.0.1`      | Scans local host to verify network response. | Host is up (127.0.0.1)               |
| `whoami`                  | Displays current user context.               | labuser                              |
| `grep "root" /etc/passwd` | Finds root entries in system file.           | `root:x:0:0:root:/root:/usr/bin/zsh` |

Executed safely within an isolated Kali VM using Host-Only networking.

**Evidence**

* `Screenshots/2025-11-07_Tool_Commands_Tested.png` — Verified local tool outputs.

**Reflection**

This mini-lab reinforced core command-line skills and how they connect to vulnerability analysis.
Testing tools locally helped validate system visibility and privilege checks in a controlled environment.

---

### 2025-11-07 — Vulnerability Scan Lab (Docker + Nmap on Juice Shop)

**Overview**

Configured Docker in Kali, launched the OWASP Juice Shop container, and performed a series of Nmap scans to simulate vulnerability enumeration on a local web application.

**Steps Taken**

1. Verified Docker service installation and startup.
2. Ran Juice Shop container:

   ```bash
   docker run -d -p 3000:3000 bkimminich/juice-shop
   ```
3. Confirmed application availability at `http://127.0.0.1:3000`.
4. Checked network reachability via:

   ```bash
   ping -c 4 127.0.0.1
   ```
5. Validated open port (3000/tcp) using:

   ```bash
   sudo ss -tuln | grep 3000
   ```
6. Conducted Nmap scans to identify services and headers:

   ```bash
   sudo nmap -p 3000 -sS -sV 127.0.0.1
   sudo nmap -p 3000 --script http-enum,http-headers,http-server-header 127.0.0.1
   sudo nmap -p 3000 --script vuln 127.0.0.1
   ```

**Evidence**

* `Screenshots/2025-11-07_Docker_Install_Success.png`
* `Screenshots/2025-11-07_JuiceShop_App_Up.png`
* `Screenshots/2025-11-07_Ping_OK.png`
* `Screenshots/2025-11-07_nmap_sV_output.png`
* `Screenshots/2025-11-07_nmap_http_output.png`

**Reflection**

This lab demonstrated practical network reconnaissance and vulnerability scanning techniques.
By testing a local containerized application, I safely observed how services respond to probes and how Nmap scripts identify metadata such as headers and server types.
It reinforced ethical testing principles and the importance of working within isolated environments.

---

### 2025-11-05 — Course 1 Completion (Foundations of Cybersecurity)

**Summary**

Completed all modules, hands-on exercises, and the final quiz for Course 1.
Earned the Coursera certificate and recorded completion for portfolio integration.

**Evidence**

* `Screenshots/2025-11-05_Module4_Completed.png`

**Reflection**

Course 1 built a solid foundation in both theory and practical skills—from risk assessment to command-line execution.
It connected the CIA Triad to hands-on operations, laying the groundwork for risk management in Course 2 and for SecureScholar’s teaching modules.

---

## Key Takeaways

1. Completed Course 1 of the Google Cybersecurity Certificate.
2. Built proficiency in core Kali commands and network reconnaissance.
3. Practiced Nmap scanning and interpreted service outputs.
4. Reinforced secure lab practice and ethical testing boundaries.
5. Established foundation for Course 2 and SecureScholar development.

---

## Hands-On Labs

| Lab Name                                 | Outcome                                          | Evidence                                                           |
| ---------------------------------------- | ------------------------------------------------ | ------------------------------------------------------------------ |
| Local Tool Verification                  | Validated nmap, whoami, and grep within Kali VM. | `2025-11-07_Tool_Commands_Tested.png`                              |
| Vulnerability Scan (Docker + Juice Shop) | Launched container and ran multiple Nmap scans.  | `2025-11-07_nmap_sV_output.png`, `2025-11-07_nmap_http_output.png` |

---

## Next Steps

* Begin **Course 2 – Play It Safe: Manage Security Risks** on Nov 10.
* Continue SecureScholar Module 2 (JavaScript quiz system).
* Prepare weekly reflection update for `Reflection.md`.
* Capture additional evidence screenshots for Course 2 setup.

---

## Professional Statement (Aarav Arora) — Draft Added Nov 7 2025

> My name is **Aarav Arora**, a high-school student committed to cybersecurity education and digital safety. Through this certificate and hands-on labs, I am building a foundation of skills in network security, Linux administration, and threat analysis.
> I value integrity, persistence, and precision in problem-solving. I see cybersecurity as a discipline that combines technical expertise with ethical responsibility. My goal is to defend systems, protect users, and build awareness that helps others stay safe online.
> As I advance to Course 2 and beyond, I plan to apply these principles in both professional projects and community initiatives like SecureScholar, which aim to make cybersecurity accessible for students and families.

---

**Status:** Course 1 (Foundations of Cybersecurity) Completed | Vulnerability Scan Lab Completed | Local Tools Practice Verified | Week 02 Fully Documented.
