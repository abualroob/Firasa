# مرآة الفراسة · Mirror of Firasa

موقع ثابت (HTML فقط) لا يحتاج خادمًا ولا مفتاح API ولا رصيد Claude. تحليل الوجه يجري في متصفح الزائر بنموذج MediaPipe Face Landmarker (Google، رخصة Apache 2.0)، والصورة لا تغادر الجهاز.

## النشر مجانًا
ارفع محتوى هذا المجلد كما هو إلى أي استضافة ملفات ثابتة:
- GitHub Pages: أنشئ مستودعًا، ارفع الملفات، ثم Settings ← Pages ← Deploy from branch.
- Netlify أو Cloudflare Pages: اسحب المجلد إلى صفحة النشر.

لا بد أن يُفتح الموقع عبر http(s)، لا بفتح index.html مباشرة من الجهاز.

## الملفات
- index.html: الموقع كاملًا (الواجهة، قواعد الرازي، القراءة، البطاقة، PDF).
- vendor/: مكتبة @mediapipe/tasks-vision 0.10.14 وملفات wasm.
- models/face_landmarker.task: نموذج قياس الوجه (float16).
