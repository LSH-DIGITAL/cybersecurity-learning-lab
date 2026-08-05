# Network Segmentation

## Overview

Network segmentation is the practice of dividing a large network into smaller, isolated networks (segments). Each segment can have its own security policies, access controls, and traffic rules.

The goal is to improve security, performance, and network management.

---

# Why Network Segmentation?

Instead of placing every device in one large network, organizations divide the network into smaller sections.

Example:

```
                Company Network
                       │
        ┌──────────────┼──────────────┐
        │              │              │
       HR          Finance           IT
```

Each department has its own network segment.

---

# Benefits

## 1. Improved Security

If one network segment is compromised, attackers cannot automatically access every other segment.

Security devices such as firewalls and ACLs can restrict communication between segments.

---

## 2. Better Performance

Smaller broadcast domains reduce unnecessary network traffic.

This improves network efficiency and reduces congestion.

---

## 3. Easier Management

Different departments can have different security policies and access permissions.

Examples:

- HR
- Finance
- IT
- Guest Network

---

# Lateral Movement

Lateral movement occurs when an attacker gains access to one system and then attempts to move to other systems inside the organization.

Without segmentation:

```
HR → Finance → IT → Servers
```

With segmentation:

```
HR
 │
Firewall
 │
Finance
 │
Firewall
 │
IT
```

The attacker encounters additional security controls, making movement more difficult.

---

# Cybersecurity Importance

Network segmentation is a key defense strategy because it:

- Limits attacker movement
- Protects sensitive systems
- Reduces the impact of malware
- Improves incident containment
- Supports the Principle of Least Privilege

---

# Technologies Used for Segmentation

Examples include:

- VLANs
- Firewalls
- Access Control Lists (ACLs)
- DMZs
- Zero Trust Architecture
- Micro-segmentation

---

# Key Points

- Segmentation divides large networks into smaller sections.
- It improves security, performance, and management.
- It helps prevent lateral movement.
- It is widely used in enterprise environments.
