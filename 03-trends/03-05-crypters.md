# Trend 05 – Crypters-as-a-Service

Attackers increasingly use crypters to evade detection.  
Crypters obfuscate malware to bypass EDR.

---

## 🔥 Indicators of Crypter Usage

- Highly obfuscated PowerShell  
- Base64 + XOR combinations  
- Small EXE files with unusual entropy  
- Suspicious DLL side-loading  

---

## 🛡️ Detection Opportunities

- Detect encoded PowerShell  
- Monitor for LOLBIN abuse  
- Track anomalous DLL loads  

---

## 🎯 MITRE ATT&CK Mapping

- **T1027** – Obfuscated Files or Information  

---

## 🧪 BTLO Relevance
Many labs include:
- Encoded PowerShell  
- Obfuscated loaders  

