# Trend 02 – Supply Chain Compromise

Supply chain attacks increased significantly, targeting software vendors, MSPs, and  
open-source ecosystems. Attackers compromise one provider to reach thousands of victims.

---

## 🔥 Key Examples

### 1. SolarWinds
Backdoored DLL inside a legitimate update.

### 2. Kaseya VSA
Zero-day exploited → MSP → mass ransomware deployment.

### 3. NPM Package Hijacking
Compromised developer accounts → malicious packages.

### 4. Log4j
Critical RCE vulnerability affecting thousands of applications.

---

## 🛡️ Detection Opportunities

- Monitor for **unexpected outbound connections** from servers  
- Detect **web shells** dropped after exploitation  
- Track **process spawning** from web server processes  
- Watch for **mass authentication failures**  

---

## 🎯 MITRE ATT&CK Mapping

- **T1195** – Supply Chain Compromise  
- **T1190** – Exploit Public-Facing Application  
- **T1505.003** – Web Shell  

---

## 🧪 BTLO Relevance
Labs often simulate:
- Log4j exploitation  
- Web shell deployment  
- Lateral movement after initial compromise  

