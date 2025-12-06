# **Week 05 — Tools of the Trade: Linux & SQL**

**Date Range:** Dec 3 – Dec 7, 2025
**Total Hours:** [Fill at end of week]
**Phase:** Google Cybersecurity Certificate — Course 4

---

# **Topics Covered (Today — Dec 3)**

### **Module 1: Introduction to Linux & Assets**

**Key Concepts:**

* Purpose of Linux in cybersecurity
* File system hierarchy (`/home`, `/etc`, `/var`)
* Absolute vs relative paths
* Basic navigation commands
* Why Linux is used in security operations
* Importance of assets, vulnerabilities, and threats
* Relationship between asset value and security posture

**Important Terms:**

* **CLI:** Command Line Interface
* **Permissions:** Read, Write, Execute
* **Asset:** Any valuable resource to protect
* **Vulnerability:** Weakness an attacker can exploit
* **Threat:** Anything that can exploit a vulnerability

---

# **Labs Completed (Dec 3)**

### **Linux Basics Lab**

**Commands Practiced:**
`pwd`, `ls`, `cd`, `mkdir`, `touch`, `chmod`, `sudo`, `whoami`

**Key Takeaways:**

* Linux navigation is foundational before doing exploitation.
* Understanding permissions is essential for hardening systems.
* Everything in Linux is a file, which makes behavior predictable.

---

# **Key Takeaways (Dec 3)**

1. Linux navigation commands support almost every security workflow.
2. The asset–vulnerability–threat relationship is the foundation of risk management.
3. Setting up the VulnForge tool today prepares for future CVE work.

---

# **Hands-On Work (Dec 3)**

### **VulnForge Tool Update**

**Improvement Added:**

* Added `source_url` field to `new_case.py`.
* Tested the tool and confirmed metadata appears in notes.md.

**Why This Matters:**
Automates consistency across 12+ CVE reproductions.

---

# **Questions / Confusion (Dec 3)**

* How advanced will SQL become in this course?
* Should I supplement SQL practice with DVWA or TryHackMe?

---

# **Next Day Goals (Thu Dec 4)**

* Complete Linux Permissions Lab
* Complete Linux Commands Lab
* Add both files to `/Labs`
* Add Thursday notes to Week05 file

---

# **Topics Covered (Today — Dec 4)**

### **Module 2: The Linux Operating System**

**Key Concepts:**

* Linux file permissions (r, w, x)
* Users, groups, and others
* Why permissions matter for system security
* Directory responsibilities and file system behavior
* Privilege boundaries inside Linux

**Important Terms:**

* **Owner:** User who controls the file
* **Group:** Assigned group with shared rights
* **Permissions:** Actions allowed on a file
* **Privilege:** Level of access a user holds
* **Access Control:** Mechanism that enforces allowed actions

---

### **Module 3: Linux Commands in the Bash Shell**

**Key Concepts:**

* Navigation with `pwd`, `cd`, `ls`
* Directory creation
* File operations (`touch`, `cp`, `mv`, `rm`, `cat`)
* Permission checking with `ls -l`
* User identity (`whoami`)
* Testing privilege boundaries with `sudo`

**Important Terms:**

* **Shell:** Command interpreter
* **Bash:** Most common Linux shell
* **Home Directory:** User workspace
* **Sudo:** Temporary privilege escalation

---

# **Labs Completed (Dec 4)**

### **Linux Permissions Lab**

**Skills Practiced:**

* `chmod` symbolic vs numeric
* `chown` for user and group ownership
* Switching users and testing access restrictions
* Viewing permission changes with `ls -l`

**Key Takeaways:**

* Permissions directly control what users can or cannot do.
* Ownership is separate from permissions.
* Proper file permissions prevent privilege misuse.

---

### **Linux Commands Lab**

**Skills Practiced:**

* Directory creation and movement
* File creation, copying, moving, deleting
* Using `cat` to view file contents
* Observing permission-denied results with `/root`

