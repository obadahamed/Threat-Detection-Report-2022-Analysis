# Trend 04 – Affiliates

Modern ransomware operations rely on **affiliate networks**.  
Different actors handle different stages of the intrusion.

---

## 🔥 Affiliate Roles

- **Initial Access Brokers** – sell access  
- **Malware Loaders** – Qbot, IcedID, Bazar  
- **Ransomware Operators** – Conti, LockBit  
- **Data Exfiltration Teams**  

---

## 🛡️ Detection Opportunities

- Detect loader malware (Qbot, IcedID)  
- Monitor for suspicious DLL loads  
- Track credential dumping activity  

---

## 🎯 MITRE ATT&CK Mapping

- **T1059** – Command Execution  
- **T1105** – Ingress Tool Transfer  

---

## 🧪 BTLO Relevance
Labs often simulate:
- Qbot → Cobalt Strike → Ransomware chain  

