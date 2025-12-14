# File Permissions in Linux

## Project Description

In this project, I used Linux commands to examine and modify file and directory permissions. The goal was to understand how permissions control access to files and directories, and how security professionals use permission management to protect systems from unauthorized access.

---

## Check File and Directory Details

I used the `ls -l` command to view detailed information about files and directories, including permission settings, ownership, and group assignment.

Example:

```bash
ls -l
```

This command displays:

* File type
* Permission string
* Number of links
* Owner and group
* File size
* Last modification date
* File or directory name

---

## Describe the Permissions String

A permissions string consists of **10 characters**:

Example:

```text
-rwxr-xr--
```

Breakdown:

* **First character**: file type

  * `-` = regular file
  * `d` = directory
* **Next three**: owner permissions
* **Next three**: group permissions
* **Last three**: others permissions

Permission meanings:

* `r` = read
* `w` = write
* `x` = execute
* `-` = permission not granted

---

## Change File Permissions

I used the `chmod` command to modify file permissions.

Example:

```bash
chmod 640 file.txt
```

This sets:

* Owner: read and write
* Group: read
* Others: no access

Changing permissions ensures that only authorized users can access or modify files.

---

## Change File Permissions on a Hidden File

Hidden files begin with a dot (`.`). Permissions are changed the same way as regular files.

Example:

```bash
chmod 600 .hidden_file
```

This restricts access so only the owner can read and write the file, improving security for sensitive configuration files.

---

## Change Directory Permissions

Directory permissions control access to the files inside the directory.

Example:

```bash
chmod 750 secure_directory
```

This allows:

* Owner: full access
* Group: read and execute
* Others: no access

The execute permission on directories allows users to enter and access contents.

---

## Summary

In this project, I:

* Viewed file and directory permissions using `ls -l`
* Interpreted Linux permission strings
* Modified permissions using `chmod`
* Secured both regular and hidden files
* Controlled directory access using permission settings

Understanding file permissions is essential for maintaining system security and enforcing access control in Linux environments.
