# Virtualization Basics – CompTIA A+ Core 1 (4.1)

Understand the fundamentals of virtualization — running multiple operating systems on a single physical machine using hypervisors and virtual environments.

---

## 🧠 What is Virtualization?

Virtualization allows one physical machine (host) to run multiple operating systems (guests) as virtual machines (VMs).

### Key Components:
- **Host Machine**: The physical system
- **Guest Machine**: The virtual machine (VM)
- **Hypervisor**: Manages VMs and system resources

---

## ⚙️ Types of Hypervisors

| Type      | Description                         | Examples                   |
|-----------|-------------------------------------|----------------------------|
| Type 1    | Bare-metal, runs directly on hardware | VMware ESXi, Microsoft Hyper-V |
| Type 2    | Runs within a host OS               | VirtualBox, VMware Workstation |

---

## 🛠 Common VM Features

- **Snapshots**: Save a VM’s state for rollback
- **Virtual Switches**: Allow networking between VMs
- **NAT/Bridged Mode**: Network visibility settings
- **Virtual Disk Files**: VHD/VMDK store VM’s virtual hard drive

---

## 🧰 Requirements for Virtualization

- CPU support: Intel VT-x / AMD-V
- Sufficient RAM and disk space
- Hypervisor installed

---

## 💡 A+ Exam Tips

- Know the differences between Type 1 and Type 2
- Understand VM terminology (guest, host, snapshot, virtual switch)
- Expect scenario-based questions about configuring or troubleshooting VMs

---

> “One machine. Infinite possibilities.”
