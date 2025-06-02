# 🔐 Tunneling Protocols Drill – Network+ Flat Format

**User:** Chris (ct432)  
**Date:** 2025-06-01  
**Topic:** Tunneling vs. Non-Tunneling Protocols

---

**❓ Drill Focus:**  
Which protocols create secure or encapsulated tunnels between TCP/IP systems—and which don’t?

---

**✅ Correct Answer:**  
**NAT (Network Address Translation)**  
- **Purpose:** Translates private IPs to public IPs  
- **Tunneling?** ❌ No  
- **Encryption?** ❌ No  
- **Why it's correct:** NAT modifies packet headers for address routing, but does not create a tunnel or secure link.

---

**❌ Incorrect Options (They All Use Tunneling):**

**1. IPsec (Internet Protocol Security)**  
- **Purpose:** Encrypts IP traffic  
- **Tunneling?** ✅ Yes  
- **Encryption?** ✅ Yes (ESP mode)  
- **Note:** Common in VPNs. Works in transport or tunnel mode.

**2. L2TP (Layer 2 Tunneling Protocol)**  
- **Purpose:** Encapsulates Layer 2 frames  
- **Tunneling?** ✅ Yes  
- **Encryption?** ❌ No (used with IPsec for security)  
- **Note:** Forms tunnel, but needs help securing it.

**3. mGRE (Multipoint Generic Routing Encapsulation)**  
- **Purpose:** Supports one-to-many VPN tunnels  
- **Tunneling?** ✅ Yes  
- **Encryption?** ❌ No  
- **Note:** Cisco-specific; secure only when combined with IPsec or other encryption.

---

**📘 Comparison Table**

| Protocol | Tunnels? | Encrypts? | Primary Function                        |
|----------|----------|-----------|------------------------------------------|
| NAT      | ❌ No    | ❌ No     | IP address translation (not a VPN)       |
| IPsec    | ✅ Yes   | ✅ Yes    | Secures IP traffic (VPN standard)        |
| L2TP     | ✅ Yes   | ❌ No     | Tunnels Layer 2, pairs with IPsec        |
| mGRE     | ✅ Yes   | ❌ No     | Multipoint tunneling, Cisco VPNs         |

---

**🧠 Key Takeaway:**  
> If it encrypts or encapsulates—it's tunneling.  
> If it just rewrites IPs—it's **not**.

---

**📁 Tags**  
`network+` `vpn` `tunneling-protocols` `nat` `ipsec` `l2tp` `mgre` `drill-log`
