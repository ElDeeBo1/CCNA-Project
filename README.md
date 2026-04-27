#  CCNA Enterprise Network Implementation

##  Project Overview
This project demonstrates a complete CCNA-level network implementation using Cisco Packet Tracer.  
It simulates a real-world enterprise network environment, covering core networking concepts such as switching, routing, network services, and security.

The project is designed to showcase practical skills in building, configuring, and securing a scalable network infrastructure.

---

##  Basic Configuration

###  Device Naming

**Switches**
- S1 → First Name  
- S2 → Second Name  
- S3 → Third Name  

**Routers**
- R1 → First Name  
- R2 → Second Name  
- R3 → Third Name  

- **Domain Name:** ITI.com  
- **Password Security:** Encrypted  
- **Remote Access:** SSH enabled (Telnet disabled)  

---

##  VLAN Configuration

- **SW1:** VLAN 10, 20, 30  
- **SW2:** VLAN 40, 50, 60  

- Ports assigned according to network design  
- **Spanning Tree Mode:** Rapid-PVST  

---

##  VLAN IP Addressing Scheme

| VLAN     | Network                |
|----------|-----------------------|
| VLAN 10  | 192.168.X.0/24        |
| VLAN 20  | 192.168.(X+1).0/24    |
| VLAN 30  | 192.168.(X+2).0/24    |
| VLAN 40  | 192.168.(X+3).0/24    |
| VLAN 50  | 192.168.(X+4).0/24    |
| VLAN 60  | 192.168.(X+5).0/24    |

---

##  DHCP Configuration

- Each VLAN uses a **/24 subnet**  
- **Default Gateway:** `.1` for each VLAN  
- **DNS Server:** `192.168.7.10`  
- Automatic IP assignment configured per VLAN  

---

##  Routing

- Dynamic routing using **OSPF**  
- Full communication between all VLANs  
- Default route configured between routers  

---

##  Network Security

- **AAA Authentication** using RADIUS server  
- **SSH** enabled for secure remote access  
- **Telnet disabled**  

---

##  Access Control Lists (ACLs)

- Block a specific host from accessing DNS server  
- Restrict VLAN 30 from accessing Web Server  
- Restrict VLAN 10 from accessing Mail Server  

---

##  Testing & Verification

- ✔️ Inter-VLAN connectivity (Ping test)  
- ✔️ DHCP IP assignment verification  
- ✔️ SSH remote access testing  
- ✔️ ACL validation  

---

##  Network Topology

<img width="1600" height="592" alt="image" src="https://github.com/user-attachments/assets/698eb9aa-8e46-4879-9823-1f6f77e18047" />


```md
