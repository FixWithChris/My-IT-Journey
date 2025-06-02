# 🚧 Troubleshooting Drill – Duplex Mismatch

**User:** Chris (ct432)  
**Date:** 2025-06-01  
**Topic:** Network Troubleshooting – Ethernet Errors

---

**🧩 Scenario Recap**

- You installed new computers on a Gigabit Ethernet network.
- Configured them to use **1 Gbps, full duplex**.
- Ping tests were successful.
- But during real usage, users report:
  - Poor performance  
  - Dropped packets  
  - Network slowdowns

---

**🔎 Symptoms Observed**

- Packet collisions  
- **Late collisions**  
- CRC (Cyclic Redundancy Check) errors  
- **Runt frames**

---

**✅ Correct Diagnosis: Duplex Mismatch**

A **duplex mismatch** occurs when:
- One device is set to **full duplex**
- The other is set to **half duplex**

**Effect:**
- Half-duplex side uses CSMA/CD and sees incoming traffic as a collision.
- Full-duplex side keeps sending without waiting.
- Leads to:
  - CRC errors
  - Retransmissions
  - Major performance issues

---

**🧪 Signature Symptoms Table**

| Symptom               | Explanation                                       |
|-----------------------|---------------------------------------------------|
| CRC Errors            | Frame corruption due to unexpected collisions     |
| Runt Frames           | Frames are cut short due to collision interruption |
| Late Collisions       | Happen after the first 64 bytes (abnormal timing) |
| Good Ping, Bad Traffic| Ping works (light load), real use breaks it       |

---

**❌ Why Other Answers Are Wrong**

| Option                        | Why it's Incorrect                               |
|------------------------------|--------------------------------------------------|
| Incorrect Cable Type         | Would result in no link or downgraded speed, not collisions |
| TX/RX Reversal               | Would stop link from working at all              |
| Damaged Cables               | Could cause CRCs, but **not late collisions**    |

---

**🧠 Key Takeaway**

> CRC + collisions + late collisions = **duplex mismatch**  
> Always match duplex manually or use auto-negotiation on both ends

---

**🛠️ Quick Fix**

- Check NIC settings and switch port settings
- Set both sides to:
  - **Auto-negotiate**  
  - Or explicitly match: `1 Gbps / Full duplex`

---

**📁 Tags**  
`network+` `troubleshooting` `duplex-mismatch` `crc-errors` `late-collisions` `ethernet` `field-diagnostics`
