# IPv4 (Internet Protocol Version 4)

## Overview

IPv4 is a logical addressing system used to identify devices on a network.

It allows devices to communicate by providing source and destination addresses.

IPv4 operates at:

OSI Layer 3 - Network Layer

---

# IPv4 Address Structure

IPv4 addresses are 32 bits long.

They are divided into four octets:

Example:

192.168.1.25

192     168     1       25
Octet1  Octet2  Octet3  Octet4

Each octet contains 8 bits.

Total:

8 + 8 + 8 + 8 = 32 bits

Each octet range:

0 - 255

---

# Network Portion and Host Portion

An IPv4 address contains:

1. Network Portion
2. Host Portion

Example:

192.168.1.25/24

Network:
192.168.1

Host:
25

The subnet prefix determines where the network portion ends.

---

# CIDR Notation

CIDR represents the network prefix length.

Example:

192.168.1.0/24

/24 means:

First 24 bits = Network

Remaining 8 bits = Hosts

---

# Cybersecurity Importance

Understanding IPv4 helps security professionals:

- Identify network ranges
- Perform reconnaissance
- Understand firewall rules
- Analyze network traffic
- Configure security controls
