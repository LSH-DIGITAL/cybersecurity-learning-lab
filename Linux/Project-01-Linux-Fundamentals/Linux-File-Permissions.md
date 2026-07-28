# Linux File Permissions

## Overview

Linux file permissions determine who can read, write, or execute files and directories. Understanding permissions is essential because incorrect permissions can expose sensitive data or allow unauthorized access.

---

# Why File Permissions Matter

Proper file permissions help:

- Protect sensitive information
- Prevent unauthorized access
- Reduce security risks
- Improve system security

---

# Permission Types

There are three basic permissions:

## Read (r)

Allows a user to view the contents of a file or list a directory.

## Write (w)

Allows a user to modify a file or create and delete files inside a directory.

## Execute (x)

Allows a file to be executed as a program or script.

---

# Permission Groups

Permissions are assigned to three groups:

- Owner
- Group
- Others

Example:

```text
-rwxr-xr--
```

Meaning:

- Owner: Read, Write, Execute
- Group: Read, Execute
- Others: Read only

---

# Common Commands

## View Permissions

```bash
ls -l
```

Displays file permissions.

---

## Change Permissions

```bash
chmod 755 filename
```

Changes the permissions of a file.

---

## Change File Owner

```bash
chown username filename
```

Changes the owner of a file.

---

# Cybersecurity Importance

Attackers often look for files with weak permissions to gain unauthorized access.

Security professionals regularly review permissions to:

- Protect sensitive files
- Secure servers
- Prevent privilege escalation
- Reduce attack surfaces

---

# Best Practices

- Grant only the permissions that are necessary.
- Avoid giving write access to everyone.
- Review permissions regularly.
- Protect sensitive files with restrictive permissions.

---

# Summary

Understanding Linux file permissions is a fundamental cybersecurity skill. Proper permission management helps protect systems from unauthorized access and supports a secure operating environment.
