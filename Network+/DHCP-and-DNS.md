# DHCP vs DNS

Date: May 2025  
Focus: Understanding how IP addresses are assigned (DHCP) and resolved (DNS)

---

## DHCP – Dynamic Host Configuration Protocol

Purpose: Automatically assigns IP configuration to devices

Provides:
- IP address
- Subnet mask
- Default gateway
- DNS server

DORA Process:
1. Discover – Client looks for DHCP server  
2. Offer – Server offers IP lease  
3. Request – Client requests the lease  
4. Acknowledge – Server confirms

Windows Commands:
ipconfig /release  
ipconfig /renew

If DHCP fails: Device receives an APIPA address (169.254.x.x)

---

## DNS – Domain Name System

---

## DNS Lookup Breakdown (Root → Authoritative)

When you type a domain like `example.com`, your system doesn't magically know the IP. Here's the behind-the-scenes journey:

1. **Client Device**  
   - Asks its local DNS resolver (usually your router or ISP).

2. **DNS Resolver (Recursive)**  
   - If not cached, sends request outward.

3. **Root Server**  
   - Directs the resolver to the correct **Top-Level Domain (TLD)** server  
   - Example: For `.com`, it sends it to a `.com` nameserver.

4. **TLD Server**  
   - Points the resolver to the **Authoritative Name Server** responsible for `example.com`

5. **Authoritative Name Server**  
   - Responds with the actual IP address for `example.com`

6. **Back to Client**  
   - Resolver sends final IP to the client  
   - DNS info is now cached locally for speed

---

### Visual Flow:

Device → Recursive Resolver → Root Server  
→ TLD Server → Authoritative Server → IP Address

---

### Quick Summary

- **Root Server**: The top of the DNS hierarchy (knows where TLDs live)  
- **TLD Server**: Manages `.com`, `.net`, `.org`, etc.  
- **Authoritative Server**: Holds the actual IP info for the requested domain

---

Understanding this flow helps you troubleshoot:
- Why DNS sometimes takes longer
- Why a domain might work on one device and not another (due to caching)
- How DNS is *layered*, not instant

Purpose: Resolves domain names to IP addresses  
Example: google.com → 142.250.190.206

Why It Matters: Without DNS, users must remember IPs to access websites.

Windows Commands:
nslookup google.com  
ipconfig /flushdns

If DNS fails:
- You can ping 8.8.8.8 but not google.com
- Indicates DNS resolution issue

---

## Key Differences

DHCP:
- Assigns IP and network settings
- Runs when device joins network
- Uses ports 67 (server) and 68 (client)

DNS:
- Resolves names to IPs
- Runs during every domain lookup
- Uses port 53

---

## Troubleshooting Flow

1. Run ipconfig → Check for valid IP  
   - If 169.254.x.x → DHCP failed  
2. ping 8.8.8.8 → If this works, internet is live  
3. ping google.com → If this fails, DNS is broken  
4. Run nslookup → Test name resolution  
5. Run ipconfig /flushdns → Clear local DNS cache

---

Quote:
DHCP gets you online.  
DNS shows you where to go.
