# DHCP vs DNS

**Date:** May 2025  
**Focus:** Core networking services – how IP addresses are assigned and resolved

---

## What is DHCP?

**Dynamic Host Configuration Protocol**

- Assigns IP addresses automatically to devices on a network  
- Also assigns:
  - Subnet mask
  - Default gateway
  - DNS server
- Prevents IP conflicts and manual setup

**Process: DORA**

1. **Discover** – Client sends a broadcast looking for DHCP servers  
2. **Offer** – Server responds with IP lease offer  
3. **Request** – Client accepts offer  
4. **Acknowledge** – Server confirms lease

**Commands:**
```bash
ipconfig /release
ipconfig /renew
