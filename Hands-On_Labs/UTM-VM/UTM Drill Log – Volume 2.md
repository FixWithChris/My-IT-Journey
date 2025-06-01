### 🔧 UTM Drill Log – Volume 2

**Date:** 2025-05-31  
**System:** Windows 11 ARM – UTM 4.6.5  

#### ✅ Drill Summary:
- Explored core system tools (msconfig, regedit, services.msc)
- Practiced net diagnostic commands (ping, tracert, nslookup)
- Ran system scans (SFC, DISM)
- Reviewed Device Manager + Windows Security settings

#### 🔍 Screenshots:
- [x] ipconfig
- [x] services.msc
- [x] msinfo32
- [x] Event Viewer logs

#### 💭 Notes:
- Key finding: Registry and startup config are crucial in slow boot troubleshooting.
- DISM found no corruption; VM integrity confirmed.


### Issue: DNS Fail Caused Stuck nslookup Prompt
- Cause: DNS timeout led to interactive `nslookup` shell without prompt
- Fix: Typed `exit` to regain PowerShell prompt
- Lesson: `nslookup` doesn’t auto-exit on DNS failure; it enters manual mode
