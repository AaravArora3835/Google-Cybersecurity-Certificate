# **Week 05 — Tools of the Trade: Linux & SQL**

**Date Range:** Dec 3 – Dec 7, 2025
**Total Hours:** [Fill at end of week]
**Phase:** Google Cybersecurity Certificate — Course 4

---

# **Topics Covered (Dec 3)**

### **Module 1: Introduction to Linux & Assets**

**Key Concepts:**

* Why Linux matters for security work
* File system hierarchy (`/home`, `/etc`, `/var`)
* Absolute vs relative paths
* Basic navigation commands
* Assets, vulnerabilities, and threats framework
* How asset value drives security decisions

**Important Terms:** CLI, Permissions, Asset, Vulnerability, Threat

---

# **Labs Completed (Dec 3)**

### **Linux Basics Lab**

**Commands Practiced:**
`pwd`, `ls`, `cd`, `mkdir`, `touch`, `chmod`, `sudo`, `whoami`

**Key Takeaways:**

* Need solid Linux navigation before touching exploitation tools.
* Permissions control system behavior — critical for security work.
* Linux treats everything as a file, which makes system control consistent.

---

# **Key Takeaways (Dec 3)**

1. Navigation commands are foundational for most security workflows.
2. Asset–vulnerability–threat structure shows up everywhere in risk management.
3. VulnForge updates keep CVE documentation consistent.

---

# **Hands-On Work (Dec 3)**

### **VulnForge Tool Update**

* Added `source_url` field to `new_case.py`.
* Verified new metadata shows in template output.

**Purpose:** Keep future CVE cases formatted uniformly.

---

# **Next Day Goals (Dec 4)**

* Linux Permissions Lab
* Linux Commands Lab
* Add both labs to `/Labs`
* Document Thursday progress

---

# **Topics Covered (Dec 4)**

### **Module 2: The Linux Operating System**

**Key Concepts:**

* File permissions (read, write, execute)
* Users, groups, others
* Why permissions matter for system security
* Directory responsibilities
* Privilege boundaries

**Important Terms:** Owner, Group, Permissions, Privilege, Access Control

---

### **Module 3: Linux Commands in Bash**

**Key Concepts:**

* Navigation and directory structure
* File manipulation (`touch`, `cp`, `mv`, `rm`, `cat`)
* Checking permissions with `ls -l`
* Identity and escalation (`whoami`, `sudo`)

**Important Terms:** Shell, Bash, Home Directory, Sudo

---

# **Labs Completed (Dec 4)**

### **Linux Permissions Lab**

**Skills Practiced:**

* `chmod` symbolic vs numeric notation
* `chown` for ownership changes
* Testing access by switching users
* Inspecting permission changes

**Key Takeaways:**
Permissions control what users can actually do.
Ownership and permissions are separate — both matter.
Proper access control prevents system misuse.

---

### **Linux Commands Lab**

**Skills Practiced:**

* Creating and navigating directories
* File creation, modification, deletion
* Viewing contents with `cat`
* Hitting permission-denied cases

**Key Takeaways:**
Bash fluency speeds up lab work significantly.
File operations reveal potential misconfigurations.
Permission-denied messages enforce privilege boundaries.

---

# **Key Takeaways (Dec 4)**

1. Correct permission setup is required for secure systems.
2. Understanding ownership matters for access audits.
3. Bash skills directly support SQLi and CVE work.

---

# **Hands-On Work (Dec 4)**

Files created:
`2025-12-04_Linux_Permissions_Lab.md`
`2025-12-04_Linux_Commands_Lab.md`

Evidence:
Navigation, permission, and ownership screenshots.

**Purpose:** Build systems knowledge before SQLi testing.

---

# **Next Day Goals (Dec 5)**

* Complete SQL Intermediate Lab
* Finish Module 4
* Add SQL lab to `/Labs`
* Update Week05 notes
* Prep for DVWA SQL injection work

---

# **Topics Covered (Dec 5)**

### **Module 4: Web Vulnerabilities**

**Key Concepts:**

* SQL injection fundamentals
* Cross-site scripting (XSS)
* Cross-site request forgery (CSRF)
* Secure input validation
* Prepared statements and safe query execution

**Important Terms:** SQL Injection, XSS, CSRF, Prepared Statement, Input Validation

---

# **Labs Completed (Dec 5)**

### **SQL Intermediate Lab**

**Skills Practiced:**

* Creating tables
* Inserting records (`INSERT`)
* Updating records (`UPDATE`)
* Deleting records (`DELETE`)
* Sorting with `ORDER BY`
* Verifying changes using `SELECT`

**Key Takeaways:**
SQL modification commands need careful handling.
Accurate `WHERE` clauses prevent unintended changes.
SQL fundamentals are required before testing injection attacks.

---

# **Key Takeaways (Dec 5)**

1. SQL operations are the foundation for understanding SQL injection.
2. Module 4 connects database concepts with real exploits.
3. SQL Intermediate Lab sets up CVE #1 testing.

