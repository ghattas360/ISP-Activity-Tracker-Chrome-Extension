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

