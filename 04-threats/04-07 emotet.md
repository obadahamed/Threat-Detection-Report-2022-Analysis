# Threat: Emotet

Emotet كان واحدًا من أشهر وأخطر البرمجيات الخبيثة المستخدمة للدخول الأولي، والانتشار داخل الشبكات، وتنزيل أدوات إضافية مثل Qbot وIcedID وCobalt Strike.

---

## 🔥 كيف يدخل Emotet؟
- رسائل بريد تحتوي Word/Excel macros
- ملفات ZIP
- روابط لمواقع مزيفة
- Reply-chain hijacking (الرد على محادثات بريد حقيقية)

---

## 🔥 ماذا يفعل؟
- إنشاء Persistence
- سرقة كلمات السر وCookies
- انتشار عبر SMB
- تنزيل Loaders إضافية
- نشر Cobalt Strike لاحقًا

---

## 🔥 سلوك مميز
- Word → PowerShell
- PowerShell encoded
- DLL execution via rundll32
- اتصالات HTTP/HTTPS مشبوهة

---

## 🛡️ Detection
- مراقبة تشغيل PowerShell من Office
- كشف PowerShell encoded
- مراقبة rundll32 loading DLLs
- مراقبة SMB lateral movement

---

## 🧪 BTLO Relevance
- malicious macros
- encoded PowerShell
- DLL execution
