# 🖥️ Virtualization Concepts Drill – Network+ Flat Format

**User:** Chris (ct432)  
**Date:** 2025-06-01  
**Topic:** Virtualization, VDI, Hypervisors, Virtual Networking

---

## 🧠 What Is Virtualization?

**Virtualization** is the creation of a virtual (not physical) version of computing environments, including:
- Operating systems
- Servers
- Desktops
- Storage
- Network interfaces

---

## 🔹 Key Virtualization Terms

---

**1. Virtual Desktop Infrastructure (VDI)**  
- **What it is:** A desktop environment hosted on a **remote server**  
- **Accessed via:** Remote clients (RDP, Citrix, etc.)  
- **Use Case:** Thin clients, remote workforces, centralized management  
- **Benefits:** Security, scalability, quick recovery  

---

**2. Virtual Desktop**  
- **What it means:** A user-facing desktop that is **not local to the machine**  
- Can be:
  - A VM image (e.g., Windows 10 on Azure Virtual Desktop)  
  - A VR-enabled desktop (e.g., Oculus Virtual Desktop app)  
  - A Linux “workspace switcher” (virtual desktop environments)  
- **Important:** Does **not** include projector-based systems (those are hardware, not virtual environments)

---

**3. Hypervisor**  
- **Type 1 (Bare-metal):** Runs **directly on hardware**  
  - Examples: VMware ESXi, Microsoft Hyper-V, XenServer  
- **Type 2 (Hosted):** Runs **on top of an OS**  
  - Examples: VMware Workstation, VirtualBox, Parallels  
- **Purpose:** Creates and manages virtual machines (VMs)

---

**4. Virtual Switch (vSwitch)**  
- **What it does:** Enables communication between VMs and the physical network  
- **Acts Like:** A software-based Layer 2 switch  
- **Bonus:** Can enforce VLANs and policies

---

**5. Snapshot**  
- **What it is:** A saved state of a VM (memory, disk, config)  
- **Use Case:** Rollback after patching or testing  
- **Caution:** Long-term snapshot use can slow performance

---

## 📘 Comparison Table

| Concept         | Purpose                               | Key Feature                         |
|------------------|----------------------------------------|--------------------------------------|
| VDI              | Hosted desktop access                 | Centralized user environments        |
| Virtual Desktop  | Remote or layered user environment    | Exists independently of local device |
| Hypervisor Type 1| Bare-metal VM host                    | Runs directly on hardware            |
| Hypervisor Type 2| Host-based VM software                | Runs within existing OS              |
| Virtual Switch   | Network interface for VMs             | Software switch, supports VLANs      |
| Snapshot         | Restore point for VMs                 | Revert state, no full backup         |

---

## ❌ NOT Considered a Virtual Desktop

> “A hardware device that projects a computer desktop onto a surface”  
= **Physical projection**, not software abstraction. Doesn’t qualify.

---

## 📁 Tags  
`network+` `virtualization` `vdi` `hypervisor` `virtual-switch` `snapshots` `remote-desktop` `drill-log`
