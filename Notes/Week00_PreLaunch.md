# Week 00 – Pre-Launch Setup (October 12–13, 2025)

## Overview

Week 00 established the technical and documentation foundation for the **Google Cybersecurity Certificate**.
The goal was to confirm system readiness, verify VM connectivity, and complete the Coursera Financial Aid process.

---

## Day 1 – Sunday, October 12, 2025

### Steps Taken

1. **Booted** Kali Linux, Windows 10, and Ubuntu Server in VirtualBox.
2. **Verified** host-only network connectivity between VMs using ping commands.
3. **Finalized** GitHub repository structure for documentation consistency.
4. **Organized** local folders to match the v4.8 Foundation format.

---

### Commands Used

ipconfig – Checked host-only adapter IP on Windows
ifconfig – Verified adapter IPs on Kali and Ubuntu
ping -c 4 192.168.56.101 – Confirmed cross-VM connectivity

---

### Errors & Fixes

* **Issue:** Ping from Kali to Windows failed initially.
  **Fix:** Enabled ICMP Echo Request in Windows Firewall and re-tested successfully.

* **Issue:** Snapshot labels inconsistent across VMs.
  **Fix:** Renamed all snapshots to Clean_Oct2025.

---

### Evidence

* **VMs Successfully Booted:** 
![VM Boot Success](/Screenshots/2025-10-12_VMs_Succesfully_Booted.png)
* **Network Connectivity Test:**
![Ping Test Readiness Check](/Screenshots/2025-10-12_Ping_Test_Readiness_Check.png)
* **Repository Structure Verified:** 
![GitHub Repository Review](/Screenshots/2025-10-12_GitHub_Repo_Review.png)

---

### Reflection

All virtual machines and network connections were verified successfully.
This confirmed full system readiness for the upcoming Google Cybersecurity Certificate course and established a clean documentation workflow for the project.

---

## Day 2 – Monday, October 13, 2025

### Steps Taken

1. Completed Coursera Financial Aid application for the Google Cybersecurity Professional Certificate.
2. Wrote motivation essay focused on accessibility, professional growth, and long-term career goals.
3. Verified submission and received confirmation email from Coursera.

---

### Evidence

* **Coursera Financial Aid Pending Screenshot #1:**
![Financial Aid Step 1 – Application Screenshot 1](/Screenshots/2025-10-13_Coursera_Financial_Aid_Application_1.png)
* **Coursera Financial Aid Pending Screenshot #2:**
![Financial Aid Step 2 – Application Screenshot 2](/Screenshots/2025-10-13_Coursera_Financial_Aid_Application_2.png)
* **Coursera Financial Aid Pending Screenshot #3:**
![Financial Aid Step 3 – Application Screenshot 3](/Screenshots/2025-10-13_Coursera_Financial_Aid_Application_3.png)

---

### Reflection

Submitting the financial-aid application marked the formal start of my certification journey.
All pre-launch tasks are complete, ensuring a fully prepared environment for the course launch on October 27, 2025.

---

## End-of-Week Summary

### Key Learnings

* Practiced network diagnostics in VirtualBox.
* Standardized file naming and folder layout for documentation consistency.
* Completed Coursera Financial Aid application process and essay.

### Challenges

* Configuring Windows Firewall to allow ICMP traffic.
* Synchronizing local and GitHub directory structures.

### Next Steps

* Await financial-aid approval (expected ≈ October 29, 2025).
* Begin Introduction to Cybersecurity module.
* Continue weekly documentation and reflections every Saturday.
