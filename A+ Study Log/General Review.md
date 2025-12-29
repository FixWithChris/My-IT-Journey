# Study Session Summary — Networking, Hardware, Displays, & Input Devices

---

## 1. Firewalls

### What a Firewall Is
- First line of defense for a network
- Monitors **incoming and outgoing traffic**
- Uses predefined rules to **allow or block traffic**

### Firewall Types
#### Hardware Firewall
- Physical device or built into routers
- Protects the **entire network**

#### Software Firewall
- Installed on individual computers or servers
- Protects **specific devices**

### Key Capabilities
- Blocks unauthorized access
- Allows trusted traffic (web browsing, email)
- Detects and prevents attacks:
  - Malware
  - Port scanning

### Next-Generation Firewalls (NGFW)
- Common in business environments
- Include:
  - Deep Packet Inspection (DPI)
  - Intrusion Prevention Systems (IPS)

---

## 2. Power over Ethernet (PoE)

### What PoE Does
- Sends **power and data over a single Ethernet cable**
- Simplifies installation and cable management

### Common Uses
- IP cameras
- VoIP phones
- Wireless access points

### PoE Standards
| Standard | IEEE | Max Power |
|-------|------|-----------|
| PoE | 802.3af | 15.4 W |
| PoE+ | 802.3at | 25.5 W |
| PoE++ | 802.3bt | 60–100 W |

---

## 3. Internet Connection Types

### Cable Internet
- Uses **coaxial cable**
- Requires a **cable modem**
- Based on **DOCSIS**
  - DOCSIS 3.0, 3.1, newer = faster speeds
- Not compatible with DSL or fiber

### DSL (Digital Subscriber Line)
- Uses existing **telephone lines (copper)**
- Allows phone and internet simultaneously
- Uses unused high-frequency bands

#### Types of DSL
- **ADSL**: Faster download than upload
- **VDSL**: Higher speeds over shorter distances

### Cable vs DSL
- Cable: Faster, better bandwidth
- DSL: Often only option in rural/older areas
- DSL signal degrades over distance

---

## 4. Touchscreen & Digitizer

### Touchscreen
- Detects **finger input**

#### Capacitive Touchscreens
- Most common today
- Uses electrical conductivity of the human body
- Highly responsive
- Supports multi-touch gestures
- Limited glove support

#### Resistive Touchscreens
- Detect pressure between layers
- Works with gloves, stylus, any object
- Less sensitive
- No multi-touch
- Common in industrial/medical use

### Digitizer
- Detects **stylus input**
- Enables precision drawing and handwriting
- Separate component from touchscreen
- Common in tablets and 2-in-1 laptops

---

## 5. Display Attributes

### Pixel Density (PPI)
- Pixels per inch
- Higher PPI = sharper image
- Same resolution on smaller screen = higher PPI

### Refresh Rate (Hz)
- Screen updates per second

#### Practical Targets
- Office / Browsing → **60 Hz**
- Movies / Streaming → **60 Hz**
- Casual Gaming → **75–120 Hz**
- Competitive Gaming → **144–240 Hz**

### Screen Resolution
| Name | Resolution |
|----|-----------|
| HD | 1280×720 |
| Full HD | 1920×1080 |
| QHD | 2560×1440 |
| 4K | 3840×2160 |
| 8K | 7680×4320 |

> Resolution ≠ screen size

### Color Gamut
- Range of colors displayed

#### Standards
- sRGB → Web, general use
- Adobe RGB → Photography/design
- DCI-P3 → HDR, modern smartphones

---

## 6. Display Panel Technologies

### LCD Panel Types
- **TN**
  - Fast response
  - Cheap
  - Poor color and viewing angles
  - Competitive gaming

- **IPS**
  - Excellent color accuracy
  - Wide viewing angles
  - Productivity & creative work

- **VA**
  - Best contrast among LCDs
  - Deeper blacks
  - Slower response than TN

### OLED
- Self-emitting pixels
- True blacks, infinite contrast
- Vibrant colors
- Burn-in risk

### Mini-LED
- LCD with advanced backlighting
- Brighter, better contrast than standard LCD
- No burn-in risk

---

## 7. Inverters (Legacy Knowledge)
- Convert DC to AC
- Required for CCFL backlights
- Not used in modern LED displays

---

## 8. Real-World Examples

### Office Laptop
- IPS LCD
- 1080p
- ~300 PPI
- 60 Hz
- sRGB

### Gaming Monitor
- TN panel
- 1080p
- ~82 PPI
- 240 Hz
- Narrow color gamut

### Creative Tablet
- OLED
- High PPI
- 120 Hz
- DCI-P3
- Touchscreen + digitizer

---

## 9. Key Exam Mental Models

- Firewall = traffic control
- PoE = power + data
- Cable vs DSL = medium + distance matters
- Touchscreen ≠ digitizer
- Refresh rate = smoothness
- Resolution = detail
- PPI = sharpness
- Color gamut = color accuracy
- TN = speed | IPS = accuracy | VA = contrast
