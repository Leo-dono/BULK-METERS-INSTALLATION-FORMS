# Bulk Meter Installation Form

A responsive, dark-themed web form for capturing bulk water meter installation data. The app supports PDF export, email/WhatsApp quick sharing, dynamic fields, and simple CAPTCHA verification.

## Features
- **Modern UI** built with Poppins and Font Awesome icons.
- **Dynamic field sets**: Industrial, Production, or Border meters show different input sections.
- **Validation**: Mandatory fields and conditional "Remarks" enforcement for Substandard installations.
- **Security**: Lightweight arithmetic CAPTCHA to prevent spam submissions.
- **PDF Generation**: Uses `html2canvas` + `jsPDF` to generate multi-page PDFs.
- **Sharing**: Quick actions for Email (`mailto:`) and WhatsApp deep-links.
- **Completion Flow**: Status indicators, modal reminders, and submission overlay.

## Configure contacts
This demo includes **dummy contacts**:
- Email: `bulkmeters@example.com`
- WhatsApp (special regions): `233000000000`, `233000000001`
- WhatsApp (other regions): `233000000002`, `233000000003`

To use real contacts, edit them inside `index.html` in the **handleSendEmail** and **handleSendWhatsApp** functions.

## How to run
1. Clone or download this repository.
2. Open `index.html` in any modern browser (Chrome, Edge, Firefox).
3. Fill the form, solve CAPTCHA, and select "Send via Email" or "Send via WhatsApp".
4. A PDF will be generated for attachment.

## Repository structure
```
/
├─ .gitignore
├─ LICENSE
├─ README.md
└─ index.html
```

## Deploy with GitHub Pages
1. Push this repo to GitHub.
2. Go to **Settings → Pages → Build and deployment**.
3. Source: Deploy from branch → select `main` and `/ (root)`.
4. Save. Your live form will be available at `https://<username>.github.io/<repo-name>`.

## License
Released under the MIT License. See [LICENSE](LICENSE) for details.
