Steady — Recovery & Abstinence Tracker

A lightweight, single-file web app for tracking sobriety streaks, daily check-ins, and journal notes. Built as a focused example of designing for a sensitive use case: supportive without overstepping into medical advice.

Live demo

Open index.html directly in any browser, or host it with GitHub Pages (see below).

What it does


Streak tracker — a growth-ring progress visual that fills in as days are logged, with milestone markers at 1, 7, 30, 90, and 365 days.
Daily check-ins — quick-tap craving intensity and mood logging, plus a free-text note field.
Session log — a running list of check-ins for the current browser session.
Localized crisis resources — Kenya-specific support contacts (NACADA's 24/7 helpline, Kenya Red Cross, and a few accredited treatment centers), sourced from NACADA's public directory.


Why this design

The brief called for something calming rather than clinical, so the palette leans on sage and warm paper tones instead of typical "wellness app" gradients, with a tree-ring motif as the signature visual since it's a natural metaphor for accumulated, steady growth.

Deliberate scope limits

This app does not give medical or detox guidance. Withdrawal from some substances can be medically serious, and an app is the wrong place to offer that advice — the footer points to NACADA and Kenya Red Cross instead of attempting to simulate clinical support.

Tech

Plain HTML, CSS, and vanilla JavaScript. No build step, no dependencies. All data is held in memory (let variables in a <script> tag) and clears on page refresh — there's no backend or browser storage involved.

Running locally

bashgit clone https://github.com/<your-username>/steady-recovery-tracker.git
cd steady-recovery-tracker
open index.html   # or just double-click the file

Deploying with GitHub Pages


Push this repo to GitHub.
Go to Settings → Pages.
Under Source, select the main branch and / (root) folder.
Save — your app will be live at https://<your-username>.github.io/steady-recovery-tracker/.


Roadmap / next steps


Persist check-ins across sessions with a real backend (Supabase or Firebase).
Pull the resource directory live from NACADA's accredited-centers list instead of a hardcoded array, since centers and accreditation status change over time.
Add export-to-CSV for personal record-keeping.


Disclaimer

This is a portfolio/demo project, not a certified health tool. If you or someone you know needs support, please contact a licensed professional or one of the resources listed in the app.
