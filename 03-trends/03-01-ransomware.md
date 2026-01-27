# Trend 01 – Ransomware

Ransomware remained one of the most impactful threats across enterprise environments.  
Adversaries continued to evolve their techniques, focusing on **double extortion**,  
**Ransomware-as-a-Service (RaaS)**, and **affiliate-driven operations**.

---

## 🔥 Key Behaviors

### 1. Double Extortion
Attackers:
- Steal data before encryption  
- Threaten to leak it publicly  
- Then encrypt systems  

This increases pressure on victims to pay.

---

### 2. Ransomware-as-a-Service (RaaS)
Ransomware operators now provide:
- Infrastructure  
- Malware  
- Payment portals  
- Negotiation support  

Affiliates perform the intrusion and get a revenue share.

---

### 3. Pre-Encryption Indicators (Critical for SOC)

#### 🔹 Shadow Copy Deletion
cmd.exe  /c vssadmin delete shadows /all /quiet

Code

#### 🔹 Disable Recovery
wmic shadowcopy delete

Code

#### 🔹 PowerShell Download Cradles
powershell.exe  -nop -w hidden -c IEX(...)

Code

#### 🔹 Lateral Movement
- PsExec  
- RDP  
- SMB  

---

## 🛡️ Detection Opportunities

- Monitor for **shadow copy deletion**  
- Detect **encoded PowerShell**  
- Alert on **credential dumping tools**  
- Track **lateral movement** patterns  

---

## 🎯 MITRE ATT&CK Mapping

- **T1490** – Inhibit System Recovery  
- **T1059** – Command Execution  
- **T1105** – Ingress Tool Transfer  
- **T1021** – Remote Services  

---

## 🧪 BTLO Relevance
Many BTLO labs simulate:
- Pre-encryption activity  
- PowerShell abuse  
- Lateral movement  
- Ransomware staging  
