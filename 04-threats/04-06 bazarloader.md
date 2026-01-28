# Threat: BazarLoader / BazarCall

BazarLoader هو loader متطور جدًا، بينما BazarCall يعتمد على الهندسة الاجتماعية عبر الهاتف لخداع المستخدم.

---

## 🔥 كيف يدخل؟
### BazarLoader:
- LNK
- Office documents
- JS
- ZIP

### BazarCall:
- Email → رقم هاتف
- المستخدم يتصل
- "الدعم الفني" يطلب تنزيل ملف
- الملف يحتوي loader

---

## 🔥 ماذا يفعل؟
- Persistence
- اتصال C2
- تنزيل Cobalt Strike
- انتشار داخل الشبكة
- تمهيد الطريق للرنسوموير

---

## 🔥 سلوك مميز
- LNK → PowerShell
- DLL via rundll32
- اتصالات HTTPS جديدة
- ملفات EXE بأسماء شرعية

---

## 🛡️ Detection
- مراقبة LNK execution
- مراقبة rundll32
- مراقبة C2 traffic
- مراقبة scheduled tasks

---

## 🧪 BTLO Relevance
- malicious LNK
- loader → beacon chain
- social engineering simulation
