# 🧠 CompTIA A+ | Objective 3.2 — System Memory

## 🔹 System Memory Overview
- **RAM (Random Access Memory)**  
  - Volatile, non-permanent memory  
  - Temporarily stores data for fast access  
  - Used for loading apps, system files, and processes  

- **Addressing Memory**
  - **Cache**: High-speed memory (CPU access)
  - **Storage**: Slower but holds more data (e.g., HDD, SSD)
  - **Disk Cache**: Holds data temporarily to speed up disk access

- **Mass Storage Devices**  
  - Permanent storage (non-volatile)

---

## 🔹 Addressing and Architecture
- **Processor Access**
  - **x86 (32-bit)** → Max 4 GB RAM  
  - **x64 (64-bit)** → Supports more than 4 GB RAM (8, 16, 32, 64+ GB)

- **Memory Controllers**
  - **Single-Channel**: 64-bit data bus  
  - **Dual-Channel**: 128-bit data bus  
  - **Triple-Channel**: 192-bit data bus  
  - **Quad-Channel**: 256-bit data bus  
  - *Note: Use same model/speed/type for multi-channel systems*

---

## 🔹 Memory Modules
- **DIMM (Dual Inline Memory Module)**
  - Desktop memory  
  - 240 or 184-pin connector

- **SODIMM (Small Outline DIMM)**
  - Laptop memory  
  - Found in DDR3, DDR4, DDR5 formats

- **DDR Types (Double Data Rate)**
  - **DDR (PC133)** → 133 MHz  
  - **DDR2 (PC2-4200)** → 4.2 GB/s  
  - **DDR3 (PC3-10600)** → 10.6 GB/s  
    - Throughput: 6.4–17 GB/s  
    - Max: 8 GB per module

- **DRAM (Dynamic RAM)**  
  - Requires constant refreshing  
  - Oldest type

- **SDRAM (Synchronous DRAM)**  
  - Syncs with system bus  
  - Speeds: PC66, PC133, PC266

---

## 🔹 Memory Error Checking
- **Non-Parity Memory**
  - No error detection/correction

- **Parity Memory**
  - Basic error checking  
  - Uses parity bits (0 or 1)

- **ECC (Error Correcting Code)**
  - Detects & corrects errors  
  - Server-grade RAM  
  - Requires ECC-supported motherboard

- **Buffered / Registered Memory**
  - Additional hardware register between RAM & CPU  
  - Reduces electrical load  
  - Used in servers

---

## 🔹 Virtual Memory
- **Virtual Memory / Page File**
  - Space on HDD/SSD used when physical RAM is full  
  - OS allocates this to simulate memory

- **Page File / Swap Space**
  - Hidden system file that acts as overflow memory  
  - Slower than RAM but prevents crashes

---

## 🧪 Summary Table

| Type        | Pins | Speed/Bus       | Notes                         |
|-------------|------|------------------|-------------------------------|
| DDR         | 184  | PC1600+          | Obsolete                      |
| DDR2        | 240  | PC2-4200         | Higher latency                |
| DDR3        | 240  | PC3-10600        | 6.4–17 GB/s, 8GB max/module   |
| SODIMM      | —    | DDR3/DDR4/DDR5   | Laptop memory form factor     |
| ECC         | Varies | —              | Error correction, servers     |
| Buffered    | Varies | —              | Registers data for CPU        |

---

> 🧭 **Study Tip**: RAM types are a common test topic. Know pin count, voltage, speed, and differences between DDR versions. Use mnemonics and comparison tables.
