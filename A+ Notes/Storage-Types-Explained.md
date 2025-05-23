# Storage Types Explained

Quick-reference guide to the different storage technologies you need to know for the CompTIA A+ Core 1 exam.

---

## 1. **Magnetic Drives (HDDs)**

- **How it works:** Spinning platters + read/write heads
- **Pros:** 
  - High capacity (up to 10+ TB)
  - Cost-effective per GB
- **Cons:** 
  - Slower speeds
  - Susceptible to shock damage

> Used for: Bulk storage, archival, backup drives

---

## 2. **Solid State Drives (SSD)**

- **How it works:** Flash memory, no moving parts
- **Pros:** 
  - Extremely fast read/write speeds
  - Lower power consumption
  - Shock resistant
- **Cons:**
  - Higher cost per GB

> Used for: Operating systems, frequently accessed applications

---

## 3. **M.2 Drives**

- **Form factor:** Small and rectangular (no cables)
- **Can use:**
  - SATA (slower)
  - NVMe via PCIe lanes (faster)
- **Speed comparison:**
  - SATA M.2 ≈ 600 MB/s
  - NVMe M.2 ≈ 3000+ MB/s

> Used in: Modern laptops, desktops for lightning-fast boot times

---

## 4. **NVMe (Non-Volatile Memory Express)**

- **Protocol used with M.2 drives**
- **Super fast**: Utilizes PCIe bus instead of SATA
- **Low latency, high throughput**

> Used in: High-performance PCs, gaming rigs, servers

---

## 5. **Hybrid Drives (SSHD)**

- Combines:
  - HDD for capacity
  - SSD cache for speed
- Automatically moves frequently used data to SSD portion

> Used in: Budget-conscious users who want speed + space

---

## 6. **Optical Drives**

| Type  | Capacity      |
|-------|---------------|
| CD-R  | ~700 MB       |
| DVD-R | ~4.7 GB       |
| BD-R  | 25–50 GB      |

- **Used for:** Media, backups, legacy software
- **Note:** Becoming obsolete in modern systems

---

## 7. **Flash Storage**

- **Types:** USB flash drives, SD cards, microSD
- **Pros:** Portable, inexpensive, widely supported
- **Cons:** Slower than SSDs, wears out faster

---

## 8. **RAID (Redundant Array of Independent Disks)**

- **RAID 0:** Striping – speed, no redundancy
- **RAID 1:** Mirroring – redundancy, no speed gain
- **RAID 5:** Striping with parity – balance of speed + fault tolerance
- **RAID 10:** Combines 1 + 0 – fast + fault tolerant

> Often used in: Servers, NAS, high-performance environments

---

## 9. **Cloud Storage**

- **Examples:** Google Drive, OneDrive, Dropbox, iCloud
- **Pros:** Accessible anywhere, auto-backup
- **Cons:** Requires internet, security concerns

---

## 10. **Network Storage**

- **NAS (Network Attached Storage):**  
  Standalone device on a network that shares files (often uses RAID)
- **SAN (Storage Area Network):**  
  High-performance block-level storage, used in data centers

---

> **Tip for the Exam:** Focus on when and *why* to use each storage type — speed vs cost vs redundancy.

---
