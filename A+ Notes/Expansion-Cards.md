# Expansion Cards – CompTIA A+ Core 1 Reference

Expansion cards are installed into motherboard slots (usually PCIe) to add or enhance system functionality. Know what each card does and when you'd install one.

---

## 🧩 Common Expansion Card Types

| Card Type         | Function                                          | Example Use Case                         |
|-------------------|---------------------------------------------------|------------------------------------------|
| **Video Card (GPU)** | Renders graphics; offloads work from CPU        | Gaming, 3D rendering, multiple monitors   |
| **Sound Card**     | Enhances audio input/output capabilities          | Music production, surround sound systems  |
| **Network Interface Card (NIC)** | Adds wired/wireless network access     | Wired LAN, Wi-Fi adapter, server NICs    |
| **Capture Card**   | Inputs video/audio from external sources          | Streaming gameplay, recording HDMI feed  |
| **TV Tuner Card**  | Receives over-the-air/cable TV signals            | Watching/recording broadcast TV          |
| **Storage Controller Card** | Adds or manages additional storage interfaces | RAID, SAS arrays                         |
| **Riser Card**     | Extends expansion slot access in small form factors | Horizontal GPU mount in small cases      |

---

## ⚙️ Slot Types

| Slot Type  | Description                      | Example Cards Used           |
|------------|----------------------------------|------------------------------|
| **PCIe x1** | Shortest, for low-bandwidth cards | NICs, sound cards            |
| **PCIe x16** | Longest, used for graphics cards | GPU, high-performance RAID   |
| **PCI**     | Legacy slot (largely phased out) | Old sound/NIC cards          |

> **Note:** PCIe slots are **not interchangeable by size**. A x16 card won’t fit in a x1 slot.

---

## 🔄 Installation Tips

- Always power down and unplug the system before installing.
- Install into compatible slot (check width and type).
- Secure card with a screw at the bracket.
- Install/update drivers after boot.

---

## 💡 Troubleshooting Expansion Cards

- **No output:** Reseat the card or try a different slot.
- **Missing driver:** Check Device Manager, update or reinstall.
- **Incompatibility:** Ensure BIOS/UEFI and OS support the card.
- **Power issues:** High-power cards (like GPUs) may require separate PSU connectors.

---

## 🧠 A+ Exam Tips

- You must recognize cards **by function and form**.
- Know which slots are used for which cards (especially PCIe x1 vs x16).
- Understand when to install an expansion card vs using onboard features.

---

> "The motherboard sets the tone — expansion cards let it sing."
