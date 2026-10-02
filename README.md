# WHY Z? = YZ=?Z

## Included
- Supplied WHY Z? logo
- Wider 44px, lighter graph pattern
- Persistent REGISTER A PROJECT CTA while scrolling
- Full project-registration form
- Seven clickable live projects
- Founding-member LinkedIn
- GitHub Pages deployment workflow

## Inbox setup
In `index.html`, replace:
`const CONTACT_EMAIL = "YOUR_INBOX_EMAIL_HERE";`
with the real WHY Z? inbox.

### Current safe behavior
With `FORM_ENDPOINT` blank, the registration form creates a pre-addressed email draft using the visitor's email client. The visitor presses Send.

### True automatic delivery
Set `FORM_ENDPOINT` to a trusted form/email endpoint or your own serverless API. Do not put SMTP passwords, API keys or other private credentials into this public HTML.

## Registration fields
Name, company/startup, email, phone/WhatsApp, project name, collaboration type, problem brief, skills/technology, timeline, budget/stipend, project link and additional notes.

## GitHub Pages
Upload the contents to the repository root, push to `main`, then choose GitHub Actions under Settings → Pages.
