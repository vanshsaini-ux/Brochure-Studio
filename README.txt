BROCHURE STUDIO - DEPLOY TO VERCEL (no build step)
==================================================
Files: index.html (the app), vercel.json (settings), library/ (shared pictures)

ROUTE A - GitHub (recommended, no coding)
  1. github.com -> New repository (name: brochure-studio) -> Create.
  2. On the repo page: "uploading an existing file" -> drag in index.html, vercel.json and the library folder -> Commit changes.
  3. vercel.com -> Add New -> Project -> Import your repo.
  4. Framework Preset: Other. Build Command: leave empty. Output Directory: leave empty. -> Deploy.
  5. Open the link Vercel gives you.

ROUTE B - Command line (needs Node.js installed)
  1. Open a terminal INSIDE this folder.
  2. Run:  npx vercel        (log in, accept the defaults)
  3. Run:  npx vercel --prod (gives the final public link)

UPDATING LATER
  Replace index.html (and/or the library folder) -> commit on GitHub (Route A) or run npx vercel --prod (Route B). Vercel redeploys automatically from GitHub.

SHARED PICTURE LIBRARY (whole team)
  - In the app click Library, add logos/photos/portraits.
  - Click "Export for Vercel (team library)" -> brochure-library-for-vercel.zip
  - Unzip it into this folder so you have library/manifest.json plus the pictures, then redeploy.
  - Everyone sees them under "Shared with team". "My library" stays only in each person's own browser.

NOTES
  - Each person's work (autosave, Projects) is saved in their own browser. Use Export JSON / Backup to move work between computers.
  - The app loads html2canvas, jsPDF and Google Fonts from public CDNs, so users need internet for PDF export and fonts.
