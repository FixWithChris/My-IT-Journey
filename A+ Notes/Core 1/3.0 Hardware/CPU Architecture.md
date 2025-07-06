# 🧠 CPU Architecture

## CPU
- The brains of the computer that execute the different programming codes in the software and firmware
- Performs the basic operations for every instruction in the computer
- Once execution is complete, sends information back to memory for storage or reuse

## X86
- Supports a maximum of **4 GB of RAM**

## X64
- Extension of the X86 instruction set that supports **64-bit operations**
- 32-bit systems can only run 32-bit programs
- 64-bit processors can run both **64-bit and 32-bit programs** (fully backwards compatible)

## ARM (Advanced RISC Machine)
- Used in **low-power devices** like tablets and phones
- Optimized for:
  - Extended battery life
  - Lower heat output
- Uses **RISC (Reduced Instruction Set Computing)** architecture

---

# 🔌 CPU Sockets

## ZIF (Zero Insertion Force)
- Allows insertion of CPU without pressing or applying force
- If you **bend, snap, or break a pin**, the processor may become unusable

## LGA (Land Grid Array)
- All pins are on the socket, not the CPU
- **Used by Intel**

## PGA (Pin Grid Array)
- CPU has pins, socket has holes for alignment
- **Used by AMD**

## Multi-Socket
- Multiple CPUs or processors installed on one motherboard
- Mobile devices **cannot** be upgraded or have CPUs replaced
- Two main types:
  - **LGA** – Intel
  - **PGA** – AMD

---

# ⚙️ CPU Features

## Simultaneous Multithreading (SMT) / Hyper-threading
- A single stream of instructions can be sent by software to a processor
- Allows software to run **multiple parallel threads** at once

## Symmetric Multiprocessing (SMP)
- Traditional workstations and servers with **multiple processors**

---

# 🧩 Multi-core CPUs

- **Multi-core Processor**: One CPU with multiple cores inside
- **Dual-core**: Two CPUs inside a single chip
- **Quad-core**: Four CPUs inside a single chip
- **Hexa-core**: Six CPUs inside a single chip
- **Octa-core**: Eight CPUs inside a single chip

---

# 🧪 Virtualization Support

- **Hyper-threading / SMT**
- **SMP**
- **Multi-core processing**
- **Virtualization**: Allows multiple systems to run on one host

### Virtualization Extensions

#### Intel
- **EPT** – Extended Page Table

#### AMD
- **RVI** – Rapid Virtualization Indexing

### SLAT (Second Level Address Translation)
- Hardware-level support for software virtualization

---

# 🛠️ Installing the Motherboard & CPU

1. Review the motherboard’s documentation
2. Place the motherboard aligned at the rear of the case
3. Insert standoffs that match the holes in the motherboard
4. Install the processor and memory modules before securing the board
5. Verify standoffs are properly aligned
6. Secure standoffs using the correct screw type
7. Install the power supply, drives, and add-on cards
