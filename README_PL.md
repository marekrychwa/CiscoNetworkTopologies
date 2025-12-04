# 🌐 Cisco Packet Tracer – Projekty topologii sieci komputerowych

Repozytorium zawiera dwa projekty topologii sieci lokalnych wykonane w środowisku **Cisco Packet Tracer**.  
Każda topologia prezentuje inny scenariusz budowy i konfiguracji sieci komputerowej LAN z wykorzystaniem routerów, przełączników, serwerów oraz urządzeń końcowych.  
Celem projektów było zaprojektowanie kompletnych i poprawnie działających sieci z możliwością komunikacji między wszystkimi podsieciami.

---

## 🧩 Topologia 1 – Sieć bezprzewodowa z dwoma routerami WRT300N

### 📘 Opis
Projekt przedstawia prostą sieć bezprzewodową składającą się z dwóch segmentów LAN połączonych centralnym przełącznikiem.  
Adresacja sieci została oparta o przestrzeń **192.168.0.0/16**, z podziałem na dwie podsieci:
- **192.168.10.0/24** – lewa sieć (Router2, Wireless LAN)
- **192.168.20.0/24** – prawa sieć (Router1, Wireless LAN)

Każdy router obsługuje swoją podsieć bezprzewodową (z laptopami) oraz lokalny serwer.  
Centralny **Switch0** umożliwia wymianę danych między podsieciami — sieć została przetestowana przy pomocy pakietów ICMP (`ping`), potwierdzając pełną komunikację między urządzeniami.

### ⚙️ Założenia techniczne
- 2× bezprzewodowe routery **WRT300N**
- 1× centralny przełącznik **Switch0**
- 3× serwery (Server0, Server1, Server2)
- 4× laptopy (Laptop1–Laptop4 + Laptop_ISP)
- Adresacja: 192.168.10.0/24, 192.168.20.0/24
- Sprawdzona komunikacja wewnątrz i między podsieciami (`ping OK`)

📸 Zrzut ekranu: `Topology_1/topology_1.png`  
🎬 Film instruktażowy: [Zobacz prezentację #1](https://drive.google.com/file/d/1Np0UIKW44WcqmhYY9ZkojYivAqXBz2at/view?usp=sharing)

---

## 🧩 Topologia 2 – Sieć przewodowa z trzema podsieciami

### 📘 Opis
Drugi projekt przedstawia kompletną sieć przewodową LAN złożoną z dwóch routerów połączonych łączem 10.10.10.0/24 oraz trzech podsieci końcowych:
- **172.16.100.0/24** – lewy segment sieci (Router R1, 2 komputery i serwer)
- **172.16.200.0/24** – środkowy segment (Router R2, 2 komputery i serwer)
- **192.168.10.0/24** – sieć bezprzewodowa (Wireless Router3, 2 laptopy i serwer)

Routery R1 i R2 realizują routing między podsieciami.  
Urządzenia końcowe uzyskały łączność w pełnym zakresie (potwierdzono testami ICMP).  
Dodatkowo zastosowano podział sieci na jasno zdefiniowane podsieci dla zwiększenia przejrzystości i bezpieczeństwa konfiguracji.

### ⚙️ Założenia techniczne
- 2× routery przewodowe (R1, R2)
- 2× przełączniki (Switch1, Switch2)
- 1× router bezprzewodowy (WRT300N)
- 3× serwery (Server1–Server3)
- 4× komputery (KO1–KO4) + 2× laptopy (LO1–LO2)
- Adresacja IP: 172.16.100.0/24, 172.16.200.0/24, 192.168.10.0/24
- Statyczne trasowanie i testy komunikacji między hostami

📸 Zrzut ekranu: `Topology_2/topology_2.png`  
🎬 Film instruktażowy: [Zobacz prezentację #2](https://drive.google.com/file/d/1EyfsUU76NR9eLgMC9X4Y8yPyD1pnZIb5/view?usp=sharing)

---

## ⚙️ Jak uruchomić projekty

1. Pobierz lub sklonuj repozytorium  
2. Otwórz wybrany plik `.pkt` w programie **Cisco Packet Tracer (7.2 lub nowszy)**  
3. Uruchom symulację i wykonaj testy komunikacji (`ping`)  
4. Możesz rozwinąć sieci, modyfikując adresację IP lub konfigurację routerów  

---

## 📋 Wymagania

- Cisco Packet Tracer 7.2 lub nowszy  
- System Windows / Linux z obsługą plików `.pkt`  
- (opcjonalnie) dostęp do Internetu dla odtwarzania filmów instruktażowych  

---

## 👨‍💻 Autor

**Marek Rychwa**  
Projekt zaliczeniowy z przedmiotu *Sieci komputerowe*  
📫 [marek.rychwa@gmail.com](mailto:marek.rychwa@gmail.com)  
🌐 [github.com/marekrychwa](https://github.com/marekrychwa) 
