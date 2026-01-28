# Threat: Cobalt Strike Forks

بعد تسريب نسخة من Cobalt Strike، ظهرت نسخ معدّلة (Forks) يستخدمها المهاجمون لأنها:
- مجانية
- صعبة الكشف
- قابلة للتعديل

أمثلة:
- Vengeance
- Manjusaka
- Viper
- Geacon (macOS)

---

## 🔥 ماذا تفعل؟
- Implant (agent)
- C2 communication
- Process injection
- Lateral movement
- Credential dumping

---

## 🔥 سلوك مميز
- Named Pipes مختلفة
- Traffic patterns غير مألوفة
- DLL sideloading
- PowerShell encoded

---

## 🛡️ Detection
- مراقبة process injection
- مراقبة Named Pipes غير معتادة
- تحليل C2 traffic
- مراقبة DLL sideloading

---

## 🧪 BTLO Relevance
- beacon-like traffic
- process injection simulation
