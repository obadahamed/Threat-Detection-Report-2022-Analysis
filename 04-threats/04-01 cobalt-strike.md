# Threat: Cobalt Strike

Cobalt Strike هو أداة اختبار اختراق احترافية أصبحت تُستخدم بكثافة من قبل المهاجمين الحقيقيين.  
وجودها داخل الشبكة يعني أن الهجوم وصل مرحلة متقدمة (post-exploitation).

---

## 🔥 ما هو Cobalt Strike؟
منصة هجومية تتضمن:
- Beacon (عميل يتحكم به المهاجم)
- C2 Server
- أدوات post-exploitation
- تقنيات تخفي وإخفاء الاتصالات

---

## 🔥 كيف يدخل؟
عادةً بعد:
- Qbot
- IcedID
- BazarLoader
- Web Shell
- Exploit مثل ProxyShell

---

## 🔥 سلوك مميز
- Process Injection داخل explorer.exe أو rundll32.exe
- استخدام Named Pipes مثل:
\\.\pipe\msagent_***

Code
- PowerShell مشفّر
- اتصالات HTTP/HTTPS أو DNS مشبوهة

---

## 🛡️ Detection
- مراقبة عمليات rundll32 و dllhost
- مراقبة Named Pipes
- كشف PowerShell encoded
- مراقبة الاتصالات الخارجية

---

## 🧪 BTLO Relevance
- Beacon simulation
- Process injection
- C2 traffic
