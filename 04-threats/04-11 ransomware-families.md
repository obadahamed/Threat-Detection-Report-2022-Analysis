# Threat: Ransomware Families

الرنسوموير اليوم ليس مجرد "تشفير ملفات"، بل عملية كاملة تشمل:
- سرقة بيانات
- تعطيل EDR
- نشر Cobalt Strike
- lateral movement
- تشفير الملفات
- ابتزاز الضحية

أشهر العائلات:
- Black Basta
- LockBit
- Royal
- ALPHV/BlackCat

---

## 🔥 سلوك مميز
- PsExec لنشر ransomware
- حذف shadow copies
- تعطيل Windows Defender
- تشفير الملفات بسرعة
- اتصالات خارجية قبل التشفير

---

## 🛡️ Detection
- مراقبة PsExec activity
- مراقبة حذف shadow copies
- مراقبة تعطيل AV
- مراقبة عمليات التشفير السريعة

---

## 🧪 BTLO Relevance
- ransomware simulation
- PsExec lateral movement
