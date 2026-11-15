# Favorite Shop BD — আপডেট করা ওয়েবসাইট প্রোটোটাইপ

## চালু করার নিয়ম
1. ZIP ফাইলটি Extract করুন।
2. `index.html` খুললে Customer Website দেখা যাবে।
3. `admin.html` খুলে Admin Panel ব্যবহার করুন। প্রথমবার কমপক্ষে ৮ অক্ষরের একটি পাসওয়ার্ড তৈরি করে আবার লগইন করুন।

## এই সংস্করণে যোগ/সংশোধন করা হয়েছে
- Favorite Shop BD-এর About Us, পণ্য পরিচিতি, Why Choose Us, Contact Information ও Customer Support।
- Facebook Page এবং WhatsApp লিংক।
- পণ্যের Discount Percentage, পুরোনো দাম ও ছাড়ের দাম দেখানো।
- Admin Panel-এ Product Add, Edit, Delete, Active/Inactive, Stock ও Discount নিয়ন্ত্রণ।
- হোমপেজে একটি নিজস্ব ব্যানার বিজ্ঞাপন যোগ/সম্পাদনা/বন্ধ/মুছে ফেলার ব্যবস্থা।
- কাস্টমার রিভিউ জমা, Admin Approval/Delete এবং সর্বোচ্চ ৫০টি অনুমোদিত রিভিউ দেখানো।
- Checkout-এ Cash on Delivery, bKash, Nagad ও Rocket (ম্যানুয়াল) অপশন এবং Transaction ID ইনপুট।
- Admin Panel-এ ম্যানুয়াল পেমেন্ট নম্বর সংরক্ষণের ফিল্ড।
- আইকন ও বাটনে hover/focus color effect এবং বানান/কনটেন্ট সংশোধন।

## গুরুত্বপূর্ণ সীমাবদ্ধতা — লাইভ করার আগে পড়ুন
এই ZIP এখনো একটি front-end prototype। পণ্য, অর্ডার, রিভিউ, বিজ্ঞাপন ও Admin password ব্রাউজারের `localStorage`-এ থাকে। ফলে এগুলো একই ব্রাউজার/ডিভাইসের মধ্যে সীমাবদ্ধ; ভিন্ন ক্রেতার ডিভাইস থেকে আসা অর্ডার স্বয়ংক্রিয়ভাবে আপনার Admin Panel-এ পৌঁছাবে না। নিরাপদ Admin Login, সকল ডিভাইসে ডেটা শেয়ার, প্রকৃত অর্ডার সংরক্ষণ ও স্টক সিঙ্কের জন্য backend/database প্রয়োজন।

**Payment Gateway এখনো সক্রিয় নয়।** bKash/Nagad/Rocket অপশনগুলো ম্যানুয়াল পেমেন্ট নির্দেশনা ও Transaction ID সংগ্রহের জন্য। স্বয়ংক্রিয় পেমেন্ট যাচাই চালু করতে অনুমোদিত Merchant Account, Gateway API credentials, HTTPS এবং নিরাপদ server-side integration লাগবে। API secret কখনো HTML/JavaScript বা Admin Panel-এর localStorage-এ রাখবেন না এবং চ্যাটে পাঠাবেন না।

বিজ্ঞাপন ফিচারটি আপনার নিজস্ব ব্যানার বিজ্ঞাপন দেখায়; Google AdSense বা অন্য তৃতীয় পক্ষের বিজ্ঞাপন নেটওয়ার্ক সংযুক্ত নয়।

## প্রকাশের আগে যাচাই করুন
- পণ্যের আসল দাম, ছবি, বর্ণনা, স্টক ও ডেলিভারি চার্জ বসান।
- bKash/Nagad/Rocket-এর সঠিক Merchant নম্বর Admin Panel-এ দিন।
- ব্যবসার ঠিকানা, ফোন ও নীতিমালা যাচাই করুন।
- Hosting/domain-এ আপলোডের পর HTTPS চালু করুন।
- লাইভ ব্যবহারের আগে backend/database ও নিরাপদ authentication সংযুক্ত করুন।
