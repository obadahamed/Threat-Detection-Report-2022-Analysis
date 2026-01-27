# Trend 03 – Vulnerabilities

High-impact vulnerabilities in enterprise platforms were heavily exploited, especially  
in Exchange, VMware Horizon, Citrix, and SonicWall.

---

## 🔥 Key Observations

- Attackers rapidly weaponize new CVEs  
- Web shells are commonly dropped after exploitation  
- Vulnerabilities often lead to ransomware deployment  

---

## 🛡️ Detection Opportunities

### 1. Web Server Spawning CMD/PowerShell

w3wp.exe  → cmd.exe
w3wp.exe  → powershell.exe


### 2. Suspicious File Drops
- *.aspx  
- *.jsp  
- *.php  

### 3. Outbound C2 Traffic
Unexpected connections from servers.

---

## 🎯 MITRE ATT&CK Mapping

- **T1190** – Exploit Public-Facing Application  
- **T1505.003** – Web Shell  

---

## 🧪 BTLO Relevance
Many labs simulate:
- ProxyShell  
- ProxyLogon  
- Web shell exploitation  

