# Monthly Electricity Tracker (GitHub Pages PWA + Google Sheets Sync)

## 1. Connect Google Sheets Cloud Database
1. Create a blank Google Sheet (e.g., **Monthly Electricity Tracker Data**).
2. Click **Extensions -> Apps Script**, clear any default code, and paste `Code.gs`.
3. *(Optional)* Set a passcode: `const SYNC_SECRET = 'your-pin';`.
4. Click **Deploy -> New deployment -> Web app**:
   - **Execute as:** Me
   - **Who has access:** Anyone
5. Authorize and copy the `/exec` Web App URL.
6. Open your hosted app -> **Settings** -> paste the Web App URL (and Sync Secret if set) -> click **Save Configuration**.

## 2. Install as an App (PWA)
- **Android (Chrome/Edge):** Tap the **Install** button in the top header (or menu -> Add to Home screen).
- **iPhone (Safari):** Tap **Share -> Add to Home Screen**.
