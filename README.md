# 🐧 Linux Security Fundamentals

## 📌 Overview

This repository documents my **hands-on Linux and cybersecurity learning**, including command-line exercises, file permissions, user and group management, ownership, access control, and security-focused practical labs.

I created this project as part of my cybersecurity learning journey to develop practical skills relevant to entry-level **IT Support, Technical Support, Cybersecurity, and Security Operations** roles.

The repository includes practical exercises, security documentation, screenshots, and audit evidence demonstrating how Linux administration concepts can be applied to basic security tasks.

---

## 🎯 Learning Objectives

Through this project, I am developing the ability to:

* Navigate the Linux file system using the command line
* Search and analyse files
* Investigate files and system information
* Understand Linux file and directory permissions
* Manage users and groups
* Modify file ownership and permissions
* Apply the principle of least privilege
* Use command-line tools for basic security investigation
* Document security findings and remediation
* Use Git and GitHub for security project documentation

---

## 💻 Linux Commands Practiced

### File and Directory Navigation

```bash
pwd
ls
cd
```

### Working With Files

```bash
cat
head
echo
```

### Searching and Filtering

```bash
grep
```

### Command Piping

```bash
command1 | command2
```

### File Permissions

```bash
chmod
```

### User Management

```bash
useradd
usermod
userdel
```

### File Ownership

```bash
chown
```

### Permission and Access Auditing

```bash
stat
getfacl
setfacl
```

These commands were used to inspect and manage Linux permissions and access controls during practical exercises.

---

## 🔐 Security Concepts

### File Permissions

Linux uses permissions to control who can read, write, or execute files and directories.

The three main permission categories are:

* **Owner**
* **Group**
* **Others**

The main permissions are:

* `r` — Read
* `w` — Write
* `x` — Execute

For example:

```text
-rwxr-xr--
```

This represents different levels of access for the owner, group, and other users.

Understanding these permissions is important when protecting sensitive files and applying the **principle of least privilege**.

### User and Group Management

Linux user-management commands can be used to create, modify, and remove user accounts.

Examples include:

```bash
sudo useradd username
sudo usermod -aG groupname username
sudo userdel username
```

Proper user and group management helps control access to systems and resources.

### Access Control Lists

I also practiced working with Linux Access Control Lists (ACLs) to provide more granular access permissions when standard owner/group/other permissions are not sufficient.

Example commands include:

```bash
getfacl filename
setfacl -m group:security:r-- filename
```

---

## 🔎 Practical Security Lab

### File Permission Security Lab

The repository includes a practical **File Permission Security Lab** demonstrating the investigation and remediation of Linux file-access permissions.

The lab includes:

* Permission investigation
* Security risk identification
* Permission remediation
* ACL concepts
* Permission auditing
* Audit documentation
* Before-and-after screenshots
* Security findings and recommendations

### 📂 Lab Contents

```text
labs/
└── file-permission-security-lab/
    ├── README.md
    ├── permission-audit-report.md
    │
    ├── evidence/
    │   └── screenshots/
    │       ├── 01-before-remediation.png
    │       ├── 02-after-remediation.png
    │       └── 03-permission-audit-report.png
    │
    └── lab-data/
        ├── audit_notes.txt
        ├── customer_data.txt
        └── public_readme.txt
```

The screenshots provide visual evidence of the permissions before and after remediation, while the audit report documents the security analysis and findings.

---

## 🛡️ Cybersecurity Relevance

Linux is widely used across IT infrastructure, servers, cloud environments, and cybersecurity operations.

Understanding Linux command-line tools supports tasks such as:

* Investigating system activity
* Reviewing files and logs
* Checking file permissions
* Managing user access
* Troubleshooting systems
* Supporting security investigations
* Applying least-privilege principles
* Performing basic security auditing
* Documenting security findings

These skills provide a foundation for roles involving **IT support, technical support, system administration, security operations, and cybersecurity**.

---

## 📚 What I Learned

This project helped me strengthen my understanding of:

* Linux command-line navigation
* File and directory management
* Linux permissions
* User and group management
* File ownership
* Access Control Lists (ACLs)
* Basic security administration
* Security auditing
* The principle of least privilege
* Command-line investigation techniques
* Security documentation
* Git and GitHub

---

## 🚀 Future Improvements

I plan to continue expanding this repository with:

* Linux log-analysis exercises
* Bash scripting
* Security automation
* Additional Linux security commands
* Practical troubleshooting scenarios
* Authentication and access-control labs
* Security monitoring exercises
* Additional cybersecurity projects

---

## 🎯 Career Relevance

The skills demonstrated in this repository are relevant to entry-level **IT Support, Technical Support, Cybersecurity, and Security Operations** roles.

This project demonstrates my ability to work with Linux command-line tools, investigate files and system information, manage users and permissions, apply access-control principles, perform basic security auditing, and document security findings.

**Author:** Mthokozisi Khulu
**GitHub:** [@mthokzisi90](https://github.com/mthokzisi90)
----------------------------------------------------------

## ⭐ Portfolio

I am building a practical cybersecurity portfolio focused on developing hands-on skills through security labs, documentation, and real-world security scenarios.

**Current focus:** Linux Security • IT Support • Cybersecurity Fundamentals • Security Operations

⭐ This repository documents my ongoing journey into IT Support and Cybersecurity.
