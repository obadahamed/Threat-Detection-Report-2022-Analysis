# Trend 09 – RMM Abuse

Attackers increasingly abuse legitimate Remote Monitoring & Management (RMM) tools  
to maintain persistent remote access.

These tools are trusted, signed, and often allowed through firewalls.

---

## 🔥 Common RMM Tools Abused

- AnyDesk  
- Atera  
- ScreenConnect  
- TeamViewer  
- Splashtop  

Attackers install them silently using PowerShell or MSI installers.

---

## 🛡️ Detection Opportunities

### 1. Unexpected RMM Installations
Look for:
msiexec.exe  /i AteraAgent.msi
powershell.exe  -c "Invoke-WebRequest ..."

Code

### 2. Outbound Connections to RMM Servers
Unusual traffic to:
- *.anydesk.com  
- *.screenconnect.com  
- *.atera.com  

### 3. Persistence Mechanisms
RMM tools often create:
- Services  
- Scheduled tasks  
- Registry run keys  

---

## 🎯 MITRE ATT&CK Mapping

- **T1219** – Remote Access Software  
- **T1105** – Ingress Tool Transfer  

---

## 🧪 BTLO Relevance

Labs simulate:
- Silent RMM installation  
- PowerShell-based MSI downloads  
