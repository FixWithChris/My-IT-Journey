# OSI vs TCP/IP Model – Networking Reference

Understand the differences, purpose, and layer functions of the OSI and TCP/IP models for troubleshooting and certification success.

---

## 🧱 OSI Model (7 Layers)

| Layer | Name              | Function Example                         |
|-------|-------------------|-------------------------------------------|
| 7     | Application        | Interfaces with the user (HTTP, SMTP)     |
| 6     | Presentation       | Encoding, encryption, compression (SSL, ASCII) |
| 5     | Session            | Establish/maintain communication sessions |
| 4     | Transport          | Reliable delivery, segmentation (TCP/UDP) |
| 3     | Network            | Routing & IP addressing (IP, ICMP)        |
| 2     | Data Link          | MAC addresses, frame delivery (Ethernet)  |
| 1     | Physical           | Cables, NICs, signal transmission         |

> **Mnemonic:** Please Do Not Throw Sausage Pizza Away  
(Physical → Application, bottom to top)

---

## 🌐 TCP/IP Model (4 Layers)

| Layer        | Corresponds to OSI           | Key Protocols                          |
|--------------|------------------------------|----------------------------------------|
| Application  | OSI 7, 6, 5                  | HTTP, HTTPS, FTP, DNS, SMTP            |
| Transport    | OSI 4                        | TCP, UDP                               |
| Internet     | OSI 3                        | IP, ICMP, ARP                          |
| Network Access | OSI 2 and 1                 | Ethernet, Wi-Fi, MAC addressing        |

---

## 🔁 Side-by-Side Comparison

| OSI Layer       | TCP/IP Layer       | Description                             |
|------------------|--------------------|-----------------------------------------|
| Application (7)  | Application         | Web, email, file transfer apps           |
| Presentation (6) | Application         | Data formatting (SSL, ASCII, JPEG)       |
| Session (5)      | Application         | Dialog control, connection management    |
| Transport (4)    | Transport           | Reliable/unreliable delivery (TCP/UDP)  |
| Network (3)      | Internet            | Logical addressing, routing (IP)        |
| Data Link (2)    | Network Access      | MAC addressing, framing (Ethernet)      |
| Physical (1)     | Network Access      | Wires, wireless signals, NICs           |

---

## 💡 When to Use Each

- **OSI Model:**
  - Great for teaching, conceptual breakdown
  - Helps identify *where* something failed

- **TCP/IP Model:**
  - Real-world implementation
  - More practical for live protocol reference

---

## 🧠 Exam Tips

- Know examples at each layer (e.g., TCP = Layer 4, IP = Layer 3).
- OSI is better for **troubleshooting questions**.
- TCP/IP is what we actually use on networks today.

---

> “TCP/IP is what we run. OSI is how we understand it.”
