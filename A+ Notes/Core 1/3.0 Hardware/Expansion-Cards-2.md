# 🧠 CompTIA A+ – Expansion Cards & Bus Architectures

## PCI (Peripheral Component Interconnect)
- 32-bit expansion card
  - PCI 32-bit cards support only a max bus speed of **33 MHz** or **133 MBps**

## PCI-X
- 64-bit expansion card
  - Operates at **133 MHz**

## PCI-X 2.0
- Operates at **266 MHz up to 533 MHz**
- **Used for** networking and audio cards

---

## AGP (Accelerated Graphics Port)
- Used for **video graphics cards**
  - AGP 1x  
  - AGP 2x  
  - AGP 4x  
  - AGP 8x

---

## PCIe (PCI Express)
- **Replaces** PCI, PCI-X, and AGP
- Lane types:
  - `PCIe x1`
  - `PCIe x4`
  - `PCIe x8`
  - `PCIe x16`
- **Common uses**:
  - `x1`: Modems, network cards, wireless cards, input/output devices, audio cards
  - `x16`: Graphics cards

---

## PCIe Bus Architecture
- Connects external devices to the motherboard
- Number of lanes:  
  - 16, 24, or 32 PCIe lanes (determined by motherboard/form factor)

### PCIe Versions
- PCIe 1.0  
- PCIe 2.0  
- PCIe 3.0  
- PCIe 4.0  
- PCIe 5.0

### Power Ratings
- All PCIe slots: **25W**
- PCIe x16 card slot: **Up to 75W**

### Plugging Terms
- **Up-plugging**: Putting smaller card in a larger slot  
- **Down-plugging**: Putting larger card in a smaller slot

---

## Mini PCIe
- Smaller version of a standard PCIe card
- **Used in laptops**, especially for:
  - Modems
  - Networking cards
  - Wireless cards
  - Audio cards

---

# 🔧 Expansion Card Types

## Video Card / Graphics Adapter
- Sends quality signals to monitors

## Graphics Processing Unit (GPU)
- Specialized processor for graphics rendering acceleration

## High Speed Memory
- Embeds memory on card to offload system memory usage

## Graphical Ports
- External ports: **Thunderbolt, DisplayPort, HDMI**

## Video Capture Card
- Takes in and processes video signals
- Used for:
  - Video recording
  - Security footage

## TV Capture Card
- Connects to cable TV systems via coax cables

## Sound / Audio Card
- Improves audio output
- Example: **RJ45 Port – 1 Gbps**

---

## Riser Card
- A special expansion card installed on a motherboard
- Example: Install NIC into PCIe x1 slot (10 Gbps)
  - Uses **ST / SC / MT-RJ connectors** for fiber
