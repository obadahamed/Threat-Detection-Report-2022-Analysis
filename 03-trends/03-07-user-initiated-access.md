# Trend 07 – User-Initiated Initial Access

Many intrusions begin when users unintentionally execute malicious files.  
Attackers rely heavily on social engineering and user curiosity to bypass perimeter defenses.

---

## 🔥 Common Initial Access Vectors

### 1. Cracks & Keygens
Users download:
- "Free" software
- Game cracks
- License generators

These often contain loaders or stealers.

### 2. Fake Installers
Malicious EXE files disguised as:
- Setup.exe
- Update.exe
- Driver installers

### 3. Malicious ZIP Archives
ZIP files containing:
- LNK droppers
- JavaScript malware
- HTA payloads

### 4. SEO Poisoning
Users search for:
- “Free PDF editor”
- “Download VLC”
- “Game mods”

Attackers poison search results with malicious downloads.

---

## 🛡️ Detection Opportunities

- Monitor for **unsigned executables** launched by users  
- Detect **PowerShell spawned from user applications**  
- Alert on **LNK files spawning cmd.exe or powershell.exe**  
- Track **browser → download → execution** chains  

---

## 🎯 MITRE ATT&CK Mapping

- **T1204** – User Execution  
- **T1566** – Phishing (when combined with email delivery)  

---

## 🧪 BTLO Relevance

BTLO labs often simulate:
- Malicious LNK files  
- Fake installers  
- User-triggered malware execution  
