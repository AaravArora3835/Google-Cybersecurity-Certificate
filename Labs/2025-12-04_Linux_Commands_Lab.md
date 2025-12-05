# **2025-12-04_Linux_Commands_Lab.md**

## Linux Commands Lab — Navigation, File Operations, and Bash Fundamentals

---

## Overview

This lab provides hands-on practice with essential Linux commands used for navigation, file management, directory control, and shell operations. It reinforces the core skill set required for Course 4 Module 3 and prepares you for future CVE testing, scripting, and system administration work.

---

## Lab Environment

* OS: Kali Linux (VirtualBox)
* User: `student`
* Working directory: `~/linux_commands_lab`
* Commands practiced: `pwd`, `ls`, `cd`, `mkdir`, `touch`, `cp`, `mv`, `rm`, `cat`, `sudo`, `whoami`

---

## Step 1: Create Practice Workspace

Commands used:

```bash
mkdir ~/linux_commands_lab
cd ~/linux_commands_lab
pwd
```

Notes:

* `mkdir` created an isolated directory for safe practice.
* `pwd` confirmed the absolute path of the working directory.

Evidence:

* Screenshot showing the creation of the directory and the output of `pwd`.

---

## Step 2: Directory Navigation and Listing Commands

Commands used:

```bash
mkdir projects notes
cd projects
pwd
cd ..
ls
ls -l
ls -la
```

Notes:

* `mkdir` created two subdirectories.
* `cd` was used to move in and out of directories.
* `ls -l` displayed permissions, owners, timestamps, and file details.
* `ls -la` displayed both visible and hidden files.

Evidence:

* Screenshot showing the results of `ls`, `ls -l`, and `ls -la`.

---

## Step 3: Creating, Copying, Moving, and Deleting Files

Commands used:

```bash
touch todo.txt ideas.txt
cp todo.txt todo_copy.txt
mv ideas.txt notes/
rm todo_copy.txt
cat todo.txt
ls -l
```

Notes:

* `touch` created empty files.
* `cp` duplicated `todo.txt`.
* `mv` relocated `ideas.txt` into the notes directory.
* `rm` permanently deleted the copied file.
* `cat` displayed file content.
* `ls -l` verified all changes after file operations.

Evidence:

* Screenshot showing file creation, file movement, deletion, and final `ls -l` output.

---

## Step 4: User Identity, Permissions Awareness, and sudo Testing

Commands used:

```bash
whoami
ls -l
sudo ls /root
```

Notes:

* `whoami` confirmed the active user.
* `ls -l` showed file permissions in the working directory.
* Attempting `sudo ls /root` demonstrated restricted access since `/root` is protected.
* This step confirmed privilege boundaries and how Linux enforces access control.

Evidence:

* Optional screenshot may be included to show permission denial for `/root`.

---

## Reflection

This lab improved my ability to navigate the Linux filesystem and understand how commands interact with directories and files. Creating, moving, copying, and deleting files helped clarify how Bash handles file operations. The differences between normal listing and detailed or hidden listings became clearer through repetition. Attempting a restricted sudo command showed how Linux maintains strict permission boundaries between regular users and administrative access. These foundational skills are essential for cybersecurity work, especially when investigating system behavior, analyzing attacks, or configuring secure environments. Overall, this lab made Bash commands more familiar and increased my confidence using Linux as a daily tool.

