## Overview

This lab focuses on understanding and applying Linux file permissions, ownership, and access control.
You worked inside a controlled practice directory to experiment with `chmod`, `chown`, users, groups, and permission testing.

---

## Lab Environment

* OS: Kali Linux (VirtualBox)
* User: `student`
* Directory: `~/permissions_lab`
* Tools Used: Bash shell, chmod, chown, ls, su

---

## Step 1: Create Lab Directory and Starter Files

```bash
mkdir ~/permissions_lab
cd ~/permissions_lab
touch report.txt secret.sh
ls -l
```

### Notes

* `report.txt` and `secret.sh` created with default permissions.
* At this stage, `secret.sh` is not executable.

### Evidence

Screenshot showing the output of `ls -l`.

---

## Step 2: Modify Permissions Using chmod

### Make secret.sh executable

```bash
chmod +x secret.sh
ls -l secret.sh
```

### Restrict report.txt to owner-only access

```bash
chmod 600 report.txt
ls -l report.txt
```

### Change permissions using numeric mode (example)

```bash
chmod 710 report.txt
```

### Notes

* `chmod +x` adds execute for the owner.
* `chmod 600` removes all permissions from group and others.
* `chmod 710` gives owner full access, group execute, others none.

### Evidence

Screenshot of updated permissions for both files.

---

## Step 3: Ownership and Group Management

### Create a new user for testing

```bash
sudo useradd labuser
sudo passwd labuser
```

### Change the owner of report.txt

```bash
sudo chown labuser report.txt
```

### Change the group of report.txt

```bash
sudo chown :labuser report.txt
```

### Verify changes

```bash
ls -l report.txt
```

### Notes

* Ownership is now assigned to `labuser`.
* File permissions behave differently once owner/group changes.

### Evidence

Screenshot showing `labuser labuser` as owner and group.

---

## Step 4: Test Access as the New User

### Switch to labuser

```bash
su - labuser
cd ~/permissions_lab
```

### Attempt to read report.txt

```bash
cat report.txt
```

### Attempt to execute secret.sh

```bash
./secret.sh
```

### Notes

* Access outcomes depend strictly on the permissions set earlier.
* If denied access, this confirms permissions were configured correctly.

---

## Step 5: Practice Translating Permission Formats

Fill in symbolic equivalents:

| Desired Permission | Symbolic Form | Numeric Form |
| ------------------ | ------------- | ------------ |
| rwxr-x---          | ?             | 750          |
| rw-rw-r--          | ?             | 664          |
| r-xr-xr-x          | ?             | 555          |

(Complete these in your notes.)

---

## Reflection

Write 5–7 sentences discussing the following:

* What you learned about Linux ownership and permissions.
* How permissions affected access when switching to another user.
* Differences between symbolic and numeric permission methods.
* How these concepts relate to cybersecurity and secure system configuration.
* Which parts of the lab felt most or least intuitive.

---

## Evidence Summary

Screenshots to include in `/Screenshots`:

* `2025-12-04_LinuxPerms_ls_initial.png`
* `2025-12-04_LinuxPerms_ls_changes.png`
* `2025-12-04_LinuxPerms_Ownership_Changed.png`
