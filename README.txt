Kavitha Telecom — PWA App
=====================================================

WHAT'S IN THIS ZIP
-------------------
index.html            -> the app itself
manifest.json         -> makes the app installable (name, icon, colors)
sw.js                 -> service worker, makes the app work fully offline after first load
icon-192.png          -> app icon
icon-512.png          -> app icon (large)
icon-apple-touch.png  -> app icon (iOS)

All 6 files sit in ONE folder — no subfolders. This means you can upload
them individually (even from a mobile phone) and nothing will 404.

WHY YOU NEED TO "HOST" THIS FOLDER
------------------------------------
Installing an app as a real Android / Desktop app (icon on home screen,
opens full-screen with no browser bar) only works when the files are
served from a web address (http/https), not when you just double-click
index.html on your computer. This is a browser security rule, not a
limitation of this app.

The good news: you do NOT need a paid server. Pick any ONE option below.

OPTION 1 — Netlify Drop (easiest, no account needed, desktop only)
------------------------------------------------------------------
1. Go to https://app.netlify.com/drop
2. Drag ALL 6 files onto the page (select all of them together)
3. You'll get a free link like https://your-app.netlify.app
4. Open that link on your phone in Chrome -> menu (⋮) -> "Install app"
5. Open the same link on your computer in Chrome -> click the install
   icon (⊕) in the address bar -> it installs as a Desktop app

OPTION 2 — GitHub Pages (free, permanent link, works from mobile too)
-----------------------------------------------------------------------
1. Create a free GitHub account, create a new repository
2. "Add file" -> "Upload files" -> select ALL 6 files (index.html,
   manifest.json, sw.js, icon-192.png, icon-512.png, icon-apple-touch.png)
   and upload them together. Do NOT put them inside a subfolder.
3. Repository Settings -> Pages -> Deploy from branch -> main -> Save
4. You'll get a link like https://yourusername.github.io/reponame/
5. To check nothing is missing, open these two links directly —
   both should load (not show 404):
     https://yourusername.github.io/reponame/manifest.json
     https://yourusername.github.io/reponame/icon-192.png
6. Install it on Android/Desktop the same way as Option 1

OPTION 3 — Run it on your own shop computer (local network only)
---------------------------------------------------------------------
If you have Python installed on your computer:
1. Open this folder in a terminal / command prompt
2. Run:  python3 -m http.server 8000
3. On the SAME computer open: http://localhost:8000 in Chrome and install it
4. On phones connected to the same WiFi, use http://<your-computer-IP>:8000

AFTER INSTALLING
------------------
- Android: shows up as a normal app icon, opens full-screen, works offline
- Desktop (Windows/Mac/Chromebook): opens in its own window like a
  regular desktop app, also works offline
- Your product, billing and customer data is stored only on that
  device/browser (not on any server) — so back up regularly from
  Settings -> Export Backup inside the app

SHOP DETAILS ALREADY FILLED IN
---------------------------------
Shop Name : KAVITHA TELECOM
Address   : (not set — add it from Settings inside the app)
Phone     : (not set — add it from Settings inside the app)
Logo      : Already set to the Kavitha Telecom logo (the fire "K" emblem
            with mobile, cases, earbuds, cable and power bank icons)
You can change any of these anytime from Settings inside the app.

WHAT'S NEW IN THIS VERSION
------------------------------
- App renamed to "Kavitha Telecom" everywhere in the app (title bar,
  home screen name, install prompts, backups).
- Shop logo replaced with your Kavitha Telecom logo — used in the app
  header, the "Install App" prompts, invoices/receipts, and the Ad
  Catalog page.
- Home screen / desktop app icon now uses your new Kavitha Telecom
  logo (see note below — you must reinstall for the new icon to show
  up if you had an older version installed).
- Default Ad Catalog sample cards updated to mobile-shop categories
  (Phone Covers, Earbuds, USB Cables, Power Banks) to match your
  business — edit or replace these anytime from the Ad Catalog screen.
- Bluetooth thermal (POS) receipt printing prints your shop logo at
  the top of every receipt, above the shop name — works with plain
  ESC/POS thermal printers (58mm/80mm). No extra setup needed; it uses
  whatever logo is set in Settings.
- Purchases section (bottom nav) — record stock coming in from
  suppliers. Adding a purchase automatically increases the stock of
  the matching product (or creates a new product if it's not in your
  list yet), and tracks how much you've paid / still owe each supplier.
- Reports screen also shows a Purchases Overview (total purchases,
  amount paid, amount due) with a downloadable Purchase Report PDF,
  alongside the existing Sales Report.

IMPORTANT — About the app icon on your phone/desktop
------------------------------------------------------
If you already installed an older app icon on your phone or computer,
Android/Chrome/Windows caches that icon at install time — it will NOT
automatically refresh to the new Kavitha Telecom logo just by updating
the files on the server. To see the new logo as your app icon:
  1. Uninstall/remove the old app icon (long-press it > Uninstall,
     or remove it from your desktop/Start menu).
  2. Open this app fresh in Chrome and use "Install" again from
     Settings, or the browser's "Add to Home Screen" / "Install app"
     option.
The new icon (your Kavitha Telecom fire-K logo) will then appear
correctly.

STILL TO DO
------------------
- Add your shop's phone number, address and GST (if any) from
  Settings inside the app — these currently show blank on invoices.
