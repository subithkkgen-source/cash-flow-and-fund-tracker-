# CashFlow Ledger

A complete browser-based Cash Flow Management & Fund Requirement tracking platform — runs fully offline, installs as a Windows/Android app, all data stored locally on your device.

## 🌐 Live App
Once deployed to GitHub Pages, your app will be live at:
```
https://YOUR-USERNAME.github.io/REPO-NAME/
```

## ✨ Features
- Bank account management with statement import (Excel/CSV/PDF)
- Transaction ledger with classification, CF heads, sub-categories
- Cash Flow Statement (Operating / Investing / Financing)
- Sanction Balance tracking with set-off against payments
- **Fund Requirement Management System (FRMS)** — department fund requests, due date monitoring, payment status tracking
- Dashboard with charts (trend, account balances, category breakdown)
- Installable as a Progressive Web App (PWA) on Windows, Android, macOS
- Works fully offline after first load
- Dark mode (FRMS module)

## 📦 Deploy to GitHub Pages (one-time setup)

1. Create a new repository on GitHub (e.g. `cashflow-ledger`)
2. Upload all files from this folder to the repository root:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
   - `.nojekyll`
3. Go to **Settings → Pages**
4. Under **Source**, select **Deploy from a branch**
5. Branch: `main`, folder: `/ (root)` → **Save**
6. Wait 1–2 minutes. Your app is live at `https://YOUR-USERNAME.github.io/REPO-NAME/`

## 📱 Install on Android
1. Open the GitHub Pages URL in **Chrome** on your Android phone
2. Tap the **⋮ menu → Install app** (or wait for the install banner)
3. The app icon appears on your home screen — opens full-screen, no browser bar

## 🖥 Install on Windows
1. Open the GitHub Pages URL in **Chrome** or **Edge**
2. Click the **⊕ Install** icon in the address bar (or the in-app install banner)
3. The app installs to your Start Menu and Taskbar — opens in its own window

## 🔒 Data & Privacy
All data (accounts, transactions, fund requests) is stored in your browser's `localStorage` — **nothing is sent to any server**. Each device/browser keeps its own separate data. To move data between devices, use the Export to Excel feature and re-import.

## 🔄 Updating the App
After making changes to `index.html`, simply re-upload it to your GitHub repository (or `git push`). GitHub Pages updates automatically within ~1 minute. Installed PWA users will see an "update available" prompt next time they open the app.

## 🛠 Local Development
To test locally before deploying:
```bash
cd CashFlowLedger-PWA
python -m http.server 8080
```
Then open `http://localhost:8080`
