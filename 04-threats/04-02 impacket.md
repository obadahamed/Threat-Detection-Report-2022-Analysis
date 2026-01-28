# Threat: Impacket

Impacket هي مجموعة أدوات Python تُستخدم بكثافة في الهجمات الحديثة، خصوصًا في lateral movement وسرقة الحسابات.

---

## 🔥 أدوات Impacket المهمة
- psexec.py → تنفيذ أوامر عبر SMB
- wmiexec.py → تنفيذ أوامر عبر WMI
- smbexec.py → تنفيذ أوامر عبر SMB
- secretsdump.py → سرقة NTLM hashes و SAM
- ntlmrelayx.py → تنفيذ NTLM Relay

---

## 🔥 سلوك مميز
- SMB traffic غير طبيعي
- إنشاء خدمات جديدة (service installation)
- تنفيذ أوامر مثل:
cmd.exe  /c whoami

Code
- سرقة بيانات من SAM أو LSASS

---

## 🛡️ Detection
- Event ID 7045 (Service Installed)
- SMB connections بين أجهزة غير معتادة
- WMI execution logs
- NTLM relay patterns

---

## 🧪 BTLO Relevance
- lateral movement simulation
- secretsdump behavior
- psexec activity
