![Status](https://img.shields.io/badge/status-stable-black) ![Email
HTML](https://img.shields.io/badge/email-safe-blue) ![Outlook
Compatible](https://img.shields.io/badge/outlook-compatible-lightgrey)
![License](https://img.shields.io/badge/license-MIT-green)

# email-signature

A **production-ready, email-client-safe HTML signature template**\
designed to render consistently across:

-   Gmail (Web)
-   Outlook Web
-   Outlook Desktop (Word rendering engine)
-   Apple Mail

Built using strict **email HTML best practices**: - Tables only (no div
layouts) - Inline styles only - No JavaScript - No external CSS -
Outlook-safe spacing rules (`mso-*` compatible)

------------------------------------------------------------------------

## Why this project exists

Modern CSS does not work reliably in email clients.\
Outlook desktop uses Microsoft Word as its rendering engine.

This project provides a **minimal, robust, and portable signature
layout** that:

-   does not break in Outlook
-   does not rely on remote CSS
-   does not use unsupported modern layout systems (flex/grid)
-   remains visually clean and professional

This is not just HTML.\
This is **email-engineered HTML**.

------------------------------------------------------------------------

## Features

-   Clean two-column layout
-   Short visual divider (design-focused)
-   Hosted icons via GitHub Pages
-   Copy/paste ready templates
-   Compact version available
-   Strict compatibility-first structure

------------------------------------------------------------------------

## Project structure

    email-signature/
    │
    ├── templates/
    │   ├── signature.html        # Main version
    │   └── signature.min.html    # Compact version
    │
    ├── demo/
    │   └── index.html            # Preview page (GitHub Pages)
    │
    ├── assets/
    │   └── icons/                # Hosted icon assets
    │
    ├── docs/
    │   ├── COMPATIBILITY.md
    │   └── PRIVACY.md
    │
    └── README.md

------------------------------------------------------------------------

## Quick start

### Enable GitHub Pages (for icon hosting)

GitHub repo → **Settings → Pages**

-   Source: Deploy from a branch\
-   Branch: `main`\
-   Folder: `/root`

Your hosted icons will be accessible at:

    https://<USERNAME>.github.io/<REPO>/assets/icons/email.png

------------------------------------------------------------------------

### Customize the template

Open:

    templates/signature.html

Replace:

-   Name
-   Role
-   Location
-   Phone
-   Email
-   LinkedIn
-   GitHub

Ensure icon URLs match your GitHub Pages deployment.

Example:

    https://matalass.github.io/email-signature/assets/icons/email.png

------------------------------------------------------------------------

### Paste into your email client

Important: Paste the **rendered HTML**, not the raw source code.

#### Gmail

Settings → See all settings → General → Signature → Create new → Paste

#### Outlook (Web)

Settings → Mail → Compose and reply → Email signature → Paste

------------------------------------------------------------------------

## Preview

Open:

    demo/index.html

via GitHub Pages to validate rendering before pasting.

------------------------------------------------------------------------

## Compatibility

Tested layout principles:

-   Table-based structure
-   Explicit widths
-   Inline typography
-   No CSS classes
-   No margin collapse dependency
-   Outlook-safe line height handling

See:

    docs/COMPATIBILITY.md

for detailed constraints.

------------------------------------------------------------------------

## Customization guidelines

When modifying the layout:

✔ Keep tables\
✔ Keep inline styles\
✔ Avoid flexbox, grid, position, float\
✔ Avoid web fonts\
✔ Test in Outlook Desktop

Email HTML is not browser HTML.

------------------------------------------------------------------------

## Privacy considerations

Publishing phone numbers or personal email addresses in public
repositories may increase:

-   Spam
-   Scraping
-   Targeted phishing

Consider using: - Alias email - Contact page - Reduced public contact
exposure

See:

    docs/PRIVACY.md

------------------------------------------------------------------------

## Contributing

Contributions are welcome, but must respect email-client constraints.

Before submitting a PR:

-   Test in Gmail and Outlook
-   Keep layout table-based
-   Avoid modern CSS
-   Preserve minimal, professional design

------------------------------------------------------------------------

## License

MIT --- free to use, modify, and adapt.
