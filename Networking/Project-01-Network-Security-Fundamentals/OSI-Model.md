# OSI Model

## Overview

The OSI (Open Systems Interconnection) model is a conceptual framework that explains how data moves through a network. It divides network communication into seven layers, helping security professionals understand where problems and attacks can occur.

## The 7 Layers

### Layer 7: Application
Provides network services directly to users.

Examples:
- HTTP
- HTTPS
- DNS
- FTP

Security concerns:
- Web attacks
- Phishing
- Application vulnerabilities

---

### Layer 6: Presentation
Handles data formatting, encryption, and compression.

Security concerns:
- Encryption weaknesses
- Data exposure

---

### Layer 5: Session
Manages communication sessions between applications.

Security concerns:
- Session hijacking

---

### Layer 4: Transport
Provides reliable data transfer.

Protocols:
- TCP
- UDP

Security concerns:
- Port scanning
- DoS attacks

---

### Layer 3: Network
Handles logical addressing and routing.

Examples:
- IP addresses
- Routers

Security concerns:
- IP spoofing
- Routing attacks

---

### Layer 2: Data Link
Handles communication between devices on the same network.

Examples:
- MAC addresses
- Switches

Security concerns:
- MAC spoofing
- ARP attacks

---

### Layer 1: Physical
The actual hardware transmission layer.

Examples:
- Cables
- Radio signals

Security concerns:
- Physical access attacks

---

## Cybersecurity Importance

Understanding the OSI model helps security professionals identify:
- Where attacks happen
- Which tools to use
- How to troubleshoot security issues
