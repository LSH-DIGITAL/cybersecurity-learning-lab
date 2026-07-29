# Project 03: Bash Scripting Fundamentals

## Overview

This project focuses on learning the fundamentals of Linux shell scripting using the iSH Shell environment.

Bash scripting allows security professionals to automate repetitive tasks, collect system information, analyze files, and create simple security tools.

The goal of this project was to understand how Linux commands can be combined into scripts for automation.

---

# Lab Environment

**Platform:**
- iSH Shell on iPad

**Operating System:**
- Alpine Linux

---

# Objectives

The objectives of this project were:

- Understand basic shell scripting
- Create and execute scripts
- Learn variables and user input
- Use conditional statements
- Use loops for automation
- Create basic cybersecurity automation scripts

---

# Concepts Practiced

## 1. Creating Shell Scripts

Learned how to create `.sh` files and execute them.

Example:

```sh
hello.sh
```

Used:

```sh
chmod +x filename.sh
```

to make scripts executable.

---

# 2. Shebang

Learned the purpose of the first line in a script:

```sh
#!/bin/ash
```

The shebang tells Linux which interpreter should run the script.

Because iSH uses Alpine Linux, `/bin/ash` was used.

---

# 3. Variables

Created variables to store information.

Example:

```sh
name="Cybersecurity"
```

Used variables with:

```sh
echo $name
```

---

# 4. User Input

Learned how scripts can receive information from users.

Command:

```sh
read
```

Example:

- Ask user for information
- Store the input
- Use it inside the script

---

# 5. Conditional Statements

Used:

```sh
if
then
else
fi
```

Created a file checking script.

The script checks whether a file exists and displays the result.

---

# 6. Loops

Learned how to repeat actions automatically.

Used:

```sh
for
```

Example:

Searching multiple files automatically.

---

# Scripts Created

## Hello World Script

Purpose:

- Test script execution
- Understand executable permissions

---

## Variables Script

Purpose:

- Practice storing and displaying information

---

## File Checker Script

Purpose:

- Check whether a file exists

Cybersecurity relevance:

File checking is useful when investigating suspicious files.

---

## System Information Collector

Collected:

- Current user
- Hostname
- Operating system information
- Current directory

Commands used:

```sh
whoami
hostname
cat /etc/os-release
pwd
```

---

## Log Scanner Script

Created a simple security analysis script.

Functions:

- Accept a log file name
- Check if the file exists
- Count failed login attempts

Command used:

```sh
grep -c "Failed"
```

Cybersecurity relevance:

Similar techniques are used by security analysts during log investigations.

---

# Skills Developed

Through this project, I practiced:

- Linux shell scripting
- Automation basics
- File handling
- User interaction
- Security-focused scripting
- Command-line troubleshooting

---

# Learning Outcome

After completing this project, I understand how Linux commands can be combined into scripts to automate tasks.

These fundamentals will support future cybersecurity topics such as:

- Security automation
- SOC operations
- Incident response
- Penetration testing

---

# Status

✅ In Progress
