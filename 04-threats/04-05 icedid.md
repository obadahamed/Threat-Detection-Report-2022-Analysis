# Threat: IcedID

IcedID هو loader متطور جدًا يعتمد على HTML smuggling وملفات ZIP لتنفيذ المرحلة الأولى من الهجوم.

---

## 🔥 كيف يدخل؟
- HTML smuggling
- ZIP + JS
- LNK files
- Fake invoices

---

## 🔥 ماذا يفعل؟
- Persistence
- سرقة credentials
- اتصال C2
- تنزيل Cobalt Strike أو ransomware

---

## 🔥 سلوك مميز
- DLL execution via rundll32
- PowerShell encoded
- HTML smuggling artifacts
- اتصالات HTTPS مشبوهة

---

## 🛡️ Detection
- مراقبة rundll32
- مراقبة HTML smuggling
- تحليل PowerShell logs
- مراقبة C2 traffic

---

## 🧪 BTLO Relevance
- malicious HTML
- DLL execution
- loader → beacon chain

