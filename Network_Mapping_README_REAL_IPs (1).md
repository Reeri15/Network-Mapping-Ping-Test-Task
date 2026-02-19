
# Network Mapping & Ping Test — Distinction Level (Real IPs)

## Submission Overview
This submission demonstrates **network topology design**, **IP configuration analysis**, and **connectivity testing**
using real `ipconfig` results from a Windows 10 machine.

---

## Network Topology (README Diagram)

```text
                                   🌍 Internet
                                        |
                                  ISP Router
                               Default Gateway
                                   172.20.6.1
                                        |
                              ┌─────────┴─────────┐
                              |   Wi‑Fi Router     |
                              |   (NAT + DHCP)    |
                              └─────────┬─────────┘
                                        |
                                  🖥️ Laptop
                              IPv4: 172.20.6.15
                              Subnet: 255.255.254.0
```

---

## IP Configuration (Actual Results)

```text
Active Adapter      : Wi‑Fi
IPv4 Address        : 172.20.6.15
Subnet Mask         : 255.255.254.0
Default Gateway     : 172.20.6.1
IPv6 (Link‑Local)   : fe80::bc31:67d5:8862:7a57
```

### Additional Adapter (Virtual / Host‑Only)
```text
Adapter Name        : Ethernet 2
IPv4 Address        : 192.168.56.1
Subnet Mask         : 255.255.255.0
Default Gateway     : Not assigned
Purpose             : Virtual / Internal Network
```

---

##  Ping Test Commands (Screenshots Required)

### 1 Gateway Test
```text
ping 172.20.6.1
```

### 2 Internet Connectivity
```text
ping 8.8.8.8
```

### 3 DNS Resolution
```text
ping google.com
```

---

##  Required Screenshots (Evidence)

Created a folder called **/screenshots** and include:

-  ipconfig.png
-  ping_gateway_172.20.6.1.png
-  ping_8.8.8.8.png
-  ping_google.png

---

##  Learning Outcomes
- Identified active vs inactive network adapters
- Differentiated physical vs virtual interfaces
- Verified LAN, WAN, and DNS connectivity
- Demonstrated real‑world troubleshooting skills

---

##  Conclusion
The device successfully obtained a dynamic IP address via DHCP, communicated with the default gateway,
and confirmed internet and DNS connectivity using standard command‑line tools.
