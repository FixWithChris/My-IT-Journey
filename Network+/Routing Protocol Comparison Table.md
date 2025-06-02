# 🌐 Routing Protocol Comparison Table

**Topic:** Network+ – Routing Protocols  
**User:** Chris (ct432)  
**Date:** 2025-06-01

---

| Protocol | Type                    | Metric                                | IPv6 Support | Classful/Classless | Use Case                        | Key Notes                              |
|----------|-------------------------|----------------------------------------|---------------|--------------------|----------------------------------|----------------------------------------|
| RIP v1   | Distance Vector         | Hop Count                             | ❌ No         | Classful           | Small legacy networks           | Max 15 hops, no subnet info             |
| RIP v2   | Distance Vector         | Hop Count                             | ✅ Yes (via RIPng) | Classless     | Small/medium IPv4/IPv6 networks | Includes subnet mask, next hop         |
| EIGRP    | Advanced Distance Vector| Bandwidth, Delay, Reliability, Load   | ✅ Yes        | Classless           | Cisco-only internal routing     | Fast convergence, DUAL algorithm        |
| OSPF     | Link-State              | Cost (bandwidth-based)                | ✅ Yes        | Classless           | Enterprise internal routing     | Area-based design, uses LSAs            |
| BGP      | Path Vector             | Path attributes (AS path, etc.)       | ✅ Yes        | Classless           | Internet routing between ASes   | Exterior routing protocol (EGP)         |

---

✅ **Quick Reference Notes:**
- **RIP v1**: Outdated, classful, no subnet support.
- **RIP v2**: Updated with mask & next hop support.
- **EIGRP**: Cisco proprietary with rich metrics.
- **OSPF**: Link-state, scalable, efficient in large networks.
- **BGP**: The backbone of the internet; routes between large networks (ASes).

---

## 🗂️ Tags  
`network+` `routing-protocols` `rip` `eigrp` `ospf` `bgp` `exam-review` `networking-core`

# 🧪 Routing Protocol Command Drill Pack – Network+

**User:** Chris (ct432)  
**Focus:** Routing Protocol CLI Practice  
**Date:** 2025-06-01  

---

## 🔄 RIP Command Drills

### View active RIP configuration:
```bash
show ip protocols
