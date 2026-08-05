# Types of IPv4 Addresses

## Overview

Not all IPv4 addresses have the same purpose. Different address types are used for communication on local networks, the Internet, device testing, and network management.

---

# 1. Public IP Address

A Public IP address is globally unique and reachable over the Internet.

Example:

```
8.8.8.8
```

Used for:

- Web servers
- Mail servers
- VPN gateways
- Internet communication

Cybersecurity:

Public IPs are the addresses visible to external users and are commonly assessed during external penetration tests.

---

# 2. Private IP Address

Private IP addresses are used inside local networks and are not directly routable on the Internet.

Private ranges:

```
10.0.0.0 – 10.255.255.255

172.16.0.0 – 172.31.255.255

192.168.0.0 – 192.168.255.255
```

Cybersecurity:

Internal penetration tests usually target private IP ranges.

---

# 3. Loopback Address

Loopback address:

```
127.0.0.1
```

Also known as:

```
localhost
```

Purpose:

Allows a computer to communicate with itself for testing and local services.

Cybersecurity:

Frequently used when testing local web servers, applications, and security tools.

---

# 4. APIPA (Automatic Private IP Addressing)

Range:

```
169.254.0.0/16
```

Purpose:

Automatically assigned when a device cannot obtain an IP address from a DHCP server.

Cybersecurity:

An APIPA address often indicates a network or DHCP problem.

---

# 5. Network Address

Example:

```
192.168.1.0/24
```

Purpose:

Identifies the entire network.

A network address cannot be assigned to a host.

---

# 6. Broadcast Address

Example:

```
192.168.1.255
```

Purpose:

Sends traffic to every device within the local network.

Routers normally do not forward broadcast traffic.

---

# 7. Default Gateway

Example:

```
192.168.1.1
```

Purpose:

Acts as the exit point that allows devices to communicate with other networks and the Internet.

Cybersecurity:

Gateways are critical network devices and are often protected by firewalls and access controls.

---

# 8. DNS Server

Purpose:

Translates domain names into IP addresses.

Example:

```
google.com
        ↓
142.x.x.x
```

Without DNS, users would need to remember IP addresses instead of domain names.

Cybersecurity:

Attackers may attempt DNS spoofing or poisoning to redirect users to malicious websites.

---

# Summary Table

| Address Type | Purpose |
|--------------|---------|
| Public | Internet communication |
| Private | Local network communication |
| Loopback | Communicate with the same device |
| APIPA | Self-assigned address when DHCP fails |
| Network | Identifies a network |
| Broadcast | Sends traffic to all devices on a LAN |
| Default Gateway | Connects to other networks |
| DNS Server | Converts domain names into IP addresses |

---

# Key Points

- Public IPs are reachable from the Internet.
- Private IPs are used inside local networks.
- 127.0.0.1 always refers to the local computer.
- APIPA addresses indicate DHCP failure.
- Network addresses identify networks.
- Broadcast addresses reach all devices on a LAN.
- The default gateway connects networks together.
- DNS converts names into IP addresses.
