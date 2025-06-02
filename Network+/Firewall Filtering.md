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

# 🧱 Stateful vs. Stateless Firewall Drill – Network+ Flat Format

**User:** Chris (ct432)  
**Date:** 2025-06-01  
**Topic:** Firewall Types – Packet Behavior & Traffic Control

---

## 🔑 Core Difference

| Type      | Tracks Sessions? | Intelligent Filtering? | Speed     | Memory Use | Use Case                         |
|-----------|------------------|-------------------------|-----------|------------|----------------------------------|
| **Stateful** | ✅ Yes           | ✅ Yes (context-aware)    | Medium    | High        | Secure corporate networks        |
| **Stateless** | ❌ No            | ❌ No (per-packet only)   | Fast      | Low         | Lightweight rules, simple edge devices |

---

## ✅ **Stateful Firewall**

- **Remembers active connections**
- Evaluates packets based on:
  - Source/destination IP
  - Port number
  - **Session state** (e.g., is this part of an existing TCP handshake?)
- Dynamically opens/blocks ports based on traffic flow
- **More secure**, but needs more resources

**Example Use:**  
Corporate perimeter firewall, advanced packet inspection, internal segmentation.

---

## ⚠️ **Stateless Firewall**

- Evaluates packets **individually**, no memory of past packets
- Relies only on static rules:
  - "Allow TCP from 192.168.1.5 to port 80"
- **Faster**, but can't adapt to real-time session data

**Example Use:**  
Basic packet filtering, cloud firewalls, IoT edge control, DDoS rate-limiting.

---

## 🧠 TCP Session Scenario Example

**You send a TCP packet from your laptop to a web server (port 80).**

| Firewall Type | Behavior |
|---------------|----------|
| Stateless     | Sees a TCP packet to port 80, checks rule, allows/blocks it – no session awareness. |
| Stateful      | Checks if this is part of a valid session (SYN/ACK), and may auto-open return path – context-aware. |

---

## 🚨 Exam Tip

> If the question says “remembers connections,” “tracks sessions,” or “dynamic rule decisions” — it's **stateful**.

If it says “static rules only,” “no memory,” or “packet-by-packet” — it's **stateless**.

---

## 🧱 Real-World Combo

Most enterprise firewalls today are **stateful**, often with stateless filtering at the **edge** (cloud load balancers, pre-screen filters).

---

## 📁 Tags  
`network+` `firewalls` `stateful` `stateless` `security-filtering` `traffic-flow` `tcp-sessions` `drill-log`
