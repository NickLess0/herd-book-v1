# Herd Book — offline livestock records

Herd Book keeps every record on the phone or computer it is installed on. Nothing is sent to any server or company, and once installed it works with no internet at all.

You put the app files online **once** so people can install it. That web address only hands out the app itself, the way an app store would. Nobody's animals, photos or notes ever go there.

---

## 1. Put the app online (once, free)

The easiest free option is **GitHub Pages**:

1. Create a free account at **github.com**.
2. Click **+** (top right) → **New repository**. Name it `herd-book`, choose **Public**, and click **Create repository**.
3. On the next page click **uploading an existing file**. Drag in everything from this folder: `index.html`, `manifest.webmanifest`, `sw.js` and the `icons` folder. Click **Commit changes**.
4. Open **Settings** → **Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose **main** and **/(root)**, then click **Save**.
5. After a minute or two the page shows your address, for example `https://yourname.github.io/herd-book/`.

Send that address to anyone who should use the app.

Any other static web host, or your own web server, works the same way. The only requirement is that the address starts with `https://`, because phones only install web apps from secure addresses.

## 2. Install on each device

Open the address once while online, then:

| Device | Steps |
|---|---|
| **iPhone / iPad** (Safari) | Tap **Share** (the square with an arrow) → **Add to Home Screen** → **Add** |
| **Android** (Chrome) | Tap the **⋮** menu → **Install app** (or **Add to Home screen**) → **Install** |
| **Windows / Mac PC** (Chrome or Edge) | Click the **install icon** at the end of the address bar → **Install** |

The app also shows these steps on its Home screen until it is installed. After that, open it from the home screen or apps list. It works in airplane mode.

## 3. Keep a backup

Records live only on the device. If a phone is lost, broken or reset, its records go with it. So:

- In **Setup → Backup**, tap **Save backup file**. On phones this opens the share menu, so you can save it to Files, send it to yourself on WhatsApp, or email it. On a PC it downloads a file.
- The backup includes animals, photos, statuses and vaccine records.
- The app reminds you on the Home screen if you haven't saved a backup for 30 days.

To load a backup on a new phone, or on someone else's phone: **Setup → Restore from backup file**. This **replaces** whatever is on that device.

## Sharing one herd between several people

Each device keeps its own records, and they do not sync by themselves. For a shared herd:

- Choose **one person** to keep the main copy and enter changes.
- They send a backup file to the others whenever they want them to see the latest records.
- The others restore it. Restoring replaces their copy, so changes made on their phone since the last restore are lost.

## Moving records from the Claude version

Open the Claude version of Herd Book → **Setup** → **Full backup** to save the file. Then, in the installed app, use **Setup → Restore from backup file**. Full-size photos are not in that file, but the small photos are, and they still show on every animal.

## Trying it on a PC with no hosting

On a computer you can also double-click `index.html` to open it in Chrome or Edge. Records are then saved inside that browser on that computer. It can't be installed to phones this way.

## Updating the app later

Replace the changed files in the same place. Then open `sw.js` and raise the version, for example `herdbook-v1` → `herdbook-v2`. Each device shows **"A new version is ready — Update now"** the next time it opens the app while online. Updating never touches the records.

---

# سجل القطيع — تطبيق يعمل بدون إنترنت

يحفظ التطبيق كل السجلات على الهاتف أو الكمبيوتر المثبت عليه فقط. لا يُرسل أي شيء إلى أي خادم أو شركة، وبعد تثبيته يعمل بدون إنترنت.

تحتاج إلى وضع ملفات التطبيق على الإنترنت **مرة واحدة فقط** ليتمكن الآخرون من تثبيته. هذا العنوان يقدّم التطبيق نفسه فقط، ولا تصل إليه أي بيانات عن الحيوانات أو الصور أو الملاحظات.

## ١. وضع التطبيق على الإنترنت (مرة واحدة، مجاناً)

1. أنشئ حساباً مجانياً في **github.com**.
2. اضغط **+** ← **New repository**، واكتب الاسم `herd-book`، واختر **Public**، ثم **Create repository**.
3. اضغط **uploading an existing file** واسحب كل محتويات هذا المجلد: `index.html` و`manifest.webmanifest` و`sw.js` ومجلد `icons`، ثم **Commit changes**.
4. افتح **Settings** ← **Pages**، واختر **Deploy from a branch** ثم **main** و **/(root)** واضغط **Save**.
5. بعد دقيقة أو دقيقتين يظهر العنوان، مثل: `https://yourname.github.io/herd-book/`

أرسل هذا العنوان لكل من سيستخدم التطبيق.

## ٢. التثبيت على كل جهاز

افتح العنوان مرة واحدة مع وجود إنترنت، ثم:

- **iPhone**: زر المشاركة ← **إضافة إلى الشاشة الرئيسية** ← **إضافة**
- **Android**: قائمة Chrome ‏(⋮) ← **تثبيت التطبيق** ← **تثبيت**
- **الكمبيوتر**: أيقونة التثبيت في طرف شريط العنوان في Chrome أو Edge ← **تثبيت**

## ٣. النسخ الاحتياطي

السجلات موجودة على الجهاز فقط، فإذا ضاع الهاتف أو أُعيد ضبطه تضيع معه.

- من **الإعدادات ← النسخ الاحتياطي** اضغط **حفظ نسخة احتياطية**، واحفظ الملف في مكان آمن، مثل الملفات أو واتساب أو البريد.
- لنقل السجلات إلى هاتف آخر: **الإعدادات ← الاستعادة من نسخة احتياطية**. الاستعادة **تستبدل** كل ما على ذلك الجهاز.

## مشاركة قطيع واحد بين عدة أشخاص

كل جهاز يحتفظ بسجلاته، ولا تتزامن الأجهزة تلقائياً.

- يتولى شخص واحد النسخة الأساسية وإدخال التعديلات.
- يرسل ملف النسخة الاحتياطية للآخرين، وهم يستعيدونه على أجهزتهم.
