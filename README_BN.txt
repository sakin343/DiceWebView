Dice WebView Android project

এই ZIP-এ Android Studio project source আছে; এটি তৈরি করা APK নয়।

Build করার নিয়ম:
1. PC-তে Android Studio ইনস্টল করুন।
2. Android Studio থেকে এই ZIP extract করা DiceWebView ফোল্ডার Open করুন।
3. Gradle sync শেষ হলে Build > Build Bundle(s) / APK(s) > Build APK(s) চাপুন।
4. APK তৈরি হলে app/build/outputs/apk/debug/app-debug.apk পাওয়া যাবে।

ফিচার:
- https://dice.fm/login WebView
- Italy ডিফল্টসহ country preference dropdown; পছন্দটি ডিভাইসে সেভ থাকে
- Finish task & clear web data এবং Clear web data now বাটন
- WebView cache, cookies, DOM storage, form data ও history clear

সীমাবদ্ধতা:
- Country dropdown শুধু এই wrapper-এ preference সেভ করে। Dice ওয়েবসাইটে country নির্বাচন করাতে হলে Dice-এর নিজস্ব UI/API-তে সেই country সমর্থিত থাকতে হবে।
- ওয়েবসাইটের task completion নির্ভরযোগ্যভাবে শনাক্ত করার কোনো documented signal নেই, তাই ডেটা মুছতে বাটন চাপতে হবে।
- ডেটা clear করলে Dice login session-ও মুছে যেতে পারে।
