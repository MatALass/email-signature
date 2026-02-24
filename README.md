# email-signature

A **100% email-client-friendly** HTML signature (Gmail/Outlook) using:
- Tables (email-safe)
- Inline styles only
- No JavaScript
- No external CSS

## Files

- `signature.html` — the signature template to copy into your email client
- `assets/icons/` — small PNG icons you can host (e.g. via GitHub Pages)

## How to use (recommended workflow)

1) **Host the icons** so `signature.html` can reference public URLs.
   - Easiest: enable GitHub Pages on this repo (Settings → Pages → Deploy from branch → `main` / `/root`)
   - Your icons will then be available at:
     `https://<USERNAME>.github.io/<REPO>/assets/icons/email.png` (etc.)

2) Open `signature.html` and replace placeholders:
- `YOUR NAME`, `YOUR ROLE`, links, phone/email
- `ICON_*_URL` with your hosted icon URLs

3) Paste into your email client:
- **Gmail**: Settings → See all settings → General → Signature → create new → paste
- **Outlook**: Settings → Mail → Compose and reply → Email signature (paste)

## Notes
- Keep it simple for maximum compatibility: avoid fancy CSS, fonts, and layout tricks.
- If you want a web contact page, keep it in a **separate repo** (recommended).
