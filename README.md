# Monthly Electricity Tracker (GitHub Pages PWA + Google Sheets Sync)

## 1. Files to Upload to Your GitHub Repository Root
Upload these 6 files directly to the root of your repository (e.g., `https://ksn009.github.io/<repo-name>/`):
- `index.html`
- `manifest.json`
- `sw.js`
- `icon-192.png`
- `icon-512.png`
- `icon-maskable-512.png`

Then enable **Settings -> Pages -> Deploy from branch (`main` / `root`)** on GitHub.

*(Keep `Code.gs` for Google Apps Script — you do not need to publish it on GitHub Pages.)*

## 2. Connect Google Sheets Cloud Database
1. Create a blank Google Sheet (e.g., **Monthly Electricity Tracker Data**).
2. Click **Extensions -> Apps Script**, clear any default code, and paste `Code.gs`.
3. *(Optional)* Set a passcode: `const SYNC_SECRET = 'your-pin';`.
4. Click **Deploy -> New deployment -> Web app**:
   - **Execute as:** Me
   - **Who has access:** Anyone
5. Authorize and copy the `/exec` Web App URL.
6. Open your hosted app -> **Settings** -> paste the Web App URL (and Sync Secret if set) -> click **Save Configuration**.

## 3. Install as an App (PWA)
- **Android (Chrome/Edge):** Tap the **Install** button in the top header (or menu -> Add to Home screen).
- **iPhone (Safari):** Tap **Share -> Add to Home Screen**.
