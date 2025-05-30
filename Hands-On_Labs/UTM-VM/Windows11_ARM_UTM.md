# 🖥️ UTM + Windows 11 ARM Installation Guide (M2 Mac)

## 🔧 Requirements

- ✅ UTM (v4.6.5 recommended)
- ✅ Windows 11 ARM VHDX (Dev or Canary channel)
- ✅ Apple Silicon Mac (M1/M2/M3)
- ✅ ~25 GB Free Storage
- ✅ Stable Internet Connection

---

## 📦 Step 1: Download the Essentials

### ➤ UTM
[https://mac.getutm.app](https://mac.getutm.app)

### ➤ Windows 11 ARM (VHDX format)
- Sign up: [https://insider.windows.com](https://insider.windows.com)
- Download: **Canary or Dev**, format: **VHDX**, arch: **ARM64**

---

## 🛠️ Step 2: Set Up the VM in UTM

1. **Open UTM**, click ➕ → **Virtualize** → **Windows**
2. Name your VM
3. Select:
   - **Architecture**: ARM64 (aarch64)
   - **System**: UEFI Boot
4. Skip ISO — click **Continue**

---

## 💾 Step 3: Add the Drives

1. **Create a New Drive**
   - Interface: `NVMe`
   - Size: `64 GB` or more
   - Type: `Disk`

2. **Import the VHDX File**
   - Add existing drive → Select your `.vhdx`
   - Interface: `NVMe` (if available)
   - Type: `Removable` or `Disk`

3. Move your empty drive **above** the VHDX if needed (boot priority order)

---

## ⚙️ Step 4: Configure VM Settings

- **Memory**: 4–8 GB
- **CPU Cores**: 4+
- **Display**: Metal (Enable Display Acceleration)
- **Input**: Enable Clipboard Sharing
- **Network**: Shared Network (Emulated)

---

## 🚀 Step 5: Boot + Setup

- Start the VM
- Windows should boot from the VHDX image
- Go through setup steps:
  - Choose language/region
  - Skip Wi-Fi or log in offline
  - Skip Microsoft account if possible
- Setup should complete and land you on the desktop

---

## 🧰 Step 6: Optional Guest Tools

- UTM Guest Tools ISO (for scaling and clipboard)
  - Mount it (if download available)
  - Or manually transfer drivers via USB shared folder

---

## 🧱 Step 7: Take a Snapshot (Optional)

1. Shut down VM
2. Right-click the VM → **Manage Snapshots**
3. Click **Take Snapshot**, name it: “Fresh Install”

---

## 📦 Example Post-Setup Commands

```powershell
winget install Google.Chrome
systeminfo
