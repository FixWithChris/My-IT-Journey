# 🧮 Subnetting Practice — Recognition & Confidence

**Goal:**  
Subnet quickly, accurately, and without second-guessing.  
Focus is on **pattern recognition**, not binary conversion.

---

## 1️⃣ Core Subnetting Rules (Non-Negotiable)

### Rule 1 — Block Size
> **Block size = 256 − last subnet mask octet**

Only look at the **interesting octet**.

---

### Rule 2 — Same Subnet Test
> If the **IP and default gateway fall within the same block**, they are in the same subnet.

No extra math required.

---

### Rule 3 — Network Boundaries
Subnets always start at **multiples of the block size**.

---

## 2️⃣ Must-Know Block Sizes (Memorize These)

| Subnet Mask | CIDR | Block Size | Usable Hosts |
|------------|------|------------|--------------|
| 255.255.255.0 | /24 | 256 | 254 |
| 255.255.255.128 | /25 | 128 | 126 |
| 255.255.255.192 | /26 | 64 | 62 |
| 255.255.255.224 | /27 | 32 | 30 |
| 255.255.255.240 | /28 | 16 | 14 |
| 255.255.255.248 | /29 | 8 | 6 |
| 255.255.255.252 | /30 | 4 | 2 |

---

## 3️⃣ Subnet Range Identification (No Math Writing)

### Example    IP:   192.168.10.77
Mask: 255.255.255.192     

- Block size = 64
- Subnet starts at:
  - .0
  - .64
  - .128
  - .192

77 falls in:  192.168.10.64 – 192.168.10.127

---

## 4️⃣ Default Gateway Validation Practice

### Scenario A   IP:      10.0.5.22
Mask:    255.255.255.224
Gateway: 10.0.5.1

- Block size = 32
- Subnets: .0, .32, .64, .96…

22 is in `.0–.31`  
Gateway `.1` is also in `.0–.31`

✅ **Gateway is valid**

---

### Scenario B    IP:      192.168.50.130
Mask:    255.255.255.192
Gateway: 192.168.50.1

- Block size = 64
- Subnets: .0–.63, .64–.127, .128–.191

IP is in `.128–.191`  
Gateway `.1` is in `.0–.63`

❌ **Gateway is NOT in the same subnet**

---

## 5️⃣ Rapid Recognition Drills (Answer in < 5 Seconds)

### Drill 1 — Network Boundary  IP:   172.16.4.199
Mask: 255.255.255.128

Answer:
- Network starts at: `.128`

---

### Drill 2 — Valid or Invalid Gateway   IP:      192.168.1.14
Mask:    255.255.255.240
Gateway: 192.168.1.1

Answer:
- ❌ Invalid (block size 16 → `.0–.15`, gateway OK)
- ✅ Actually valid — this tests hesitation

---

### Drill 3 — Hosts per Subnet
Mask: /27

Answer:
- **30 usable hosts**

---

## 6️⃣ Common Exam Traps (Avoid These)

- ❌ Thinking DNS issues are subnet issues
- ❌ Forgetting to check the **gateway’s subnet**
- ❌ Doing binary when recognition is faster
- ❌ Assuming `/24` when mask is different

---

## 7️⃣ Mental Checklist (Use Every Time)

1. Identify the **interesting octet**
2. Calculate **block size**
3. Identify **subnet boundaries**
4. Place IP into a block
5. Check gateway against that block

---

## 8️⃣ Technician Translation (Real-World Use)

If:
- IP exists
- Gateway exists
- Gateway is outside subnet

Then:
> “This device cannot leave its local network.”

That’s not a DNS issue.  
That’s not a firewall issue.  
That’s a **subnet configuration issue**.

---

## ✅ Session Takeaway

Subnetting is not about math speed.  
It’s about **pattern confidence**.

When the patterns are automatic:
- Exams slow down
- Mistakes drop
- Troubleshooting becomes calm

---
