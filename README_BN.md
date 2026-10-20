# Maruf AI Assistant — প্রাথমিক Android প্রজেক্ট

## এই সংস্করণে যা কাজ করে
- ফোনের ফাইল পিকার থেকে ভিডিও বেছে নেওয়া
- গল্পের বিষয় লিখে টাইটেল/ডেসক্রিপশন/হ্যাশট্যাগের একটি প্রাথমিক খসড়া তৈরি
- তৈরি করা লেখা Android Share মেনু দিয়ে কপি/শেয়ার
- YouTube অ্যাপ খোলা

## যা এখনো নেই
- প্রকৃত AI API সংযোগ (খরচহীন অফলাইন জেনারেটর নয়, শুধু টেমপ্লেট)
- ভিডিও কাটিং/রেন্ডারিং ও স্বয়ংক্রিয় সাবটাইটেল
- সরাসরি YouTube API আপলোড ও OAuth অনুমোদন
- স্বয়ংক্রিয় থাম্বনেইল তৈরি

## মোবাইল থেকে APK তৈরি
1. GitHub-এ একটি নতুন **public** repository তৈরি করো (কোনো পাসওয়ার্ড বা API key যোগ করবে না)।
2. এই ফোল্ডারের ফাইলগুলো repository-তে আপলোড করে `main` branch-এ commit করো।
3. Repository-র **Actions** ট্যাব খুলে `Build Maruf AI Assistant APK` workflow চালাও। Push করলেও workflow চলবে।
4. Workflow সফল হলে run-এর নিচের **Artifacts** থেকে `Maruf-AI-Assistant-debug-apk` ডাউনলোড করে ZIP extract করো।
5. `app-debug.apk` নিজের ফোনে ইনস্টল করো। Android জিজ্ঞেস করলে কেবল নিজের তৈরি করা APK-র জন্য অনুমতি দেবে।

GitHub Actions-এর public repository-তে standard runner ব্যবহার সাধারণত বিনা খরচে করা যায়; সীমা ও নীতি বদলাতে পারে।

## সতর্কতা
- এই debug APK শুধু পরীক্ষার জন্য। এটি এখনো পূর্ণাঙ্গ বা প্রকাশযোগ্য অ্যাপ নয়।
- Google password, OAuth client secret, API key বা access token source code/repository-তে রেখো না।
- YouTube-এ সরাসরি আপলোড যোগ করতে OAuth 2.0 এবং YouTube Data API সেটআপ/পরীক্ষা দরকার।
