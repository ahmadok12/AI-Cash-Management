# RozCash AI Cashbook — Testing Prototype

A mobile-first cash management prototype for Roman Urdu voice, chat and manual transaction entry.

## Test locally

Publish the app on GitHub Pages and open its HTTPS address in Chrome. Allow microphone access when prompted. Voice entry is configured for Pakistan English so spoken Roman Urdu remains in Latin letters for the prototype parser.

Try these phrases:

- `mujhe bees hazaar cash aya`
- `mujhe 20000 cash aya`
- `maine 3180 khane ke diye`
- `2000 rs diye chaye wale ko`
- `office cash se petrol ke 7500 diye`

The latest parser treats `cash aya` as cash received. For phrases such as `diye chaye wale ko`, it records cash paid and places `Chaye Wala` in the note.

For this offline prototype parser, spoken digits such as `20000` are recognized more reliably than number words such as `bees hazaar`.

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
