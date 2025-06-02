# 🌐 DNS Records– Network+ Flat Format

**User:** Chris (ct432)  
**Date:** 2025-06-01  
**Focus:** DNS Resource Records + Zone Management

---

**🧠 Core Concept: What is a DNS Zone?**  
A **zone** is a segment of the DNS namespace managed by a specific group of authoritative name servers. These servers are defined using **NS records**.

---

**✅ Correct Record for Delegating DNS Authority**

**Record:** `NS` (Name Server)  
**Purpose:** Specifies the authoritative DNS servers for a given zone.

**Example:**  

---

**❌ Common Distractors & Why They're Wrong**

**Record:** `PTR`  
- **Use:** Reverse DNS (IP → domain name)  
- **Example:** `192.0.2.1 → mail.example.com`  
- **Wrong Because:** Doesn’t assign DNS zone authority  

**Record:** `MX`  
- **Use:** Directs email traffic to the right mail server  
- **Example:** `example.com → mail.example.com`  
- **Wrong Because:** Used for email routing only  

**Record:** `SRV`  
- **Use:** Directs clients to specific services and ports  
- **Example:** `_sip._tcp.example.com`  
- **Wrong Because:** Used in VoIP, LDAP, etc.—not DNS delegation  

---

**📘 DNS Records Summary Table**

| Record | Purpose                                | Example                        |
|--------|----------------------------------------|--------------------------------|
| A      | Maps domain → IPv4                     | `example.com → 192.0.2.1`      |
| AAAA   | Maps domain → IPv6                     | `example.com → ::1`            |
| NS     | Authoritative name server              | `example.com → ns1.dns.net`    |
| MX     | Mail exchange for email delivery       | `example.com → mail.example.com` |
| CNAME  | Canonical name alias                   | `www → example.com`            |
| PTR    | Reverse DNS lookup                     | `192.0.2.1 → host.example.com` |
| SRV    | Maps services to specific hosts/ports  | `_sip._tcp.example.com`        |
| TXT    | Holds text for SPF, DKIM, validation   | `v=spf1 include:_spf.google.com` |

---

**💡 Net+ Tip:**  
If you see a question asking:  
> “Which record identifies the DNS servers responsible for a zone?”  
It’s always `NS`.

---

**📁 Tags**  
`network+` `dns-records` `ns` `mx` `ptr` `srv` `dns-zones` `flat-drill` `zone-delegation`
