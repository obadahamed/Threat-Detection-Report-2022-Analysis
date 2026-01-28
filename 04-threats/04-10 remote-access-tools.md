# Threat: Remote Access Tools (RATs)

المهاجمون يستخدمون أدوات شرعية للتحكم عن بُعد لأنها:
- signed
- trusted
- firewall-friendly

أمثلة:
- NetSupport Manager
- AnyDesk
- Atera
- ScreenConnect
- AsyncRAT (خبيث)
- QuasarRAT

---

## 🔥 كيف تدخل؟
- Phishing
- Fake installers
- PowerShell download
- Silent MSI installation

---

## 🔥 سلوك مميز
- تثبيت صامت (silent install)
- إنشاء خدمات جديدة
- اتصالات خارجية مستمرة
- Persistence عبر registry أو scheduled tasks

---

## 🛡️ Detection
- مراقبة MSI silent installs
- مراقبة outbound connections
- مراقبة إنشاء الخدمات
- مراقبة PowerShell download commands

---

## 🧪 BTLO Relevance
- silent MSI install
- RAT behavior simulation
