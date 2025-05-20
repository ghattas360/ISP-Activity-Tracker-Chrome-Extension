# ISP Activity Tracker – Chrome Extension 🔍💻

A lightweight Chrome Extension that helps Point-of-Sale agents log their activity when generating codes on ISP web dashboards.

---

## ✅ Features

- Tracks selected code price (e.g., $16, $25, etc.)
- Detects when the "Generate Code" button is clicked
- Logs the action with a timestamp
- Stores data **locally** using `localStorage`
- Allows **CSV export** from popup
- Popup interface shows all logs with clear formatting
- (Coming soon): Extract the generated code for full logging

---

## 📦 How It Works

1. When the ISP site loads, the extension listens for clicks on the "Generate Code" button.
2. It checks which price option was selected.
3. It logs:
   - The full label (e.g., `iClik - 25$  Price : 25`)
   - The parsed dollar amount
   - The exact time of the action
4. All logs are stored in `localStorage` and can be viewed/exported in the popup.

---

## 📁 File Structure

isp-activity-tracker/
├── manifest.json # Chrome extension config
├── content.js # Tracker script injected into the ISP page
├── popup.html # Extension popup interface
├── popup.js # JS logic for viewing/exporting logs
├── styles.css # Optional styling for the popup


---

## 🔧 Installation (Development Mode)

1. Clone or download this repo.
2. Open Chrome and go to `chrome://extensions/`.
3. Enable **Developer mode** (top right).
4. Click **"Load unpacked"** and select the folder.
5. Visit your ISP platform and try generating a code!

---

## 📤 Exporting Logs

- Open the extension popup
- Click **Export CSV**
- The CSV will be downloaded to your default browser folder (usually `Downloads`)

---

## 📌 Notes

- All logs are **only saved locally** — no data is sent to any server.
- You can clear logs anytime from the popup.
- Future versions will add:
  - Generated code extraction
  - Google Sheets sync
  - More customization and filters

---

## 🧠 Tech Used

- JavaScript (ES6+)
- Chrome Extensions API (Manifest v3)
- HTML/CSS for the popup
- `localStorage` for persistence

---

## 🙌 Author

Built by [Ghattas Saliba](https://www.linkedin.com/in/ghattassaliba/)  
First Chrome Extension. Many more to come!

---

## 📄 License

MIT License

