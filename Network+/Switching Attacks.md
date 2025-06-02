# 🛡️ Switching Attacks Drill – Network+

**User:** Chris (ct432)  
**Date:** 2025-06-01  
**Focus:** Layer 2 Attacks + Mitigations (VLAN, Switch Security)

---

## 🚨 VLAN Hopping

### 🔸 Attack Type:
- Layer 2 attack to **gain access to unauthorized VLANs**

### 🔹 Techniques:
1. **Switch Spoofing (802.1Q Spoofing)**  
   - Attacker pretends to be a switch  
   - Exploits dynamic trunk negotiation  
   - Gains access to all VLANs on the trunk

2. **Double Tagging**  
   - Inserts two VLAN tags into one Ethernet frame  
   - First switch strips outer tag  
   - Inner tag forwards to target VLAN

### 🛡️ Defense Tactics:
```bash
switchport mode access
switchport nonegotiate
switchport access vlan <ID>
