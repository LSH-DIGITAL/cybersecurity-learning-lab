# Project 02: Linux Log Analysis

## Overview

This project focuses on understanding Linux log analysis and how security professionals use logs to investigate system activity.

Logs provide important evidence about events happening on a system. Security analysts use log analysis to detect suspicious activity, investigate incidents, and monitor system behavior.

In this project, I practiced creating and analyzing authentication-related log data using Linux command-line tools.

---

# Lab Environment

**Platform:**
- iSH Shell on iPad

**Operating System:**
- Alpine Linux

---

# Objectives

The objectives of this project were to:

- Understand the purpose of Linux logs
- Practice reading and analyzing log files
- Search log files for security-related information
- Identify failed and successful login attempts
- Learn basic security investigation techniques using Linux commands

---

# Linux Commands Practiced

```bash
uname
mkdir
cd
touch
echo
cat
grep
grep -c
head
tail
less
dmesg

---

# Common Linux Log Locations

| Location | Description |
|----------|-------------|
| `/var/log` | Stores most Linux log files |
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

✅ Completed

---

# Next Project

Project 03: Bash Scripting Fundamentals
