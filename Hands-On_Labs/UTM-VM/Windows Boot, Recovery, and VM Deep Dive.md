# Windows Boot, Recovery, and VM Deep Dive (UTM on Apple Silicon)

## Objective
Develop a *first-principles understanding* of how Windows boots, recovers, and fails — by intentionally breaking and rebuilding a Windows 11 VM on UTM (Apple Silicon).

---

## Environment
- Host OS: macOS (Apple Silicon / M2)
- Hypervisor: UTM (QEMU + EDK II UEFI)
- Guest OS: Windows 11 (ARM64)
- Firmware: UEFI (EDK II)
- Disk Layout: GPT with EFI System Partition (ESP)
- Encryption: BitLocker enabled (auto by Windows)

---

## High-Level Concepts Covered
- UEFI vs Windows
- EFI System Partition (ESP)
- Bootloaders vs Kernel
- BCD (Boot Configuration Data)
- WinRE vs Safe Mode
- BitLocker interaction with recovery
- Why some failures are *not* recoverable
- Driver loading during Windows setup
- VirtIO drivers in virtualized environments

---

## Windows Boot Chain (Correct Mental Model)
