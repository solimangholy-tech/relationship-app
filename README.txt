Relationship — نسخة أندرويد (APK)
===================================

المتطلبات (على جهازك، مش هنا):
1) ثبّت Node.js من nodejs.org
2) ثبّت Android Studio من developer.android.com/studio
   (بيجيب معاه Android SDK و Java اللي محتاجينهم)

خطوات البناء:
    npm install
    npx cap add android
    npx cap sync android
    npx cap open android

هيفتح Android Studio تلقائي. من جوه:
    Build > Build Bundle(s) / APK(s) > Build APK(s)

هتلاقي ملف APK جاهز للتركيب في:
    android/app/build/outputs/apk/debug/app-debug.apk

لو عايز تنزّله على Google Play لازم توقّعه (signed release)
بدل النسخة التجريبية دي — Android Studio بيوضح الخطوات
من قايمة Build > Generate Signed Bundle / APK.

الأيقونة: استبدل صور icon-512.png و icon-192.png بنفس
الأسماء لو عدّلتها، وبعدين npx cap sync android تاني.

ملاحظة: www/index.html هو نفس التطبيق. أي تعديل في نموذج
الدردشة، انسخه هنا قبل البناء.
