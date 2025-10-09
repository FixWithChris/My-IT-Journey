# 🧠 Security+ Daily Log — Day 01  
**Week:** 1 — Threats, Attacks, and Vulnerabilities  
**Topic:** Threat Types & Actors  
**Total Study Time:** ≈ 4 h 30 m  

---

## 📘 Gibson Reading
**Chapters:** 1 *Mastering Security Basics* (Threat Overview + CIA Triad) and 6 *Comparing Threats, Vulnerabilities, and Common Attacks* (Threat Actor Types).  

**Key Sections to Note**
- Security control types (preventive, detective, corrective)  
- Threat categories and attack vectors  
- Relationship between actor → motive → capability  

---

## 🎥 Video & Coursework
- **Professor Messer:** Domain 1.1 & 1.2 (Threat Actors + Attack Vectors)  
- **Dion Training:** Threat Actors & Motivations + Quiz  
- **TryHackMe (Optional):** Pre-Security → Cyber Security Fundamentals  

---

## 🧩 Flashcards Created
| Threat Actor | Motive | Capability |
|---------------|---------|-------------|
| Nation-State | Espionage / Political Advantage | APTs, Zero-Days, Advanced Tooling |
| Insider | Financial Gain / Negligence | Legitimate Access, High Impact |
| Hacktivist | Ideological / Social Cause | Moderate to Advanced, Disruption-Focused |
| Script Kiddie | Curiosity / Clout | Limited Tools, Copy-Paste Scripts |

---

## 🎯 Objectives Met
- Identified 5 major threat actor types and their motivations  
- Mapped motive → capability patterns to likely attack vectors  
- Linked Gibson Ch. 1 control types to real-world scenarios  
- Created flashcards and Anki entries for actor profiles  

---

## 🧠 Key Takeaways
- Threat actors are defined by intent more than toolset  
- Nation-states and APTs focus on long-term espionage  
- Hacktivists use symbolic attacks to gain attention  
- Insiders remain the most unpredictable and costly risk  

---

## 🔁 Reflection
Today’s session set a solid foundation for understanding attackers’ mindsets and motivations.  
Tomorrow transitions into **Malware & Delivery Mechanisms (Day 02)** — how those actors weaponize their capabilities.  

---

> “A mind disciplined daily becomes unbreakable.” — *Maestro Journal Entry*


--------------------------------------------------------------------------------------------------------------------
# 🧠 Security+ Daily Log — Day 02  
**Week:** 1 — Threats, Attacks, and Vulnerabilities  
**Topic:** Malware & Delivery Mechanisms  
**Total Study Time:** ≈ 4 h 45 m  

---

## 📘 Gibson Reading
**Chapters:**  
- **Ch. 6 – Comparing Threats, Vulnerabilities, and Common Attacks**  
  - Malware types: Virus, Worm, Trojan, Ransomware, Rootkit, Keylogger, Logic Bomb  
  - Indicators of infection: unusual pop-ups, CPU spikes, altered files  
  - Delivery mechanisms: phishing emails, drive-by downloads, infected USBs  
  - Defensive measures: antivirus, sandboxing, EDR, patching  

**Optional Preview:**  
- **Ch. 7 – Protecting Against Advanced Attacks** → persistence and stealth techniques  

---

## 🎥 Video & Coursework

### Professor Messer (YouTube — Current SY0-701 Playlist)
> Search inside playlist for “malware” to jump directly to these:
- **Malware Types** (~13 min)  
- **Malware Delivery Methods** (~11 min)  
- **Malware Indicators** (~10 min)  
- *(Optional)* **Malware Prevention and Removal** (~12 min)

### Dion Training (Udemy)
- **Types of Malware** (~10 min)  
- **Common Delivery Mechanisms** (~10 min)  
- **Malware Indicators and Symptoms** (~12 min)  
- **Quiz – Malware and Delivery Mechanisms** (~5 min)

### Optional Lab
- **TryHackMe:** *Malware Intro Room* → Identify signatures and sandbox analysis.  
  *(Alternative: run a Defender Offline Scan inside your Windows VM.)*

---

