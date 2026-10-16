# Maglite Collection — standalone app

Runs on your phone with no Claude and no account. Your torches, photos, classes and
dating charts are stored on the phone itself. Nothing is uploaded anywhere.

## Files in this folder
index.html · sw.js · manifest.webmanifest · jszip.min.js · icon-192.png · icon-512.png · README.md

## 1. Put the app online (once, about 10 minutes, free) — GitHub Pages
The app needs a secure (https) web address so Android can install it and run it offline.
Only these program files go online. Your data never does.

1. Go to github.com and create a free account (if you don't have one).
2. Click **+** (top right) → **New repository**. Name it `maglite`, choose **Public**, click **Create repository**.
3. On the new page, click **uploading an existing file**. Drag in all the files from this folder
   (not the folder itself). Click **Commit changes**.
4. Open **Settings → Pages**. Under "Build and deployment", Source = **Deploy from a branch**,
   Branch = **main**, folder = **/ (root)**. Click **Save**.
5. Wait 1–2 minutes. Your app address is `https://YOUR-USERNAME.github.io/maglite/`
   (shown at the top of the Pages screen).

Never upload a backup .zip to GitHub — the repository is public.

## 2. Install it on your Android phone
1. Open the address in **Chrome** on the phone.
2. Tap **⋮ → Add to Home screen** (or **Install app**) → **Install**.
3. Open it from the new icon. It opens full-screen and works offline from then on.

## 3. Load your collection
1. Save `maglite-starter-backup.zip` to the phone (e.g. Downloads).
2. In the app: **Restore from backup** → pick the file → **Restore**.
   All 18 torches and 45 photos load.

## Backups — do this regularly
More → Backup & restore → **Make backup file** → **Save to phone** or **Share to Drive / email**.
The file holds everything (torches, photos, receipts, classes, charts, wanted list).
The app reminds you if you haven't backed up for 30 days.

**Changing phones:** install the app on the new phone (step 2), then Restore your latest backup.
**Warning:** uninstalling the app, or clearing Chrome's data for the site, deletes the collection
on that phone. Your backup file is the safety copy.

## Adding a new class of torch (no help needed)
More → **Classes** → **+ New class**. Give it a name, cell type (AAA, CR123A, 18650…),
volts per cell or a fixed pack voltage, model suggestions, and optionally link a dating chart.

## Building or editing a dating chart
More → **Dating charts** → **+ New chart** (or Edit on an existing one).
1. Add **eras** (year ranges). Leave "To" empty for one that runs to today.
2. Add **features** (e.g. Bezel mark) and their **options** (e.g. Panther TM), ticking the eras each option appears in.
3. Optional: switch on **serial ranges** (first digit = cell count).
4. Save, then link the chart to a class under Classes. **Date it** uses it straight away.

## If you change the app files later
Edit `sw.js` and change `const VERSION = "mc-v1"` to `"mc-v2"` (and so on), then upload.
That tells phones to pick up the new version. Your data is not affected.
