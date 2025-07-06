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

# CompTIA A+ Study Notes  
## BIOS/UEFI  
**Objective 3.4**

---

### BIOS and UEFI

#### • Basic Input/Output System (BIOS)
- Program that a CPU uses to start the computer system
- BIOS serves as a method of configuring the motherboard using a text-based interface

#### • Firmware
- Software on a chip and contains BIOS program code in the flash memory of a motherboard

#### • Unified Extensible Firmware Interface (UEFI)
- Supports 64-bit processors
- Provides a GUI

---

### Boot Options

#### • Basic Input/Output System (BIOS)
- Program a computer’s microprocessor uses to start and boot after being turned on
- BIOS is an example of firmware

**Boot features:**
- Power-on self-test (POST)
- Hardware configuration
- Boot order setup

---

### BIOS/UEFI Startup

- **ROM (Read-Only Memory)** is embedded in the motherboard and can be upgraded via flashing
- **CMOS** now uses a lithium-ion battery lasting up to 10 years
- **POST (Power-On Self Test)** checks input/output system on startup
- **Variable beeps** indicate system errors

**Common BIOS keys to enter configuration:**
`F2`, `DEL`, `ESC`, `F1`, `F10`, `F12`

- BIOS uses a text-based menu and keyboard
- UEFI allows both keyboard and mouse input with GUI
- UEFI supports 64-bit systems

---

### UEFI Features

- Supports larger HDDs/SSDs (up to 9.4 zettabytes)
- Supports GUID Partition Table (GPT)
- Faster boot-up
- Larger ROM

**Additional UEFI Options:**
- Disable booting from optical or USB drive
- Set boot priority (e.g. PXE network boot)

---

### Flashing
Performed for upgrades, fixes, or improvements:

1. Back up configuration and data
2. Use USB to flash firmware
3. BIOS/UEFI overwrites old code with the new

---

### BIOS/UEFI Security

- BIOS uses **MBR (Master Boot Record)**
- UEFI uses **GPT (GUID Partition Table)**

#### Supervisor/Admin/Setup Password
- Prevents unauthorized access to BIOS/UEFI config

#### User/System Password
- Locks access to the system

---

### TPM and HSM

#### • Hardware Root of Trust (RoT)
- Cryptographic module embedded in the system
- Ensures boot settings and verifies signatures

#### • TPM (Trusted Platform Module)
- Foundation of all secure computing ops
- Secured boot-up
- Provides encryption
- Can be managed via `tpm.msc` or Group Policy

#### • HSM (Hardware Security Module)
- Stores/generates cryptographic keys
- Less vulnerable to tampering or insider threats

---

### BIOS/UEFI Security Options

- **Storage/Hard Drive Password:** Prevents unauthorized drive access
- **Secure Boot:** UEFI-only setting that checks integrity of OS files
- **Rootkit Defense:** Protects from low-level malware
- Disable/enable USB ports to control access

---

### BIOS/UEFI Cooling Options

- BIOS/UEFI can configure **fan speed settings**

#### Modes:
- **Quiet mode:** Reduces fan speed and allows higher temperatures
- **Balanced mode:** Default setting
- **Cool mode:** Increases fan speed for airflow

- Overclocking generates more heat
- Temperature sensors monitor and adjust fan behavior:
  - Rising temp → Speed up
  - Below setpoint → Slow down or shut off

---
