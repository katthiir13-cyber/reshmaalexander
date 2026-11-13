# Speak English with Reshma — website

A static site: one `index.html` plus the `img/` folder. No build step.

## Deploy on Vercel (easiest: CLI, ~2 minutes)

1. Install Node.js (https://nodejs.org) if you don't have it.
2. Unzip this folder, open a terminal inside it, and run:

   ```
   npx vercel
   ```

   - Log in when asked (GitHub/Google/email).
   - "Set up and deploy?" → **Y**
   - "Which scope?" → your account
   - "Link to existing project?" → **N**
   - Project name → e.g. `speak-english-with-reshma`
   - "In which directory is your code located?" → `./`
   - It detects no framework ("Other"). Keep the defaults — no build command, no output directory.

3. That gives you a preview link. To publish the live site:

   ```
   npx vercel --prod
   ```

   Your site is now at `https://speak-english-with-reshma.vercel.app` (or similar).

## Deploy on Vercel (no terminal: via GitHub)

1. Create a new repository on github.com and upload everything in this folder
   (`index.html`, `vercel.json`, `img/`) using "Add file → Upload files".
2. On vercel.com → **Add New… → Project** → import that repository.
3. Framework preset: **Other**. Leave Build Command and Output Directory empty. Click **Deploy**.
4. Every time you upload a changed file to the repo, Vercel redeploys automatically.

## Custom domain (optional)

Vercel → your project → **Settings → Domains** → add `speakenglishwithreshma.com`
(or whatever you buy) and follow the DNS instructions shown there.

## Updating the site

Replace `index.html` (and any images in `img/`), then run `npx vercel --prod` again
(or upload the changed files to GitHub if you used that route).

## Still to connect before launch

- Waitlist forms only show a message right now; they don't save emails yet.
- "Book a trial class" / "Schedule a call" open Instagram DMs — swap in the Cal ID booking links.
- Pitch deck and WhatsApp buttons show "coming soon".
