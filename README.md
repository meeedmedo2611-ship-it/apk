# تطبيق التزام الفروع (أندرويد)

## الطريقة 1: بدون تثبيت أي برنامج (GitHub)
1. اعمل حساب مجاني على github.com وأنشئ مستودع جديد (New repository).
2. ارفع كل محتويات هذا المجلد للمستودع، مع مجلد `.github` (Add file ← Upload files).
3. افتح تبويب **Actions** ← **Build APK** ← **Run workflow**، وانتظر 5-10 دقايق.
4. افتح التشغيل الناجح ونزّل **app-debug-apk** من تحت (Artifacts). فك الضغط وانقل `app-debug.apk` لموبايلك.
5. ثبّته (اسمح بالتثبيت من مصدر غير معروف إذا طلب).

## الطريقة 2: على كمبيوترك
المطلوب: Node 18+ وJava 17 وAndroid Studio.
    npm install
    npm run prep
    npx cap add android
    npx cap sync android
    npx cap open android   # ثم Build ← Build APK(s)
