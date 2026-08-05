# Portfolio — Zeyad Magdy Mogahed

A single-file static site. No build step, no dependencies to install.

## Files
- `index.html` — the homepage (HTML + CSS + JS in one file)
- `attack-disruption-lab.html` — case study, linked from the "Attack Disruption Lab" card
- `vm-deletion-lab.html` — case study, linked from the "VM Deletion Lab" card
- `resume.pdf` — your résumé, wired to the "Download résumé" buttons. Currently the fuller CV (`Zeyad_Magdy_CV`). Swap in the fixed LaTeX version later — just keep the filename `resume.pdf`, or update the `href="./resume.pdf"` references if you rename it.

All four files need to stay in the same folder — the case studies and résumé are linked with relative paths.

## Deploy it (pick one, all free)

### Option A — Netlify (fastest, zero setup)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag this whole folder onto the page
3. Done — you get a live URL in seconds. Add a custom domain later if you want, under Site settings → Domain management.

### Option B — Vercel
1. Push this folder to a GitHub repo (see below)
2. Go to [vercel.com/new](https://vercel.com/new), import the repo
3. Framework preset: "Other" — no build command needed. Deploy.

### Option C — GitHub Pages (lives right next to your code)
```bash
# from inside this folder
git init
git add .
git commit -m "portfolio site"
git branch -M main
git remote add origin https://github.com/Zeyad-Magdy/portfolio.git
git push -u origin main
```
Then on GitHub: repo → **Settings → Pages → Source: Deploy from branch → main / (root)**.
Your site goes live at `https://zeyad-magdy.github.io/portfolio/`.

## Before you share the link
- [ ] **VM Deletion Lab page has one placeholder claim, flagged in an amber callout box on the page itself:** your notes stop right before actually deleting a test VM and watching the pipeline fire. I wrote a plausible ending (rule fires within ~1 min → incident opens → playbook notifies the team) but I don't know what your playbook actually does. Run the real test, swap in the real outcome, delete the callout.
- [ ] Both case-study pages have `[ screenshot placeholder ]` boxes in the exact spots your original captions pointed to (e.g. "onboard the VM," "disable antivirus," "RDP session closed"). Drop your real screenshots into those and delete the dashed boxes.
- [ ] Double check job title: the site currently says **"M365 Security Engineering Intern."** Your full CV calls this role a full "Security Engineer" (no "Intern") — pick whichever is accurate and I'll match it everywhere.
- [ ] Skills list: your two CVs disagree on one language — one lists **C**, the other lists **Java**. I left both out where they conflicted; add whichever is actually current.
- [ ] Swap `resume.pdf` for your fixed LaTeX version once it's done.
