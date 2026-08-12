# Linux Commands Practice

## 📌 Purpose

This document records some of the Linux commands I have practiced while developing my cybersecurity and IT support skills.

---

## 1. Checking the Current Directory

### Command

```bash
pwd
```

### Purpose

Displays the current working directory.

### Example

```text
/home/analyst
```

---

## 2. Listing Files

### Command

```bash
ls
```

### Purpose

Displays files and directories in the current location.

---

## 3. Changing Directories

### Command

```bash
cd
```

### Purpose

Used to navigate between directories.

### Example

```bash
cd /home/analyst
```

---

## 4. Reading Files

### Command

```bash
cat
```

### Purpose

Displays the contents of a file.

### Example

```bash
cat server_logs.txt
```

---

## 5. Searching for Information

### Command

```bash
grep
```

### Purpose

Searches text for a specific pattern or keyword.

### Example

```bash
grep "failed" server_logs.txt
```

This can be useful when looking for specific events in log files.

---

## 6. Using Pipes

### Example

```bash
cat server_logs.txt | grep "failed"
```

### Purpose

A pipe (`|`) sends the output of one command to another command.

This allows commands to be combined to filter and analyse information.

---

## 7. Viewing the First Lines of a File

### Command

```bash
head
```

### Example

```bash
head server_logs.txt
```

### Purpose

Displays the beginning of a file.

---

## 8. Changing File Permissions

### Command

```bash
chmod
```

### Example

```bash
chmod g+x projects
```

### Purpose

Changes permissions for files or directories.

Linux permissions help control who can read, write, or execute resources.

---

## 9. Creating a User

### Command

```bash
sudo useradd analyst2
```

### Purpose

Creates a new user account.

---

## 10. Modifying a User

### Command

```bash
sudo usermod
```

### Purpose

Modifies an existing user account.

---

## 11. Deleting a User

### Command

```bash
sudo userdel analyst2
```

### Purpose

Removes a user account.

---

## 12. Changing File Ownership

### Command

```bash
sudo chown analyst2 file.txt
```

### Purpose

Changes the owner of a file or directory.

---

# 🔐 Cybersecurity Relevance

These commands are useful for cybersecurity and IT support tasks such as:

* Investigating files
* Searching logs
* Checking permissions
* Managing user accounts
* Troubleshooting Linux systems
* Controlling access to resources
* Supporting security investigations

## 📚 What I Learned

Through these exercises, I gained practical experience with:

* Linux navigation
* File management
* Searching and filtering information
* File permissions
* User management
* File ownership
* Command-line investigation

This is part of my ongoing development toward an **IT Support and Cybersecurity career**.
