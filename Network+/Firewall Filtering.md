# 🔥 Firewall Filtering Types Drill – Network+ Flat Format

**User:** Chris (ct432)  
**Date:** 2025-06-01  
**Topic:** Firewall Filtering Methods – Network+ Exam Focus

---

## ❓ What’s the Scenario?

> Which term describes when a firewall examines port numbers within transport layer headers?

---

**✅ Correct Answer:**  
**Service-dependent filtering**  
- **Definition:** Firewall inspects **transport layer protocol headers** (TCP/UDP) to determine the service (e.g., port 80 for HTTP, port 443 for HTTPS).  
- **Used In:** Stateful firewalls  
- **Purpose:** Allows or blocks traffic based on session type and known service behavior (e.g., TCP handshakes)

---

## ❌ Why the Other Options Are Wrong

**1. Deep Packet Inspection (DPI)**  
- **What it does:** Inspects **packet payloads**, not just headers  
- **Used for:** Malware detection, content filtering, application identification  
- **Not correct here** because it operates beyond the transport layer

**2. Next-Generation Firewall (NGFW)**  
- **What it is:** A firewall type, not a filtering **method**  
- **Capabilities:** DPI, app-layer control, intrusion prevention  
- **Not correct here** because the question asked about **filtering behavior**, not firewall models

**3. IP Address Filtering**  
- **What it does:** Filters based on **source and destination IPs**  
- **Limitation:** Doesn’t consider ports or protocols  
- **Not correct here** because it doesn’t use transport layer info

---

## 🧠 Firewall Filtering Comparison Table

| Filter Type               | Looks At                         | Use Case                              |
|---------------------------|----------------------------------|----------------------------------------|
| IP Address Filtering      | Source/Destination IP only       | Simple whitelist or blacklist rules    |
| Port-based Filtering      | TCP/UDP port numbers             | Service control (block FTP, allow HTTP)|
| **Service-dependent Filtering** | Ports + session state (SYN, ACK) | Stateful filtering based on service behavior |
| Deep Packet Inspection    | Payload/content                  | Malware scans, app identification      |
| NGFW                      | Uses DPI + advanced techniques   | App-aware, content-aware firewalling   |

---

## 🧠 Quick Definitions

- **Stateful Firewall:** Remembers connections and filters traffic based on state and expected behavior.
- **Stateless Firewall:** Makes decisions per-packet, without memory of past traffic.
- **NGFW:** Combines DPI, signature detection, app awareness, and traditional filtering.

---

## 📁 Tags  
`network+` `firewalls` `filtering-methods` `dpi` `ngfw` `stateful-firewall` `packet-filtering` `drill-log`
