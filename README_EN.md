# 🌐 Cisco Packet Tracer – Computer Network Topology Projects

This repository contains two local area network (LAN) topology projects created in **Cisco Packet Tracer** as part of the *Computer Networks* course.  
Each topology represents a different configuration scenario of a local network built with routers, switches, servers, and end devices.  
The goal was to design fully functional networks with complete communication between all subnets.

---

## 🧩 Topology 1 – Wireless network with two WRT300N routers

### 📘 Overview
This project shows a simple wireless network composed of two LAN segments connected through a central switch.  
The network uses the **192.168.0.0/16** address space divided into subnets:
- **192.168.10.0/24** – left subnet (Router2, Wireless LAN)
- **192.168.20.0/24** – right subnet (Router1, Wireless LAN)

Each wireless router (WRT300N) manages its own laptop subnet and a local server.  
The central **Switch0** handles traffic between the segments.  
Connectivity was verified using ICMP (`ping`), confirming full communication between all devices.

### ⚙️ Technical details
- 2× wireless routers (**WRT300N**)  
- 1× central switch (**Switch0**)  
- 3× servers (Server0, Server1, Server2)  
- 4× laptops (Laptop1–Laptop4 + Laptop_ISP)  
- IP addressing: 192.168.10.0/24, 192.168.20.0/24  
- Successful communication between all subnets (`ping OK`)

📸 Screenshot: `Topology_1/topology_1.png`  
🎬 Instructional video: [Watch presentation #1](https://drive.google.com/file/d/1Np0UIKW44WcqmhYY9ZkojYivAqXBz2at/view?usp=sharing)

---

## 🧩 Topology 2 – Wired network with three subnets

### 📘 Overview
The second project represents a fully wired LAN using two routers connected over the **10.10.10.0/24** link and three end subnets:
- **172.16.100.0/24** – left network (Router R1, two PCs and Server1)  
- **172.16.200.0/24** – middle network (Router R2, two PCs and Server2)  
- **192.168.10.0/24** – wireless network (Wireless Router3, two laptops and Server3)

Routers **R1** and **R2** handle static routing between subnets.  
All end devices have full connectivity verified through ICMP echo tests.  
The design improves clarity and security through clearly separated IP address spaces.

### ⚙️ Technical details
- 2× wired routers (R1, R2)  
- 2× switches (Switch1, Switch2)  
- 1× wireless router (WRT300N)  
- 3× servers (Server1–Server3)  
- 4× PCs (KO1–KO4) and 2× laptops (LO1–LO2)  
- IP addressing: 172.16.100.0/24, 172.16.200.0/24, 192.168.10.0/24  
- Static routing and connectivity successfully verified (ICMP ping)

📸 Screenshot: `Topology_2/topology_2.png`  
🎬 Instructional video: [Watch presentation #2](https://drive.google.com/file/d/1EyfsUU76NR9eLgMC9X4Y8yPyD1pnZIb5/view?usp=sharing)

---

## ⚙️ How to open the projects

1. Download or clone this repository  
2. Open `.pkt` files using **Cisco Packet Tracer (version 7.2 or newer)**  
3. Run the simulation and test connectivity using `ping` commands  
4. Optionally, expand the networks or modify IP addressing for practice  

---

## 📋 Requirements

- Cisco Packet Tracer 7.2 or newer  
- Windows or Linux system capable of running `.pkt` files  
- (optional) Internet access – required for viewing video presentations  

---

## 👨‍💻 Author

**Marek Rychwa**  
Course project – *Computer Networks*  
📫 [marek.rychwa@gmail.com](mailto:marek.rychwa@gmail.com)  
🌐 [github.com/marekrychwa](https://github.com/marekrychwa) 
