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
