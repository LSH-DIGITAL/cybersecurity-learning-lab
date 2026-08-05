# IPv4 Address Structure

## What is IPv4?

IPv4 (Internet Protocol Version 4) is a logical addressing system used to identify devices on a network.

It works at:

OSI Layer 3 - Network Layer

Its purpose is to allow devices to communicate using source and destination addresses.

---

# IPv4 Format

An IPv4 address contains 32 bits.

Example:
192.168.1.25

It is divided into four sections called octets.

192       168       1        25
Octet 1   Octet 2   Octet 3  Octet 4

Each octet contains 8 bits.

Therefore:

8 bits + 8 bits + 8 bits + 8 bits = 32 bits

---

# Binary Representation

Computers understand binary.

Example:
192.168.1.25

is stored as:
11000000.10101000.00000001.00011001

Each octet can have values between:
0 - 255

because 8 bits can represent 256 possible values.

---

# Network Portion and Host Portion

Every IPv4 address has two important parts:

## Network Portion

Identifies the network.

Example:
192.168.1

## Host Portion

Identifies the specific device.

Example:
25

Complete address:
192.168.1.25

means:

Host number 25 inside network 192.168.1

---

# CIDR Prefix

CIDR tells us how much of the address belongs to the network.

Example:
192.168.1.25/24

The /24 means:
First 24 bits = Network
Last 8 bits = Host

A /24 network contains:
254 usable devices

---

# Why IPv4 Structure Matters in Cybersecurity

Security professionals use IPv4 knowledge for:

- Network reconnaissance
- IP range scanning
- Firewall configuration
- Traffic analysis
- Identifying internal networks
- Understanding attack surfaces

Example:

A penetration tester receives:
192.168.10.0/24

They understand:

The possible hosts are:
192.168.10.1 - 12.168.10.254
---

# Key Points

- IPv4 has 32 bits
- IPv4 contains 4 octets
- Each octet ranges from 0-255
- IP addresses contain network and host portions
- CIDR defines the network size
- IPv4 operates at OSI Layer 3




