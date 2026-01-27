# Trend 11 – Abusing RPC

Remote Procedure Call (RPC) mechanisms were abused for lateral movement,  
privilege escalation, and domain controller targeting.

---

## 🔥 Key Examples

### 1. PetitPotam
Forces a domain controller to authenticate to an attacker-controlled machine.

### 2. PrintNightmare
Abuses the Print Spooler service for:
- RCE  
- Privilege escalation  
- Lateral movement  

---

## 🛡️ Detection Opportunities

### 1. spoolsv.exe Anomalies
Look for:
- spoolsv.exe spawning cmd.exe  
- spoolsv.exe making outbound connections  

### 2. NTLM Relay Patterns
- Unexpected SMB authentication  
- Anonymous logon attempts  

---

## 🎯 MITRE ATT&CK Mapping

- **T1210** – Exploitation of Remote Services  
- **T1557** – Adversary-in-the-Middle  

---

## 🧪 BTLO Relevance

Labs simulate:
- PrintNightmare exploitation  
- Lateral movement via RPC  
