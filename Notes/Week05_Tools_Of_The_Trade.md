# **Week 05 — Tools of the Trade: Linux & SQL**

**Date Range:** Dec 3 – Dec 7, 2025
**Total Hours:** [Fill at end of week]
**Phase:** Google Cybersecurity Certificate — Course 4

---

## **Topics Covered (Today — Dec 4)**

### **Module 2: The Linux Operating System**

**Key Concepts:**

* Linux file permissions: read, write, execute
* Ownership structure: user, group, others
* File system roles and directory responsibilities
* Why permissions matter for system hardening
* Relationship between users, groups, and privilege boundaries

**Important Terms:**

* **Owner:** The user who controls the file
* **Group:** A set of users with shared permissions
* **Permissions:** Defines what actions are allowed
* **Privilege:** Level of access a user holds
* **Access Control:** Mechanism controlling allowed actions

---

### **Module 3: Linux Commands in the Bash Shell**

**Key Concepts:**

* Navigation: `pwd`, `cd`, `ls`
* Directory management: `mkdir`, moving between levels
* File operations: `touch`, `cp`, `mv`, `rm`, `cat`
* Viewing permissions with `ls -l`
* User identity and sudo behavior
* How Bash is used in cybersecurity workflows

**Important Terms:**

* **Shell:** Interface that interprets commands
* **Bash:** Common Linux shell used for scripting and operations
* **Home Directory:** User-specific workspace
* **Sudo:** Temporary privilege elevation

---

## **Labs Completed (Dec 4)**

### **Linux Permissions Lab**

**Skills Practiced:**

* Changing permissions with `chmod`
* Understanding numeric vs symbolic modes
* Using `chown` to change ownership
* Verifying access as another user
* Testing permission boundaries with `su -`

**Key Takeaways:**

* Permission changes directly affect what another user can do.
* Ownership is separate from file permissions.
* Correct permission configuration is foundational for secure systems.

---

### **Linux Commands Lab**

**Skills Practiced:**

* Navigating directories
* Creating and managing files
* Copying, moving, and deleting data
* Reading file contents
* Using `sudo` and observing permission restrictions

**Key Takeaways:**

* Bash navigation is essential for cybersecurity workflows.
* File operations must be understood before exploiting or defending systems.
* Restricted access to `/root` illustrates privilege security in action.

---

## **Key Takeaways (Today)**

1. Permission management is a core component of Linux system security.
2. Understanding default permissions and ownership helps identify misconfigurations.
3. Bash command fluency makes future labs (SQL, DVWA, CVEs) more efficient.
4. Both labs reinforced real-world system administration skills.
5. Course content is beginning to shift from fundamentals to exploitation preparation.

---

## **Hands-On Work (Today)**

### **Lab Files Added:**

* `2025-12-04_Linux_Permissions_Lab.md`
* `2025-12-04_Linux_Commands_Lab.md`

### **Evidence Added:**

* Navigation, permissions, and file-operation screenshots
* Ownership and privilege test results

### **Why This Matters:**

These labs create the practical foundation for SQL Injection analysis, privilege escalation, and CVE reproduction in VulnForge.

---

## **Questions / Confusion**

* Is symbolic or numeric permission notation better for real-world use?
* When does a cybersecurity analyst need to modify group permissions vs user permissions?

---

## **Next Day Goals (Fri Dec 5)**

* Complete SQL Intermediate Lab
* Finish Module 4 (SQLi, XSS, CSRF)
* Write notes for Module 4
* Add lab file: `2025-12-05_SQL_Intermediate_Lab.md`
* Prepare environment for VulnForge CVE #1 (SQL Injection)

---

## **Reflection (Will complete on Dec 7)**

*(Leave blank until Sunday.)*

---
