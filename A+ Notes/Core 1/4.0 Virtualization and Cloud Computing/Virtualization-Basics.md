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
>
> # CompTIA A+ — Virtualization Concepts  
**Objective 4.2: Given a scenario, select and install storage devices**

---

## Virtualization

- **Virtualization**: Host computer installed with a hypervisor that can be used to install and manage multiple guest operating systems or virtual machines (VMs)

  - **Type I Hypervisor (Bare Metal)**:  
    Runs directly on the host hardware and functions as the operating system

  - **Type II Hypervisor**:  
    Runs within the normal operating system

- Ensure that each virtual machine runs its own copy of an operating system

---

## Access Models

- **Server-based (Terminal Services)**  
  Server-based solution that runs the application on servers in a centralized location

- **Client-based (Application Streaming)**  
  Client-based solution that allows an application to be packaged up and streamed directly to a user’s PC

---

## Containerization

- Each container relies on a common host OS as the base for each container
- Examples: Docker, Parallels Virtuozzo, OpenVZ

---

## Virtualization Risks

1. When a physical server crashes, all organizations hosted on that same server are affected
2. An organization's failure to secure virtual environments poses a security risk for others

---

## Best Practices

- Set up virtual servers in the cloud with:
  - Proper failover
  - Redundancy
  - Elasticity
- Hosting all VMs on the same type of hypervisor:
  - Requires proper configurations
  - Ensure hypervisors are patched and up-to-date
  - Apply tight access control

---

## Virtual Machine Purposes

- **Hypervisor**  
  Manages the distribution of physical resources to the VMs

  - Type I – Bare Metal  
  - Type II – Hosted

---

## Container-Based Virtualization

- Less resource-intensive
- Doesn’t require its own copy of the OS

---

## Additional Concepts

- **Hyperconverged Infrastructure**  
  Full integration of storage, network, and servers

- **Application Virtualization**  
  Encapsulates applications to run independent of the underlying OS

- **Virtual Desktop Infrastructure (VDI)**  
  Centralized hosting of virtual desktop OS

- **Sandboxing**  
  Isolated environment used for malware analysis

- **Cross-Platform Virtualization**  
  Used to test/run software across OSes

  - Emulation
  - System Imitation
  - Virtualization to simulate a new “physical” machine

---

## Resource Requirements

- **SLAT (Second Level Address Translation)**  
  Optimizes virtual memory performance

- **Processor Architecture**  
  - x86: 32-bit processor, 4GB RAM max  
  - x64: 64-bit processor, 16 exabytes of RAM  
  - ARM: Reduced instruction set

- **System Memory**  
  - Barebones Windows: 20–50 GB  
  - Linux: 4–8 GB  
  - macOS: 20–40 GB

- **NIC Teaming**  
  Multiple network cards for higher speeds

---

## Security Requirements

- **VM Escape**:  
  Threat attempts to break out of VM to control the hypervisor or host OS  
  - Easier on Type II hypervisor  
  - Mitigations: Up-to-date patches, secure configurations

- **VM Hopping**:  
  Attempts to move from one VM to another on same host

---

## Other Key Terms

- **Sandbox Escape**  
  Attacker bypasses sandbox to access host OS or privileged processes

- **Live Migration**  
  Moving VM from one host to another while running (requires trusted network/encryption)

- **Data Remnants**  
  Residual data not wiped  
  - Mitigate via encryption or destroying encryption keys

- **VM Sprawl**  
  Uncontrolled deployment of too many VMs
