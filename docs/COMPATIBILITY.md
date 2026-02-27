# Compatibility Guide

This project follows strict **email HTML best practices** to ensure
stable rendering across major email clients.

## Core Principles

-   Table-based layout (no div-based structure)
-   Inline CSS only
-   Explicit widths for stability
-   No external stylesheets
-   No JavaScript
-   Outlook-safe spacing rules (`mso-*` compatible)

Email HTML is fundamentally different from browser HTML. Many modern CSS
features are not supported in email environments.

------------------------------------------------------------------------

## Clients Tested

### Reliable Rendering

-   Gmail (Web)
-   Outlook Web
-   Apple Mail (macOS / iOS)

### Special Case: Outlook Desktop (Windows)

Outlook Desktop uses the Microsoft Word rendering engine.

To ensure compatibility:

-   Avoid flexbox and CSS grid
-   Avoid floats and absolute positioning
-   Avoid margin-based layout
-   Prefer fixed widths
-   Use inline font declarations
-   Define explicit image dimensions

------------------------------------------------------------------------

## Known Limitations

-   Web fonts are not supported in most email clients
-   Advanced CSS selectors are ignored
-   Dark mode behavior may vary across clients
-   SVG images are not reliably supported (PNG recommended)

------------------------------------------------------------------------

## Testing Checklist

Before using the signature in production:

-   Verify icons are aligned properly
-   Check line-height consistency
-   Confirm links are clickable
-   Ensure no unexpected font substitutions occur
-   Confirm images are not stretched (width + height explicitly set)
-   Test in at least Gmail and Outlook Desktop

------------------------------------------------------------------------

## Recommended Testing Workflow

1.  Open `demo/index.html` in browser
2.  Copy rendered signature
3.  Paste into Gmail
4.  Send test email to:
    -   Gmail account
    -   Outlook account
    -   Mobile device
5.  Validate spacing and alignment

------------------------------------------------------------------------

If you modify the layout, always re-test in Outlook Desktop.
