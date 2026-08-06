# Subnetting an IPv4 Network

## Overview

Subnetting is the process of dividing one large IPv4 network into smaller networks called subnets.

Subnetting is used to:

- Improve network security
- Reduce broadcast traffic
- Improve performance
- Organize devices
- Use IP addresses efficiently

---

# IPv4 Address Review

IPv4 addresses contain:

```
32 bits
```

Example:

```
192.168.1.25
```

An IPv4 address has two parts:

```
Network Portion + Host Portion
```

The subnet prefix determines where the network part ends.

---

# Prefix Length (/)

The prefix length shows the number of network bits.

Formula:

```
Network Bits + Host Bits = 32
```

Examples:

```
/24

Network bits = 24
Host bits = 8


/26

Network bits = 26
Host bits = 6
```

---

# Subnet Mask

A subnet mask identifies the network and host portions.

Example:

```
IP:
192.168.1.25

Prefix:
 /24

Subnet Mask:
255.255.255.0
```

Meaning:

```
192.168.1 | 25
 Network  | Host
```

---

# Borrowing Bits

Subnetting works by borrowing bits from the host portion.

Example:

Original:

```
/24
```

Binary:

```
11111111.11111111.11111111.00000000
```

Change to:

```
/26
```

Binary:

```
11111111.11111111.11111111.11000000
```

Two host bits were borrowed.

```
24 + 2 = 26
```

---

# Calculating Addresses

The number of host bits determines the number of addresses.

Formula:

```
Total Addresses = 2^Host Bits
```

Example:

```
/27
```

Host bits:

```
32 - 27 = 5
```

Calculation:

```
2⁵ = 32 addresses
```

Two addresses are reserved:

1. Network Address
2. Broadcast Address

Usable hosts:

```
32 - 2 = 30 hosts
```

---

# Common Subnet Sizes

| Prefix | Host Bits | Total Addresses | Usable Hosts |
|--------|-----------|----------------|--------------|
| /24 | 8 | 256 | 254 |
| /25 | 7 | 128 | 126 |
| /26 | 6 | 64 | 62 |
| /27 | 5 | 32 | 30 |
| /28 | 4 | 16 | 14 |
| /29 | 3 | 8 | 6 |
| /30 | 2 | 4 | 2 |

---

# Cybersecurity Importance

Subnetting is important for:

- Network reconnaissance
- Nmap scanning
- Firewall rules
- Network segmentation
- Attack surface analysis

Example:

```
nmap 192.168.1.0/24
```

This scans the entire subnet.

---

# Key Memory Rule

```
Prefix = Network size

Host bits = Number of devices
```

A larger prefix means:

```
More subnets
+
Fewer hosts per subnet
```
