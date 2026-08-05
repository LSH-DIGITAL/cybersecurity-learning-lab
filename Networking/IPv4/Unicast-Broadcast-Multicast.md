# IPv4 Unicast, Broadcast, and Multicast

## Overview

IPv4 devices communicate using three primary communication methods:

- Unicast
- Broadcast
- Multicast

Each method determines how packets are delivered across a network.

---

# 1. Unicast

## Definition

Unicast is one-to-one communication.

One sender communicates with one receiver.

Example:

```
Computer A ─────────► Computer B
```

Examples:

- Opening a website
- SSH connection
- Email
- File transfer

### Cybersecurity

Most penetration testing activities use unicast communication, including:

- Nmap scans
- SSH
- HTTP/HTTPS requests
- Remote administration

---

# 2. Broadcast

## Definition

Broadcast is one-to-all communication within the same local network.

One device sends a packet that every device on the LAN receives.

Example:

```
           Computer B
              ▲
              │
Computer A ───┼────► Everyone
              │
              ▼
           Computer C
```

Example Uses

- ARP Requests
- Device discovery
- DHCP Discover messages

### Cybersecurity

Broadcast traffic can help devices discover each other.

Excessive broadcast traffic may indicate:

- Network misconfiguration
- Broadcast storms
- Certain denial-of-service attacks

Routers normally do not forward broadcast traffic between networks.

---

# 3. Multicast

## Definition

Multicast is one-to-many communication.

Packets are delivered only to devices that have joined a multicast group.

Example:

```
Server
   │
   ├────────► Client A
   ├────────► Client B
   └────────► Client C
```

Devices that are not members of the group do not receive the traffic.

Example Uses

- Live video streaming
- IPTV
- Video conferencing
- Routing protocols

### Cybersecurity

Multicast reduces unnecessary network traffic by sending data only to subscribed devices.

Security professionals may encounter multicast traffic when analyzing enterprise networks.

---

# Comparison

| Communication Type | Delivery | Example |
|--------------------|----------|---------|
| Unicast | One to One | Web browsing |
| Broadcast | One to All | ARP Request |
| Multicast | One to Many | Live video streaming |

---

# Key Points

- Unicast is the most common communication type.
- Broadcast reaches every device on the local network.
- Multicast reaches only subscribed devices.
- Routers normally block broadcast traffic from crossing network boundaries.
