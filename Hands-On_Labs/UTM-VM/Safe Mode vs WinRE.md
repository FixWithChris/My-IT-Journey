---

## Key Clarifications & Corrections

### 1. Safe Mode vs WinRE
- **Safe Mode**
  - IS Windows
  - Kernel is loaded
  - Minimal drivers + services
  - GUI available
- **WinRE**
  - Separate recovery environment
  - Launched via bootloader/BCD
  - NOT guaranteed if boot chain is broken

❗ Safe Mode cannot run if Windows cannot boot.

---

### 2. WinRE Dependency Reality
- WinRE requires:
  - Functional EFI loader
  - Valid BCD entry
  - Access to disk
- If **BCD or bootloader is corrupted**, WinRE may be unreachable.
- “No OS found” does NOT guarantee WinRE access.

---

### 3. EFI System Partition (ESP)
- ESP = **EFI System Partition**
- FAT32 formatted
- Contains:
