# Ports and Protocols

**Date:** May 2025  
**Focus:** Common ports and protocols every IT tech should know

---

## Why This Matters

Ports are like numbered doors that services use to communicate across the network.  
Protocols define the language and structure of that communication.

Knowing ports helps troubleshoot:
- Connectivity issues
- Firewall blocks
- Misconfigured applications

---

## Common Ports You Must Know

| Port | Protocol | Purpose                          | Notes                          |
|------|----------|----------------------------------|--------------------------------|
| 20   | FTP (Data)       | File Transfer Protocol           | Used for sending files        |
| 21   | FTP (Control)    | FTP control channel              | Initiates file transfer        |
| 22   | SSH              | Secure remote login              | Also used for SCP & SFTP       |
| 23   | Telnet           | Unsecure remote access           | Obsolete, replaced by SSH      |
| 25   | SMTP             | Send mail                        | Often blocked on public Wi-Fi  |
| 53   | DNS              | Resolve domain names             | UDP for queries, TCP for zones |
| 67   | DHCP Server      | Assigns IPs                      | Works with port 68             |
| 68   | DHCP Client      | Receives IPs                     | Paired with 67                 |
| 80   | HTTP             | Web traffic (unencrypted)        | Default for web browsers       |
| 110  | POP3             | Retrieve emails                  | Legacy email protocol          |
| 143  | IMAP             | Email sync                       | Used by Gmail & Outlook apps   |
| 443  | HTTPS            | Secure web traffic               | TLS/SSL encryption             |
| 3389 | RDP              | Remote Desktop Protocol          | Windows remote control         |

---

## Mnemonic Trick (FTP, SSH, Telnet…)

**"F**ile, **F**etch, **S**ecure, **T**rusted, **S**ervices":  
- **F**TP → 21  
- **F**TP-Data → 20  
- **S**SH → 22  
- **T**elnet → 23  
- **S**MTP → 25

---

## Real-World Relevance

- Blocked port 443? No HTTPS sites load  
- DNS not working on port 53? You can't resolve names  
- Can’t RDP into a server? Check if port 3389 is open

---

## Quick Reference: Web, Email, Remote

- **Web:**  
  - HTTP → 80  
  - HTTPS → 443

- **Email:**  
  - SMTP → 25  
  - POP3 → 110  
  - IMAP → 143

- **Remote Access:**  
  - SSH → 22  
  - RDP → 3389  
  - Telnet → 23 *(legacy)*

---

## Study Tips

- Make flashcards for port/protocol pairs  
- Draw real-world use cases (e.g., opening Outlook = IMAP/SMTP)  
- Say them out loud to lock in

---

"Know your ports, know your flow. Everything online moves through these doors."

---
