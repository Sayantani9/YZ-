WHY Z? = YZ=?Z

A Gen-Z-native project and innovation network connecting student builders, startups and companies through real projects, technical execution and fresh ideation.

The website is designed as a hybrid of a brutalist engineering lab, editorial portfolio, technical research studio and experimental Gen-Z agency.

What the site communicates

WHY Z? is built around a simple loop:

STUDENTS → REAL PROBLEMS → PROJECTS → COMPANIES → MORE BUILDERS

The site separates the ecosystem into clear layers:





WHY Z? — the network and the reason it exists.



LIVE WORK — real project builds with large browser-style previews.



ABOUT — founding member and collaboration ecosystem.



AGENT LAB — AI agents presented as products rather than generic chatbots.



REGISTER — a persistent route for companies/startups to submit a project brief.



CONNECT — direct email, phone and WhatsApp contact.



Live project showcase

The current project section contains six builds. CinderPeak has been removed from this version.







Project



Focus



Live site





Smart Waste System



IoT + AI / waste segregation



https://shuddh-main-2.vercel.app





Pistons Autopedia



Automotive / vehicle knowledge



https://piston-s-autopedia-cnm374a2y-theinvinciblefire-8003s-projects.vercel.app





Rakshak



Cybersecurity / threat reporting



https://rakshak-weld.vercel.app





Vayunetra



Satellite AQI forecasting / ML



https://vayunetra-five.vercel.app





Smart Attendance System



Computer vision + IoT



https://sayantani9.github.io/SMART-ATTENDANCE-SYSTEM_COGNIZANT/





Tendrix



Robotics + ML / L&T project



https://tendrix-site.vercel.app/#innovations



Project display behaviour

Each project is shown as a large browser-style display containing a lazy-loaded iframe of the live website, followed by:





project name



domain / category



plain-language explanation



reported metric or output



"What it shows" purpose line



OPEN LIVE SITE action

Some external websites may restrict iframe embedding through their own security headers. If a preview does not render, the OPEN LIVE SITE button still takes the visitor directly to the project.

Contact

Email: sanghamitra.ventures@gmail.com
Phone / WhatsApp: +91 93459 94213
WhatsApp: https://wa.me/919345994213

Project registration

The registration form collects:





Name



Company / Startup



Email



Phone / WhatsApp



Project / Idea name



Collaboration type



Project brief



Tech / skills required



Timeline



Budget / stipend



Existing project link



Additional notes



Email behaviour

The site is intentionally safe to host as a static GitHub Pages website. By default, the form creates a pre-addressed email to:

sanghamitra.ventures@gmail.com

The visitor confirms and sends the email from their mail client.

For true automatic submission without opening an email client, set the FORM_ENDPOINT constant in index.html to a trusted serverless/form endpoint. Do not place SMTP passwords, API secrets or private credentials in this public repository.

Agent Lab

The Agent Lab is structured for real AI systems, not generic chatbot cards. Each agent should eventually communicate:

Problem → Agent → Tools → Action → Outcome

When adding an agent, replace the placeholder card with:





Agent name



What it does



Who it is for



Problem it solves



Actual actions/capabilities



Models / APIs / tools



Live / beta / private status



Demo link



GitHub link, if public



Screenshot or product video, if useful



File structure

WHY-Z-GitHub-Site-v4/
├── index.html
├── README.md
├── .nojekyll
├── assets/
│   └── why-z-logo.png
└── .github/
    └── workflows/
        └── pages.yml



Deploy on GitHub Pages

This is a static site. No Hostinger account or custom domain is required to publish the current version. GitHub Pages can host the site directly from the repository.

Option A — GitHub Actions

The repository already includes:

.github/workflows/pages.yml





Create a new GitHub repository.



Upload the contents of this folder to the repository.



Push the files to main.



Open Settings → Pages.



Under Build and deployment, select GitHub Actions if it is not already selected.



Open the Actions tab and wait for the Pages workflow to complete.



GitHub will provide the published site URL.

GitHub documents both branch-based publishing and GitHub Actions workflows for Pages. See: https://docs.github.com/en/pages/getting-started-with-github-pages

Option B — Publish from a branch

For a simple static site, GitHub Pages can also publish the repository directly from a selected branch/folder. Keep index.html at the top level of the publishing source.

Editing the site

Most content lives directly in index.html, so no build tool or framework is required.

Change contact information

Search for:

const CONTACT_EMAIL = "sanghamitra.ventures@gmail.com";
const FORM_ENDPOINT = "";



Add or remove projects

Update both:





the project cards inside the #projects section



the projects JavaScript array near the bottom of index.html

Keep the project number and array order aligned so the detail modal opens the correct project.

Change the logo

Replace:

assets/why-z-logo.png

with the updated logo while keeping the same filename, or update the <img src> path in index.html.

Design system

The visual system intentionally combines:





graph-paper background



wide grid spacing



black engineering-style borders



orange as the primary accent



monospaced technical labels



large editorial typography



browser-window project displays



asymmetric layouts



minimal gradients and no generic AI stock imagery

The goal is to make the site feel like a working lab + project network, not a conventional corporate portfolio.

Important security note

This repository is intended to be publicly deployable. Never commit:





API keys



SMTP credentials



passwords



private access tokens



database credentials



private agent credentials

Use a serverless function or trusted form provider for anything that requires a secret.

Credits / ecosystem references

The current site references project work and collaboration context involving:





Ashok Leyland



Ford



The Invincible Fire



Sanghamitra Ventures



student project teams

Project claims and metrics are presented as supplied project information and should be updated whenever the underlying project data changes.



WHY Z? = YZ=?Z
STUDENTS × COMPANIES × PROJECTS × AGENTS
