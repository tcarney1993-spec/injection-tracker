# Injection Tracker

A free, offline-capable, mobile-first injection logging PWA. No build process or account required.

## Publish using GitHub Pages
1. Create a new **public** GitHub repository named `injection-tracker` (keep this separate from any existing app).
2. Upload all four app files (`index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`) into the repository root and commit them. You can also upload this README.
3. In the repository, go to **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, choose `main` and `/ (root)`, then **Save**.
4. Wait for deployment. Open `https://YOUR-USERNAME.github.io/injection-tracker/` in iPhone Safari.
5. Tap **Share → Add to Home Screen → Add**.

## Privacy and backups
Records are saved in localStorage on the current browser/device only. GitHub hosts the public app code, not the private records. Data is not synced between devices. Use **Settings → Backup JSON** regularly and save the file somewhere safe. Use **Restore JSON backup** to move your data to another device. CSV export opens in Google Sheets.

This is a recordkeeping tool, not a dosing calculator or medical advice.

## Multiple medications and editable profiles
Add as many medications as you need. Each has its own name, optional schedule, and independent cycle start date. Tap **Edit** beside any medication to update its details or start date without deleting the medication or its injection history. The selected medication and injection date determine the suggested cycle week for **new** logs. You can override the suggested week. Existing saved injection logs retain their recorded cycle weeks when a medication start date changes, so historical records are not silently rewritten.

## Automatic cycle week
Cycle week 1 covers days 1–7 after the medication's cycle start date, week 2 covers days 8–14, etc. Dates before the start date are left blank. Changing the medication or injection date recalculates the proposed cycle week in the log form.