---

# **Hands-On Work (Dec 5)**

File added:
`2025-12-05_SQL_Intermediate_Lab.md`

Evidence:
`2025-12-05_SQL_IntermediateLab_Completed.png`

**Purpose:** Learn normal SQL behavior before exploring injection techniques.

---

# **Next Day Goals (Dec 6)**

* Initialize VulnForge CVE #1
* Set up DVWA or TryHackMe SQLi
* Fill Summary, Lab Environment, Payloads sections
* Conduct first SQL injection attempt

---

# **Topics Covered (Dec 6)**

### **CVE Case Study #1: SQL Injection**

**Key Concepts:**

* Union-based SQL injection
* Error-based information gathering
* Database enumeration techniques
* Payload crafting and testing
* Attack surface analysis

**Important Terms:** Union Select, Database Schema, Payload, Enumeration, Attack Vector

---

# **Labs Completed (Dec 6)**

### **VulnForge CVE #1 — SQL Injection Attack**

**Skills Practiced:**

* Initializing VulnForge case structure
* Setting up DVWA SQL injection lab
* Testing basic injection payloads
* Documenting attack methodology
* Recording proof-of-concept exploits

**Key Takeaways:**
Real exploitation requires methodical payload testing.
Documentation during attack matters for reports.
Understanding SQL structure enables better injection techniques.

---

# **Key Takeaways (Dec 6)**

1. VulnForge documentation creates professional portfolio evidence.
2. SQL injection testing combines Linux, SQL, and web security knowledge.
3. Attack methodology needs to be reproducible and clear.

---

# **Hands-On Work (Dec 6)**

VulnForge work:
* Ran `python new_case.py` for CVE #1
* Documented lab environment setup
* Captured initial payloads and results
* Added screenshots to `/Evidence`

**Purpose:** Create first complete CVE case study for portfolio.

---

# **Next Day Goals (Dec 7)**

* Complete CVE #1 write-up
* Add mitigation section
* Review week's progress
* Fill reflection and total hours
* Plan Week 06 priorities

---

# **Topics Covered (Dec 7)**

### **CVE #1 Completion & Review**

**Key Concepts:**

* Mitigation strategies for SQL injection
* Defensive coding practices
* Input validation and sanitization
* Prepared statements implementation
* Security testing best practices

**Important Terms:** Parameterized Query, Whitelist Validation, Least Privilege, Defense in Depth

---

# **Labs Completed (Dec 7)**

### **CVE #1 Final Documentation**

**Skills Practiced:**

* Writing clear mitigation recommendations
* Explaining technical concepts for non-technical readers
* Organizing evidence for portfolio review
* Creating reproducible attack documentation

**Key Takeaways:**
Complete documentation requires offense and defense perspectives.
Mitigation advice shows security thinking beyond exploitation.
Portfolio quality depends on clear communication.

---

# **Key Takeaways (Dec 7)**

1. CVE #1 integrates Linux, SQL, and web security concepts from entire week.
2. Documentation quality directly impacts internship readiness.
3. Week 05 built foundational skills for upcoming exploitation work.

---

# **Hands-On Work (Dec 7)**

Files finalized:
* Complete CVE #1 case study with all sections
* Week 05 notes updated with full progress
* Evidence organized in `/Evidence` directory

**Purpose:** Deliver complete, portfolio-ready case study.

---

# **Weekly Reflection**

**What Worked:**
* Consistent lab documentation made CVE #1 write-up easier.
* Linux and SQL skills transferred directly to injection testing.
* VulnForge structure kept work organized and professional.

**What Could Improve:**
* Could have started CVE #1 earlier in the week for more testing time.
* Need to balance speed with documentation quality.
* Should review previous week's notes before starting new topics.

**Connections Made:**
* Linux permissions relate to privilege escalation attacks.
* SQL fundamentals are required for understanding injection impact.
* Asset management concepts apply to prioritizing vulnerabilities.

**Next Week Focus:**
* Complete Course 4 if remaining modules exist.
* Begin Course 5 or start second CVE case study.
* Maintain lab documentation consistency.
* Review GitHub portfolio presentation.

---

# **Week 05 Summary**

**Certifications Progress:** Course 4 content — significant progress
**Labs Completed:** 4 (Linux Basics, Permissions, Commands, SQL Intermediate)
**CVE Cases:** 1 (SQL Injection — first complete case study)
**Tools Used:** VulnForge, DVWA, Kali Linux, Bash, SQL
**GitHub Updates:** All labs documented, CVE #1 added to portfolio

**Portfolio Impact:**
First complete CVE case study demonstrates hands-on exploitation skills. Linux and SQL lab documentation shows foundational competency. VulnForge structure proves organized methodology for future case studies.

**Recruiter Takeaway:**
Candidate successfully documented real SQL injection attack with mitigation recommendations. Technical writing quality matches hands-on skills. Evidence shows systematic approach to vulnerability research.
