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

# **Reflection (To be completed Dec 7)**

*(Leave blank until Sunday)*
