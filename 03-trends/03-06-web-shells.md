# Trend 06 – Common Web Shells

Web shells remain one of the most common post-exploitation tools after exploiting  
public-facing applications.

---

## 🔥 Common Web Shell Families

- China Chopper  
- Godzilla  
- Behinder  

---

## 🛡️ Behavioral Indicators

### 1. Windows IIS Worker Process Spawning certutil.exe
parent == w3wp.exe
&&
command_line_includes (certutil && -split)

Code

This indicates a web shell downloading payloads.

---

### 2. Windows IIS Worker Process Spawning CMD/PowerShell
w3wp.exe  → cmd.exe
w3wp.exe  → powershell.exe

Code

---

### 3. Linux PHP/Java Spawning wget/curl
parent_process == (php || java)
&&
command_line_includes (wget || curl)

Code

---

## 🛠️ TAKE ACTION (SOC Guidance)

- Patch vulnerable web applications  
- Use MSERT for Exchange  
- Inspect ASPX/JSP/PHP file modifications  
- Monitor web server process behavior  
- Block outbound traffic from web servers  

---

## 🎯 MITRE ATT&CK Mapping

- **T1505.003** – Web Shell  
- **T1190** – Exploit Public-Facing Application  

---

## 🧪 BTLO Relevance
Many labs simulate:
- Web shell deployment  
- certutil abuse  
- curl/wget downloads
