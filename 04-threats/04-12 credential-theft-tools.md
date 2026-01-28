# Threat: Credential Theft Tools

سرقة الحسابات هي قلب كل هجوم.  
أشهر الأدوات:
- Mimikatz
- Rubeus
- LaZagne
- SharpHound (BloodHound)

---

## 🔥 ماذا تفعل؟
- سرقة NTLM hashes
- استخراج كلمات السر من الذاكرة
- Kerberoasting
- DCSync
- AD enumeration

---

## 🔥 سلوك مميز
- LSASS access
- rundll32 → comsvcs.dll MiniDump
- unusual Kerberos traffic
- AD enumeration queries

---

## 🛡️ Detection
- مراقبة LSASS access
- مراقبة MiniDump behavior
- مراقبة Kerberos anomalies
- مراقبة AD enumeration

---

## 🧪 BTLO Relevance
- LSASS dump
- Kerberoasting
- AD enumeration simulation
