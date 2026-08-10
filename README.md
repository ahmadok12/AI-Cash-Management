# RozCash AI Cashbook — Testing Prototype

A mobile-first cash management prototype for Roman Urdu voice, chat and manual transaction entry.

## Test locally

Open `index.html` in Chrome. Voice entry works best in Chrome and may require the page to be served over HTTPS.

## Publish with GitHub Pages

1. Create a new public GitHub repository.
2. Upload `index.html` to the root of the repository.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.

GitHub will show the public site URL after deployment completes.

## Prototype limitations

- Transactions and preferences are saved only in the current browser using local storage.
- Google Sheets connection is simulated and clearly labelled as demo mode.
- Roman Urdu understanding uses an offline prototype parser; the production version should use an AI extraction API through a secure backend.
- Browser voice recognition availability varies by browser and device.

## Included test flows

- Roman Urdu examples such as `mje 20000 cash aya`, `maine 3180 khane k diye`, and `kal client se 2 lakh mile`
- Editable confirmation before saving
- Optional auto-save with Undo
- Manual entry
- Multiple cashbooks
- Transaction search and filters
- Cash-flow and category reports
- Simulated Google Sheets connection
