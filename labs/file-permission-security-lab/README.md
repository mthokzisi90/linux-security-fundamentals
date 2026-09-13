# Linux File Permissions Security Lab

## Overview

This safe, hands-on lab demonstrates how Linux file permissions protect sensitive information.

I created harmless fictional training files, reviewed their permissions, identified excessive read access on a fictional customer-data file, applied least-privilege permissions, and verified the remediation.

## Scenario

A routine security review identified that `customer_data.txt` had permissions of `644` (`-rw-r--r--`).

This allowed the owner to read and write the file, but also allowed group members and other users to read it. While this lab uses fictional data only, the same permission setting could expose sensitive customer information in a real environment.

## Tools Used

- Ubuntu Linux on WSL2
- Bash
- Visual Studio Code
- Linux commands: `ls -l` and `chmod`

## Investigation

The initial permission review showed:

```text
-rw------- audit_notes.txt
-rw-r--r-- customer_data.txt
-rw-r--r-- public_readme.txt
```

### Finding

`customer_data.txt` was marked as sensitive training data but had permission `644`.

This was identified as a security concern because users other than the file owner could read the file.

## Remediation

I applied the following least-privilege permission:

```bash
chmod 600 customer_data.txt
```

The permission was then verified:

```text
-rw------- customer_data.txt
```

The corrected setting allows only the file owner to read and write the sensitive file.

## Security Concepts Demonstrated

- Linux file permissions
- Read, write, and execute access
- File ownership
- Least privilege
- Confidentiality
- Security auditing
- Remediation and verification

## Evidence

Screenshots in `evidence/screenshots/` show the permission review before remediation and the successful corrected permissions after remediation.

## Disclaimer

This is an educational cybersecurity project using only fictional training files. No real user data, systems, or sensitive information was accessed or modified.

**Author:** Mthokozisi Khulu  
**GitHub:** [@mthokzisi90](https://github.com/mthokzisi90)