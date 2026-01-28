# Threat: SocGholish

SocGholish هو تهديد يعتمد على الهندسة الاجتماعية عبر مواقع مخترقة تُظهر للمستخدم "تحديث متصفح" مزيف.

---

## 🔥 كيف يعمل؟
1. اختراق موقع شرعي
2. إضافة JavaScript خبيث
3. عرض صفحة "Update Browser"
4. المستخدم ينزّل ZIP أو JS
5. يبدأ الـ loader
6. يتم تنزيل Cobalt Strike لاحقًا

---

## 🔥 سلوك مميز
- ملفات JS مشفّرة
- ZIP يحتوي JS أو LNK
- PowerShell encoded
- اتصالات HTTP/HTTPS لمواقع جديدة

---

## 🛡️ Detection
- مراقبة WScript و cscript
- كشف PowerShell encoded
- مراقبة ملفات ZIP المشبوهة
- تحليل JavaScript obfuscation

---

## 🧪 BTLO Relevance
- fake browser update simulation
- malicious JS
- loader → beacon chain
