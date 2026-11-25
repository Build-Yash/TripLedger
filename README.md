# TripLedger
**Live app:** https://build-yash.github.io/TripLedger/

Open the link on your phone, then use Add to Home Screen to install it.

A lightweight, mobile-first web app for recording business trip expenses on the spot and producing a clean reimbursement report at the end of the trip.

Built to solve a common problem: small payments made through UPI, cash and cards during client visits get forgotten, and the expense sheet is rebuilt from memory afterwards.

## Features

- **Trips:** create trips, mark them complete, reopen them, and compare totals across trips
- **Quick expense entry:** amount, description, payment mode (UPI, Cash, Debit Card, Credit Card, Other), date and time, location and notes
- **Bank name:** shown for debit and credit card payments, with a list of common Indian banks plus a manual "Other" option
- **Payment screenshots:** attach multiple images per expense from the camera or gallery, and view them again later
- **Dashboard:** total spend, totals by payment mode and category, recent expenses
- **History:** search by description, filter by payment mode and date, edit or delete entries
- **PDF report:** employee name, trip details, full transaction table, totals by payment mode, overall total, and receipt images
- **CSV export, share sheet, backup and restore**
- **Delete data:** PIN-protected option that clears all trips, expenses and receipts
- **Light and dark mode** that follows the device setting
- **Installable:** add to the Home Screen on iPhone or Android

## How to use

1. Open the hosted link in your phone browser.
2. iPhone (Safari): Share, then **Add to Home Screen**. Android (Chrome): menu, then **Add to Home screen** or **Install app**.
3. Create a trip, add expenses with the **+** button, then open **Reports** to save the PDF.

## Tech

Single-file app: plain HTML, CSS and JavaScript, no build step. PDF generation uses [jsPDF](https://github.com/parallax/jsPDF).

## Data and privacy

- All data is stored in the browser's `localStorage` on the user's own device. There is no server and no account.
- Receipt images are resized before saving to keep storage small.
- Browsers allow only a few MB per site, so back up and clear old trips regularly.
- Clearing browser data or removing the app can erase your trips. Use **Back up data** in the Reports tab.

## Limitations

- No cloud sync, so data does not move between devices.
- The delete PIN is stored in the app code and is meant only to prevent accidental deletion, not for security.

## Running locally

Open `index.html` in a browser, or host the file on any static host such as Netlify, GitHub Pages or Cloudflare Pages.

## Screenshots

Add screenshots made with dummy data to a `screenshots` folder and link them here.

## License

MIT, see [LICENSE](LICENSE).
