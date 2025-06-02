# 🛡️ Switch Security Attacks – Flat Format Version

**User:** Chris (ct432)  
**Date:** 2025-06-01  
**Focus:** Layer 2 Threats + Defenses

---

**🔥 VLAN Hopping**

**Attack Type:**  
Exploiting VLAN trunking to access unauthorized VLANs.

**Techniques:**  
1. Switch Spoofing – Attacker mimics a trunking switch using 802.1Q.
2. Double Tagging – Attacker sends two VLAN tags; inner tag reaches another VLAN.

**Defense Tactics:**  
- switchport mode access  
- switchport nonegotiate  
- switchport access vlan <ID>  
- Set native VLAN to unused ID  
- Disable trunking on access ports  

---

**🔥 MAC Flooding**

**Attack Type:**  
Overloads the switch’s MAC address table, forcing it to broadcast traffic like a hub.

**Effect:**  
Attacker can sniff traffic across VLAN or user ports.

**Defense Tactics:**  
- switchport port-security  
- switchport port-security maximum 1  
- switchport port-security violation shutdown  
- Limit MACs per port  
- Enable shutdown or restrict on violation  

---

**🔥 DHCP Spoofing**

**Attack Type:**  
Rogue DHCP server gives clients fake gateway, DNS, and IP config.

**Effect:**  
Redirects traffic through attacker (Man-in-the-Middle).

**Defense Tactics:**  
- ip dhcp snooping  
- ip dhcp snooping trust  
- ip dhcp snooping limit rate 15  
- Trust only valid ports  
- Block rogue DHCP offers  
- Enable rate limiting on access ports  

---

**✅ Summary Table**

| Attack        | Effect                          | Key Defense Commands                         |
|---------------|----------------------------------|----------------------------------------------|
| VLAN Hopping  | VLAN access via spoofing         | `switchport mode access`, `nonegotiate`      |
| MAC Flooding  | Switch broadcasts to all ports   | `switchport port-security`                   |
| DHCP Spoofing | Rogue IP/DNS config to users     | `ip dhcp snooping`, `trust`, `rate limit`    |

---

**Tags:**  
`network+` `switch-security` `layer2-attacks` `cli-defenses` `mac-flooding` `vlan-hopping` `dhcp-spoofing`
