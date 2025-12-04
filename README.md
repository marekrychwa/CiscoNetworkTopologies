# 🌐 Cisco Packet Tracer – Computer Network Topology Projects

[🇵🇱 Polish version](README_PL.md)

---

This repository contains two local area network (LAN) topology projects created in the **Cisco Packet Tracer** environment.  
Each topology presents a different scenario of building and configuring a computer LAN network using routers, switches, servers, and end devices.  
The goal of the projects was to design complete and properly functioning networks with the ability of communication between all subnets.

---

## 🧩 Topology 1 – Wireless network with two WRT300N routers

### 📘 Description
The project presents a simple wireless network consisting of two LAN segments connected by a central switch.  
The network addressing is based on the **192.168.0.0/16** space, divided into two subnets:
- **192.168.10.0/24** – left network (Router2, Wireless LAN)
- **192.168.20.0/24** – right network (Router1, Wireless LAN)

Each router supports its own wireless subnet (with laptops) and a local server.  
The central **Switch0** allows data exchange between subnets — the network was tested using ICMP packets (`ping`), confirming full communication between the devices.

### ⚙️ Technical assumptions
- 2× wireless routers **WRT300N**
- 1× central switch **Switch0**
- 3× servers (Server0, Server1, Server2)
- 4× laptops (Laptop1–Laptop4 + Laptop_ISP)
- Addressing: 192.168.10.0/24, 192.168.20.0/24
- Verified communication inside and between subnets (`ping OK`)

📸 Screenshot: `Topology_1/topology_1.png`  
🎬 Instructional video: [Watch presentation #1](https://drive.google.com/file/d/1Np0UIKW44WcqmhYY9ZkojYivAqXBz2at/view?usp=sharing)

---

## 🧩 Topology 2 – Wired network with three subnets

### 📘 Description
The second project presents a complete wired LAN consisting of two routers connected by a 10.10.10.0/24 link and three end subnets:
- **172.16.100.0/24** – left network segment (Router R1, 2 computers and a server)
- **172.16.200.0/24** – middle segment (Router R2, 2 computers and a server)
- **192.168.10.0/24** – wireless network (Wireless Router3, 2 laptops and a server)

Routers R1 and R2 perform routing between subnets.  
End devices obtained full connectivity (confirmed by ICMP tests).  
Additionally, the network was divided into clearly defined subnets to increase transparency and configuration security.

### ⚙️ Technical assumptions
- 2× wired routers (R1, R2)
- 2× switches (Switch1, Switch2)
- 1× wireless router (WRT300N)
- 3× servers (Server1–Server3)
- 4× computers (KO1–KO4) + 2× laptops (LO1–LO2)
- IP addressing: 172.16.100.0/24, 172.16.200.0/24, 192.168.10.0/24
- Static routing and connectivity tests between hosts

📸 Screenshot: `Topology_2/topology_2.png`  
🎬 Instructional video: [Watch presentation #2](https://drive.google.com/file/d/1EyfsUU76NR9eLgMC9X4Y8yPyD1pnZIb5/view?usp=sharing)

---

## ⚙️ How to run the projects

1. Download or clone the repository  
2. Open the selected `.pkt` file in **Cisco Packet Tracer (7.2 or newer)**  
3. Run the simulation and perform communication tests (`ping`)  
4. You can expand the networks by modifying IP addressing or router configuration  

---

## 📋 Requirements

- Cisco Packet Tracer 7.2 or newer  
- Windows / Linux system capable of handling `.pkt` files  
- (optional) Internet access for playing the instructional videos  

---

## 👨‍💻 Author

**Marek Rychwa**  
Course project for the subject *Computer Networks*  
📫 [marek.rychwa@gmail.com](mailto:marek.rychwa@gmail.com)  
🌐 [github.com/marekrychwa](https://github.com/marekrychwa)
