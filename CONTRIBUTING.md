# Contributing

Thank you for your interest in improving this project.

This repository follows strict email-client compatibility principles.
Email HTML is not browser HTML.

Before submitting a pull request, please read the guidelines below.

------------------------------------------------------------------------

## Core Rules

1.  Keep the layout table-based (no div layout systems).
2.  Use inline styles only (no external CSS).
3.  Avoid modern CSS (flexbox, grid, float, position, web fonts).
4.  Define explicit width and height for images.
5.  Test changes in:
    -   Gmail (Web)
    -   Outlook Web
    -   Outlook Desktop (Windows)

------------------------------------------------------------------------

## Design Principles

-   Minimal and professional
-   High contrast and readable typography
-   No unnecessary visual complexity
-   No decorative elements that may break in Outlook

------------------------------------------------------------------------

## Testing Workflow

1.  Open `demo/index.html`
2.  Copy the rendered signature
3.  Paste into Gmail
4.  Send test email to:
    -   Gmail account
    -   Outlook account
    -   Mobile device
5.  Validate spacing, line-height, and icon alignment

------------------------------------------------------------------------

## Pull Request Guidelines

When submitting a PR:

-   Clearly describe what was changed
-   Explain why the change improves compatibility or design
-   Confirm manual testing was done

Contributions that break email-client compatibility will not be merged.

------------------------------------------------------------------------

Email reliability \> visual complexity.
