# BIOS vs UEFI – CompTIA A+ Core 1 Reference

Understand the differences, capabilities, and real-world relevance of BIOS and UEFI — essential for both hardware familiarity and exam success.

---

## 🧠 BIOS (Basic Input/Output System)

| Feature           | Description                                             |
|------------------|---------------------------------------------------------|
| Legacy firmware  | Used since the 1980s, very basic interface               |
| 16-bit software  | Limited device support, runs in real mode                |
| MBR partitioning | Max 2 TB drives, 4 primary partitions max                |
| Keyboard only    | No mouse support, text-only setup                        |
| Stored in ROM/Flash | Configurable via CMOS battery backup                |
| Boot speed       | Slower than UEFI                                        |

> **Common key to enter BIOS:** `DEL`, `F2`, or `F10` during POST

---

## 🚀 UEFI (Unified Extensible Firmware Interface)

| Feature             | Description                                                 |
|--------------------|-------------------------------------------------------------|
| Modern replacement | Graphical, user-friendly interface                          |
| 32-bit or 64-bit   | Supports larger and more complex drivers                    |
| GPT partitioning   | Supports drives over 2 TB and up to 128 partitions          |
| Secure Boot        | Prevents bootloader malware and rootkits                    |
| Mouse + Keyboard   | Full navigation support                                      |
| Fast Boot          | Reduces boot time significantly                             |

> **UEFI may also include a built-in shell for command-line configuration**

---

## 💾 MBR vs GPT (Partition Types)

| Feature      | MBR (BIOS)      | GPT (UEFI)         |
|--------------|-----------------|--------------------|
| Drive Size   | Max 2 TB        | Over 2 TB supported |
| Partition #  | 4 primary       | 128 partitions      |
| Compatibility | Widely supported | Modern OS only     |

---

## 🔄 Summary Table

| Feature          | BIOS                       | UEFI                        |
|------------------|----------------------------|-----------------------------|
| Interface        | Text-only                  | Graphical / CLI             |
| Boot Mode        | Legacy                     | Secure Boot, Fast Boot      |
| Partition Style  | MBR                        | GPT                         |
| Device Support   | Limited                    | Extensive                   |
| Drive Support    | ≤ 2 TB                     | > 2 TB                      |
| Input Devices    | Keyboard only              | Mouse + Keyboard            |

---

## 💡 Exam Tips

- UEFI is backward-compatible with BIOS mode (called “CSM” – Compatibility Support Module).
- BIOS settings are reset with **CMOS battery removal** or jumper reset.
- Secure Boot must often be disabled to install Linux or unsigned OS images.

---

> "BIOS walked so UEFI could sprint."  
> Know both — legacy lives on in the field.
