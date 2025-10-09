# 🧠 Core 2 Network Troubleshooting Guide

This guide explains how to use `tracert`, `ping`, `nslookup`, and other tools to diagnose where a network outage occurs.  
Each command reveals a different layer of the network — from your PC, to the router, to the ISP, to the destination server.

---

## ⚙️ What `tracert` Does
`tracert` (Traceroute) tracks the path your data takes to reach a destination, showing every router or “hop” along the way.  
If communication breaks at a certain hop, that’s where the issue lies.

Example:
---

## 🔍 How to Read Traceroute Results

### 1️⃣ Fails on the First Hop
**Problem Area:** Local computer or router.  
**Possible Causes:**
- Network adapter disabled
- Wrong default gateway
- Wi-Fi disconnected

**Fix:**  
Run `ipconfig` to verify IP and gateway, restart adapter or router.

---

### 2️⃣ Stops at Hop 2–3
**Problem Area:** Between local network and ISP.  
**Fix:**  
Check ISP connection, test other devices, reboot modem/router.

---

### 3️⃣ Dies Mid-Path
**Problem Area:** ISP or backbone provider.  
**Fix:**  
Contact ISP and report the hop where it stops.

---

### 4️⃣ Reaches Destination’s Network but Times Out
**Problem Area:** Usually NOT an outage — the destination network/firewall blocks ICMP.  
**Fix:**  
Test with `ping` or a web browser. If the site loads, it’s not a real issue.

---

## 🧩 Real-World Troubleshooting Strategy

| Command | Purpose | What It Reveals |
|----------|----------|----------------|
| `ping` | Tests if host replies | Basic reachability |
| `tracert` | Maps route to host | Finds where packets stop |
| `nslookup` | Checks DNS resolution | Verifies name → IP works |
| `ipconfig /all` | Shows local settings | IP, Gateway, DNS correctness |

**Interpretation Flow:**
- `ping` fails + `tracert` fails at hop 1 → Local config issue  
- `ping` fails + `tracert` stops mid-path → Routing/ISP issue  
- Both succeed, but site fails → Server or app-layer issue  

---

## 📊 Layers of What You’re Fixing

| Tool | Layer | Purpose |
|------|--------|---------|
| `ipconfig` | Layer 1–3 | Check NIC, IP, gateway |
| `ping` | Layer 3 | Test connectivity |
| `tracert` | Layer 3 | Identify where packets drop |
| `nslookup` | Layer 7 | Validate DNS resolution |

---

## 🧠 Summary
- `tracert` shows **how far** your packets travel.
- **Timeouts** don’t always mean failure — many routers block ICMP.
- Use multiple tools together for clarity.
- Combine results with logical reasoning across OSI layers.

---

### ✅ Example: Your Hilton Trace
✔ Local network = good  
✔ ISP routing = good  
⚠ Destination network = blocks ICMP (normal, not outage)

---

**Author:** Chris 
**Purpose:** Core 2 Lab Notes — Network Troubleshooting Section  
 
