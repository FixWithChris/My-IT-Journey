# Subnetting Practice Log

**Date:** May 2025  
**Focus:** CIDR, block sizes, usable ranges, broadcast calculation

---

## Key Concepts

- Hosts = 2^(32 - subnet bits) - 2
- Block Size = 256 - subnet mask value
- Broadcast address = Last IP in the range
- Usable IP range = From (Network +1) to (Broadcast -1)

---

## Example 1

**IP:** 192.168.5.0/26  
- Block size = 64  
- Range: 192.168.5.0 – 192.168.5.63  
- Usable: 192.168.5.1 – 192.168.5.62  
- Broadcast: 192.168.5.63

---

## Example 2

**IP:** 192.168.5.130/27  
- Block size = 32  
- Range: 192.168.5.128 – 192.168.5.159  
- Usable: 192.168.5.129 – 192.168.5.158  
- Broadcast: 192.168.5.159

---

## Mistakes I Made

- Added block size to usable IP instead of base  
- Miscounted usable IPs  
- Confused broadcast location

---

## Takeaways

- Say it aloud: *“Broadcast is always last. Network is first.”*  
- Draw IP number lines  
- Practice smaller block sizes: /29, /30

---
