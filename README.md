![Status](https://img.shields.io/badge/status-stable-black) ![Email
HTML](https://img.shields.io/badge/email-safe-blue) ![Outlook
Compatible](https://img.shields.io/badge/outlook-compatible-lightgrey)
![License](https://img.shields.io/badge/license-MIT-green)

# email-signature

A production-ready, email-client-safe HTML signature template\
engineered to render consistently across:

-   Gmail (Web)
-   Outlook Web
-   Outlook Desktop (Word rendering engine)
-   Apple Mail

Built using strict email HTML best practices:

-   Table-based layout
-   Inline styles only
-   No JavaScript
-   No external CSS
-   Outlook-safe spacing handling (`mso-*` compatible)

------------------------------------------------------------------------

## Why this project exists

Modern CSS does not render reliably inside email clients.

Outlook Desktop uses Microsoft Word as its rendering engine.\
Most layout systems (flexbox, grid, floats) fail in email environments.

This project provides:

-   A minimal, robust layout
-   A compatibility-first structure
-   A professional design that does not break

This is email-engineered HTML.

------------------------------------------------------------------------

## Features

-   Clean two-column identity layout
-   Short visual divider (design-focused)
-   Hosted icons via GitHub Pages
-   Copy/paste ready templates
-   Compact version available
-   Strict compatibility-first structure

------------------------------------------------------------------------

## Preview

### Full Version

![Full Signature](assets/screenshots/full.png)

### Compact Version

![Compact Signature](assets/screenshots/min.png)

(Add your screenshots inside `assets/screenshots/` and update filenames
if needed.)

------------------------------------------------------------------------

## Project Structure

    email-signature/
    │
    ├── templates/
    │   ├── signature.html
    │   └── signature.min.html
    │
    ├── demo/
    │   └── index.html
    │
    ├── assets/
    │   ├── icons/
    │   └── screenshots/
    │
    ├── docs/
    │   ├── COMPATIBILITY.md
    │   └── PRIVACY.md
    │
    ├── CONTRIBUTING.md
    ├── LICENSE
    └── README.md

------------------------------------------------------------------------

## Quick Start

### 1. Enable GitHub Pages

Settings → Pages\
Deploy from branch → `main` → `/root`

Icons will be available at:

    https://<USERNAME>.github.io/<REPO>/assets/icons/email.png

------------------------------------------------------------------------

### 2. Customize the Template

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

------------------------------------------------------------------------

### 3. Paste into Your Email Client

Important: paste the rendered signature, not the raw HTML.

Gmail:\
Settings → General → Signature → Create new → Paste

Outlook Web:\
Settings → Mail → Compose and reply → Email signature → Paste

------------------------------------------------------------------------

## Compatibility

See:

    docs/COMPATIBILITY.md

For detailed client constraints and testing workflow.

------------------------------------------------------------------------

## Privacy Considerations

See:

    docs/PRIVACY.md

Before publishing personal contact details.

------------------------------------------------------------------------

## Contributing

See:

    CONTRIBUTING.md

Pull requests must respect email-client compatibility rules.

------------------------------------------------------------------------

## License

MIT License
