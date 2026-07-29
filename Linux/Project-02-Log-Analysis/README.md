 # Project 02: Linux Log Analysis

## Overview

This project focuses on understanding Linux log files and how they are used to monitor systems, troubleshoot issues, and investigate security events.

Log analysis is one of the most important skills in cybersecurity because logs provide evidence of what has happened on a system. Security analysts use logs to detect suspicious activity, investigate incidents, and identify security issues.

---

# Lab Environment

**Platform:**
- iSH Shell (Alpine Linux)
- Ubuntu Playground (Killercoda)

**Operating Systems:**
- Alpine Linux
- Ubuntu Linux

---

# Objectives

The objectives of this project are to:

- Understand what Linux log files are
- Learn the purpose of different log files
- Read log files using Linux commands
- Search logs for useful information
- Understand how logs support cybersecurity investigations

---

# Linux Commands Practiced

```bash
cat
less
head
tail
grep
dmesg
```

---

# Common Linux Log Locations

| Location | Description |
|----------|-------------|
| `/var/log` | Stores most Linux log files |
| `/var/log/messages` | General system messages (varies by distribution) |
| `/var/log/auth.log` | Authentication and login activity (Ubuntu/Debian) |
| `/var/log/secure` | Authentication logs (RHEL/CentOS) |
| `/var/log/syslog` | General system log (Ubuntu/Debian) |
| `/var/log/dmesg` | Kernel boot messages |

---

# Tasks Completed

## Viewing Available Log Files

```bash
ls /var/log
```

Purpose:

Displays the available log files stored on the system.

---

## Viewing System Information

```bash
cat /etc/os-release
```

Purpose:

Displays operating system information.

---

## Viewing Kernel Messages

```bash
dmesg | head
```

Purpose:

Displays the first few kernel messages generated during system startup.

---

## Searching Logs

```bash
grep
```

Purpose:

Searches for keywords inside log files.

---

# Cybersecurity Importance

Log analysis is essential because security professionals use logs to:

- Detect suspicious activity
- Investigate security incidents
- Monitor system health
- Identify failed login attempts
- Troubleshoot system problems
- Support digital forensic investigations

---

# Skills Developed

Through this project, I practiced:

- Linux log analysis
- Reading system information
- Understanding log file locations
- Searching text using Linux commands
- Basic security investigation techniques

---

# Learning Outcome

After completing this project, I understand the purpose of Linux log files and how they help security professionals monitor systems and investigate security events.

This knowledge provides a strong foundation for future topics such as incident response, security operations, digital forensics, and penetration testing.

---

# Status

🚧 In Progress

---

# Next Project

Project 03: Bash Scripting Fundamentals
