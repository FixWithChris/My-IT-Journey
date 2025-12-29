- Result:
- Error screen
- No WinRE menu
- Demonstrated bootloader dependency on valid config + environment

---

## BitLocker Discovery & Impact

### What Happened
- System prompted for **BitLocker recovery key**
- This occurred because:
- Boot state changed
- TPM trust was broken (VM context)
- Without the key:
- OS volume inaccessible
- BCD repair impossible
- WinRE limited

### Key Insight
> You cannot repair what you cannot decrypt.

BitLocker protects **data integrity over recoverability**.

---

## Why the System Became Unrecoverable
- No installation media available
- BitLocker blocked disk access
- BCD + loader state inconsistent
- UEFI could run `.efi` files, but Windows could not initialize

✅ Correct decision: **Rebuild VM**

---

## Windows Reinstallation (Correct Path)

### ISO Selection
- Downloaded Windows 11 ARM64 ISO
- Used Insider Preview (UTM-compatible)

### Installation Flow
- Booted ISO via UEFI
- Windows Setup launched successfully
- Encountered network issue (expected)

---

## Network Driver Issue Explained

### Why No Internet?
- Windows setup environment is minimal
- No driver for virtual NIC
- Network device detected, driver missing

### Solution
- Attach **VirtIO driver ISO**
- Load driver manually during setup

---

## File Transfer: macOS → UTM
Methods discussed:
- Shared directory (UTM feature)
- ISO attachment
- Drag-and-drop (post-install)

---

## Key Takeaways

### Technical
- Bootloaders are just files
- Recovery is conditional, not guaranteed
- Encryption changes everything
- Firmware ≠ OS
- Drivers gate functionality, not hardware

### Mental Models Upgraded
- Boot failures are structural, not random
- Reinstallation can be the *correct* fix
- Understanding dependencies > memorizing steps

---

## Final Reflection
This exercise turned a failed VM into:
- A full boot-chain walkthrough
- A recovery-path stress test
- A practical understanding of Windows internals

**Outcome:** Deeper, durable knowledge — not just a working VM.

---

## Next Optional Drills
- Disable WinRE intentionally
- Break and rebuild BCD
- Compare Linux boot chain
- Tie boot security to malware persistence
