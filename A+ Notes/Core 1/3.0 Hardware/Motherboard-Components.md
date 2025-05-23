# Motherboard Components – CompTIA A+ Reference

A quick reference guide to key motherboard components, form factors, and connection types for the A+ Core 1 exam.

---

## 🧠 Core Components

| Component           | Description                                                      |
|---------------------|------------------------------------------------------------------|
| **CPU Socket**       | Connects the processor to the board (Intel: LGA, AMD: PGA/AM4)   |
| **Chipset**          | Manages communication between CPU, RAM, storage, and peripherals |
| **Northbridge**      | Handles high-speed communication (older boards; now integrated)  |
| **Southbridge**      | Manages I/O like USB, SATA, audio, legacy ports                  |
| **RAM Slots (DIMMs)**| Install memory modules (DDR3, DDR4, DDR5 depending on board)     |
| **PCIe Slots**       | Add-in cards: GPU, NIC, capture cards                            |
| **Power Connectors** | 24-pin ATX (motherboard) + 4/8-pin CPU power                    |
| **SATA Connectors**  | Storage devices: HDDs, SSDs, optical drives                      |
| **M.2 Slot**         | High-speed storage via NVMe or SATA                              |
| **Front Panel Header**| Connect power button, reset switch, LEDs                       |
| **CMOS Battery**     | Powers BIOS firmware settings (typically a CR2032 coin cell)     |
| **Fan Headers**      | For system cooling and CPU fans                                  |

---

## 🧰 Internal Connectors

- **SATA Ports** – Used for hard drives and optical drives
- **NVMe/M.2 Slot** – Used for solid-state drives with PCIe speed
- **Front Panel Connectors** – Connect case’s buttons and LEDs

---

## 🔌 External Connectors (Rear I/O)

| Port Type      | Use Case                     |
|----------------|------------------------------|
| USB (2.0/3.0/C)| Keyboard, mouse, drives      |
| HDMI / DisplayPort | Video output             |
| Ethernet (RJ-45) | Networking                 |
| Audio Jacks    | Mic, speakers, line-in       |
| PS/2           | Legacy mouse/keyboard        |
| VGA / DVI      | Legacy video output          |

---

## 🧱 Form Factors

| Form Factor | Size (inches)     | Notes                                 |
|-------------|-------------------|---------------------------------------|
| ATX         | 12 x 9.6          | Full-sized, max expansion             |
| MicroATX    | 9.6 x 9.6         | Fewer slots, fits smaller cases       |
| Mini-ITX    | 6.7 x 6.7         | Ultra-compact, limited expandability  |

> **Tip:** ATX and microATX share the same mounting holes — microATX fits in ATX cases.

---

## 🔄 BIOS vs UEFI

| BIOS         | UEFI                          |
|--------------|-------------------------------|
| Legacy firmware | Modern interface, graphical |
| MBR support only | GPT support (larger drives) |
| Up to 2 TB drives | Over 2 TB supported        |

> **CMOS battery** maintains BIOS settings when power is off.

---

## 💡 Exam Tips

- Know which connectors attach to **power**, **storage**, and **expansion**.
- Understand form factor differences (especially ATX vs microATX).
- Be able to identify major motherboard components visually.

---

**“The board doesn’t just hold the system — it *is* the system.”**