## 🧩 Flashcards Created
| Malware | Delivery Mechanism | Indicator | Defense |
|----------|--------------------|------------|----------|
| **Virus** | Email attachment | File corruption | Antivirus, sandbox testing |
| **Worm** | Network propagation | Network congestion | Segmentation, firewall |
| **Trojan** | Fake installer | Unknown process | Application whitelisting |
| **Ransomware** | Phishing, drive-by | Files encrypted | Backups, user training |
| **Rootkit** | Privilege escalation | Hidden processes | Secure boot, EDR |
| **Spyware / Keylogger** | Malicious link | Strange keystroke lag | Anti-spyware tools |

---

## 🎯 Objectives Met
- Classified major malware categories and how they spread  
- Recognized behavioral indicators of infection  
- Practiced mapping malware → delivery → defense  
- Completed Dion quiz (80 %+ target)  
- Updated Anki deck with six malware archetypes  

---

## 🧠 Key Takeaways
- Malware is *software with intent*; delivery mechanisms exploit user trust  
- Rootkits and worms emphasize stealth and self-propagation  
- Layered defense (EDR + awareness + least privilege) is strongest  
- Training users remains the cheapest prevention  

---

## 🔁 Reflection
Understanding how malware enters and operates connects Day 1’s threat actors to their tools.  
Tomorrow’s focus: **Social Engineering & Human Exploitation (Day 03)** — the psychological side of attack delivery.  

---

> “Control systems. Control access. Control yourself.”
>
> ---------------------------------------------------------------------------------------------------------------------------

# 🧠 Security+ Daily Log — Day 03  
**Week:** 1 — Threats, Attacks, and Vulnerabilities  
**Topic:** Social Engineering & Human Exploitation  
**Total Study Time:** ≈ 4 h 30 m  

---

## 📘 Gibson Reading
**Chapters:**  
- **Ch. 6 – Comparing Threats, Vulnerabilities, and Common Attacks**  
  - Social-engineering fundamentals: influence, urgency, authority  
  - Common techniques: phishing, spear phishing, pretexting, baiting, tailgating, shoulder surfing  
  - Defenses: awareness training, verification procedures, technical controls (email filters, MFA)

**Optional Preview:**  
- **Ch. 11 – Implementing Policies to Mitigate Risks** → Awareness program development & user training frameworks  

---

## 🎥 Video & Coursework  

### Professor Messer (YouTube — Current SY0-701 Playlist)  
Search within playlist for **“social engineering”** or **“phishing”**; you’ll find:  
- **Social Engineering Attacks** (~14 min)  
- **Phishing and Vishing** (~9 min)  
- **Smishing and Spear Phishing** (~8 min)  
- **Business Email Compromise (BEC)** (~7 min)  
- *(Optional)* **Social Engineering Defense and Training** (~10 min)  

### Dion Training (Udemy)  
- *Social Engineering Concepts* (~12 min)  
- *Types of Phishing and Fraud* (~10 min)  
- *Human Behavior and Psychological Triggers* (~8 min)  
- *Quiz – Social Engineering* (~5 min)

### Optional Lab  
- **TryHackMe:** *Phishing Room* → Explore baiting & payload delivery  
- Or analyze a sample phishing email header in your VM  

---

## 🧩 Flashcards Created  
| Technique | Psychological Trigger | Example | Defense |
|------------|----------------------|----------|----------|
| **Phishing** | Urgency | Fake invoice email | Email filtering, training |
| **Spear Phishing** | Personalization / Trust | Targeted exec email | MFA, verification policy |
| **Pretexting** | Authority | “IT Support needs your password” | Callback verification |
| **Tailgating** | Courtesy | Piggybacking through door | Badge policy, awareness |
| **Baiting** | Curiosity | USB labeled “Salary Data” | Endpoint control |
| **Vishing / Smishing** | Fear or Greed | Fake bank call / text | User education, reporting |

---

## 🎯 Objectives Met  
- Defined and compared key social-engineering tactics  
- Linked psychological principles to technical delivery methods  
- Mapped defenses (technical + training) to each attack type  
- Completed Dion quiz (≥ 80 %) and flashcard set  

---

## 🧠 Key Takeaways  
- The weakest link is almost always human behavior  
- Awareness training is a technical control in human form  
- Phishing remains the #1 initial access vector in breaches  
- Politeness and urgency are the most exploited emotions  

---

## 🔁 Reflection  
Social engineering turns psychology into a weapon. By understanding the emotions behind each attack, I can better anticipate how they penetrate technical defenses.  
Tomorrow’s focus: **Application & Web Attacks (Day 04)** — how code and inputs are manipulated instead of people.  

---

> “The mind that cannot be fooled cannot be controlled.” 