**Key Takeaways:**

* Bash fluency is required before exploitation or defensive work.
* File operations must be understood to identify misconfigurations.
* Permission-denied outputs show how Linux enforces boundaries.

---

# **Key Takeaways (Dec 4)**

1. Permission management strengthens system security.
2. Ownership vs permissions must be understood for access auditing.
3. Bash skills make future labs significantly faster.
4. Linux fundamentals support DVWA, SQLi, and CVE workflows.

---

# **Hands-On Work (Dec 4)**

**Lab Files Added:**

* `2025-12-04_Linux_Permissions_Lab.md`
* `2025-12-04_Linux_Commands_Lab.md`

**Evidence Added:**

* Navigation, permission, and file operation screenshots
* Ownership change verification

**Why This Matters:**
Real Linux experience prepares for SQLi labs and future CVE exploitation.

---

# **Questions / Confusion (Dec 4)**

* Is numeric or symbolic permission notation preferred in production?
* When should permissions be modified at the group level vs the user level?

---

# **Next Day Goals (Fri Dec 5)**

* Complete SQL Intermediate Lab
* Finish Module 4 (SQLi, XSS, CSRF)
* Update Week05 notes with Module 4
* Add lab file: `2025-12-05_SQL_Intermediate_Lab.md`
* Prepare system for SQL injection testing (DVWA or equivalent)

---

# **Topics Covered (Today — Dec 5)**

### **Module 4: Web Vulnerabilities (SQLi, XSS, CSRF)**

**Key Concepts:**

* How databases interact with web applications
* SQL injection fundamentals
* Cross-site scripting and script injection risks
* Cross-site request forgery and session abuse
* Input validation and prepared statements
* Why user-supplied data is dangerous

**Important Terms:**

* **SQL Injection:** Manipulating queries through user input
* **XSS:** Injecting malicious JavaScript into pages
* **CSRF:** Forcing actions through forged requests
* **Prepared Statement:** Safe, parameterized SQL query
* **Input Validation:** Filtering and sanitizing user input

---

# **Labs Completed (Dec 5)**

### **SQL Intermediate Lab**

**Skills Practiced:**

* Creating a database and table
* Inserting data (`INSERT`)
* Modifying rows (`UPDATE`)
* Deleting rows (`DELETE`)
* Sorting results with `ORDER BY`
* Verifying each operation with `SELECT`

**Key Takeaways:**

* SQL modification commands are powerful and potentially destructive.
* `WHERE` clauses must be precise to avoid accidental changes.
* Sorting data helps identify highest-impact records.
* Understanding normal SQL behavior is required before learning SQL injection.

---

# **Key Takeaways (Dec 5)**

1. SQL operations form the base layer for understanding SQL injection attacks.
2. Database modification commands require careful verification.
3. Module 4 connects theory (web vulnerabilities) with practice (SQL operations).
4. Completing today’s lab builds confidence with real database environments.
5. Today’s work sets the stage for VulnForge SQL Injection testing.

---

# **Hands-On Work (Dec 5)**

**Lab File Added:**

* `2025-12-05_SQL_Intermediate_Lab.md`

**Evidence Added:**

* Final SQL output screenshot:
  `2025-12-05_SQL_IntermediateLab_Completed.png`

**Why This Matters:**
These SQL operations mirror the exact commands that attackers manipulate during injection attacks.

---

# **Questions / Confusion (Dec 5)**

* How often do real-world developers still rely on raw SQL versus ORMs?
* What common mistakes lead to SQL injection in beginner-level applications?

---

# **Next Day Goals (Sat Dec 6)**

* Create CVE #1 directory with `new_case.py`
* Set up DVWA or SQLi TryHackMe room
* Fill in CVE #1 notes: Summary, Lab Environment, Basic Payloads
* Perform at least one SQLi attempt (success not required yet)
* Add Saturday notes

---

## **Reflection (Will complete on Dec 7)**

*(Leave blank until Sunday.)*

---
