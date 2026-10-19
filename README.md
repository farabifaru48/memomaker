# Memo Maker (মেমো মেকার)

A free, simple memo / invoice maker for small shops. Works in the browser, no login, no server.
ছোট দোকানের জন্য ফ্রি মেমো / ইনভয়েস তৈরির টুল। ব্রাউজারেই চলে, লগইন বা সার্ভার লাগে না।

**Live demo / লাইভ লিংক:** https://USERNAME.github.io/memo-maker/

## Features / সুবিধা

- Make a memo in seconds: items, quantity, price, discount, delivery charge, paid and due
- Download as a real **A4 PDF** and **share** it to WhatsApp, Messenger or any app
- Save your business name, address, phone and **logo**; keep more than one business
- Two memo designs (Classic and Card) with your own color
- Default note that fills in every new memo
- Every memo is saved on your device; find past memos by memo number, customer name or date
- Bangla and English interface

---

- মুহূর্তেই মেমো: পণ্য, পরিমাণ, দাম, ডিসকাউন্ট, ডেলিভারি চার্জ, পরিশোধ ও বাকি
- আসল **A4 PDF** ডাউনলোড এবং WhatsApp, Messenger বা যেকোনো অ্যাপে **শেয়ার**
- প্রতিষ্ঠানের নাম, ঠিকানা, ফোন ও **লোগো** সেভ থাকে; একাধিক প্রতিষ্ঠান রাখা যায়
- ক্লাসিক ও কার্ড, দুই ডিজাইন, নিজের পছন্দের রং
- ডিফল্ট নোট, যেটা প্রতিটা নতুন মেমোতে নিজে থেকে বসে
- প্রতিটা মেমো ডিভাইসে সেভ হয়; মেমো নম্বর, কাস্টমারের নাম বা তারিখ দিয়ে পুরনো মেমো খোঁজা যায়
- বাংলা ও English ইন্টারফেস

## How to use / ব্যবহারের নিয়ম

1. Open the live link. / লাইভ লিংক খুলুন।
2. Fill in your business details once (and add a logo). / প্রতিষ্ঠানের তথ্য একবার দিন (চাইলে লোগো দিন)।
3. Add the customer and items. / কাস্টমার ও পণ্য যোগ করুন।
4. Tap **Download PDF** or **Share**. / **PDF ডাউনলোড** বা **শেয়ার** চাপুন।
5. Find old memos from the three-dot menu at the top. / উপরের তিন ডট মেনু থেকে পুরনো মেমো খুঁজুন।

## Privacy / গোপনীয়তা

Everything is stored only in your own browser (localStorage). Nothing is uploaded to any server.
Clearing the browser data, or opening the app on another phone or computer, will not bring the data along.

সব তথ্য শুধু আপনার ব্রাউজারে সেভ থাকে, কোনো সার্ভারে যায় না।
ব্রাউজারের ডেটা মুছলে বা অন্য ফোন বা কম্পিউটারে খুললে তথ্য পাওয়া যাবে না।

## Run it yourself / নিজে চালান

It is a single `index.html` file. Download it and open it in a browser, or host it with GitHub Pages.
PDF creation needs an internet connection (it loads html2canvas and jsPDF from a CDN).

এটা একটাই `index.html` ফাইল। ডাউনলোড করে ব্রাউজারে খুলুন, অথবা GitHub Pages-এ হোস্ট করুন।
PDF বানাতে ইন্টারনেট লাগে।

## Built with

Plain HTML, CSS and JavaScript. [html2canvas](https://html2canvas.hertzen.com/) and [jsPDF](https://github.com/parallax/jsPDF) for PDF.

## License

MIT
