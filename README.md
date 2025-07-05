# TDBA Vault Project

This project powers the TDBA Card Vault — a web application that allows users to:

- Upload images of basketball cards
- Extract player name, year, brand, and card type
- Estimate market value (Raw + PSA 10)
- Assign Tier (1–4) using predefined logic
- Log the card to a central Google Sheet (`TDBA RWA Cards Vault`)
- Display cards publicly in a dynamic, mobile-friendly vault UI

---

## 📁 Folder Contents

| File | Purpose |
|------|---------|
| `index.html` | Live front-end for displaying the vault using `metadata.json` |
| `metadata.json` | Card data (generated or AI-enriched) |
| `upload.html` | Static upload form (manual card entry) |
| `firebase.json` | Firebase hosting configuration |
| `.firebaserc` | Firebase project connection |
| `README.md` | You are reading this file |
| `logo/` | Optional folder for storing brand assets |
| `images/` | Can be used for local image references or demos |

---

## 🚀 Deployment Instructions

1. Clone this repo or unzip into a folder
2. Install Firebase CLI: `npm install -g firebase-tools`
3. Log in: `firebase login`
4. Run: `firebase init` and select:
   - Hosting: Configure files for Firebase Hosting
   - Use `public` directory (or current folder)
   - Deploy everything from root folder
5. When ready: `firebase deploy`

Your project will go live at: `https://<your-project>.web.app`

---

## 🔗 Connected Services

- Google Apps Script Webhook (linked to Google Sheet)
- Firebase Hosting (for vault UI)
- Optional: Firebase Storage for image uploads
