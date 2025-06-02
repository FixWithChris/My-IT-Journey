# 🛡️ VPN Protocols Drill – Network+ Flat Format

**User:** Chris (ct432)  
**Date:** 2025-06-01  
**Topic:** VPN Protocols – Function, Security, Use Cases

---

## 🔑 What is a VPN?

A **Virtual Private Network (VPN)** creates a secure, encrypted connection (tunnel) across an untrusted network like the internet.

---

## ✅ VPN Protocols Breakdown

---

**1. IPsec (Internet Protocol Security)**  
- **Tunneling?** ✅ Yes  
- **Encryption?** ✅ Yes  
- **Use Case:** Secure site-to-site and remote access VPNs  
- **Modes:**  
  - **Transport Mode:** Encrypts payload only  
  - **Tunnel Mode:** Encrypts entire packet  
- **Often used with:** L2TP or IKEv2

---

**2. L2TP (Layer 2 Tunneling Protocol)**  
- **Tunneling?** ✅ Yes  
- **Encryption?** ❌ No (by itself)  
- **Use Case:** Tunneling, but requires pairing with IPsec for security  
- **Combo Name:** L2TP/IPsec  
- **Advantage:** Widely supported on OS-level VPNs  

---

**3. PPTP (Point-to-Point Tunneling Protocol)**  
- **Tunneling?** ✅ Yes  
- **Encryption?** ❌ Weak (MS-CHAPv2)  
- **Use Case:** Legacy systems  
- **Status:** Deprecated – avoid in production  
- **Port:** TCP 1723  

---

**4. SSTP (Secure Socket Tunneling Protocol)**  
- **Tunneling?** ✅ Yes  
- **Encryption?** ✅ Strong (uses SSL/TLS)  
- **Use Case:** VPN over restrictive networks (e.g., hotels, firewalls)  
- **Port:** TCP 443  
- **Bonus:** Integrates cleanly with Windows

---

**5. IKEv2 (Internet Key Exchange v2)**  
- **Tunneling?** ✅ Yes (with IPsec)  
- **Encryption?** ✅ Yes  
- **Use Case:** Fast reconnects, stable mobile VPNs (e.g., iPhones switching networks)  
- **Bonus:** Supports mobility and multi-homing (MOBIKE)

---

**6. SSL VPN (Clientless / Web-based)**  
- **Tunneling?** ✅ Yes (via browser or lightweight client)  
- **Encryption?** ✅ Yes (TLS)  
- **Use Case:** Remote access via browser, secure portal  
- **Port:** TCP 443  
- **Note:** Ideal for application-layer VPN (email, files, etc.)

---

## 🧠 VPN Protocol Comparison Table

| Protocol | Encrypts | Native Tunnel | Stable? | Use Case                      | Port     |
|----------|----------|----------------|---------|-------------------------------|----------|
| IPsec    | ✅ Yes   | ✅ Yes         | ✅ Yes  | Site-to-site, remote client   | UDP 500  |
| L2TP     | ❌ No    | ✅ Yes         | ✅ Yes  | Use with IPsec                | UDP 1701 |
| PPTP     | ❌ Weak  | ✅ Yes         | ❌ No   | Obsolete legacy VPN           | TCP 1723 |
| SSTP     | ✅ Yes   | ✅ Yes         | ✅ Yes  | VPN over HTTPS (firewall safe)| TCP 443  |
| IKEv2    | ✅ Yes   | ✅ (with IPsec)| ✅ Yes  | Mobile VPNs, stable reconnect | UDP 500  |
| SSL VPN  | ✅ Yes   | ✅ Yes         | ✅ Yes  | Browser-based VPN             | TCP 443  |

---

## 🧠 Key Takeaways

- **Fastest & Most Stable:** IKEv2  
- **Firewall-Friendly:** SSTP, SSL VPN  
- **Legacy / Weak:** PPTP  
- **Best Practice Combo:** L2TP + IPsec or IKEv2 + IPsec  
- **Easiest for end users:** SSL VPN (no full install needed)

---

## 📁 Tags  
`network+` `vpn` `ipsec` `l2tp` `sstp` `pptp` `ikev2` `ssl-vpn` `secure-remote-access` `tunneling`
