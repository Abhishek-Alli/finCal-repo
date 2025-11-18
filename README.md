# finCal — Financial Calculator Suite

finCal is a responsive, client-side web application that provides multiple financial calculators to help with investment planning and loan calculations. It is built with plain HTML, CSS, and JavaScript and uses Chart.js (CDN) for visualizations.

Live demo: run locally (see Run section).

Features
 - SIP (Systematic Investment Plan) calculator with growth chart and Invested vs Returns donut chart
 - Lumpsum calculator
 - SWP (Systematic Withdrawal Plan) calculator with corpus projection and donut chart
 - EMI calculators for Home / Car / Bike loans (monthly EMI, principal vs interest visualization)
 - Retirement planner (corpus & savings estimate)
 - Interactive sliders and synced input fields for parameters
 - Charts (Chart.js) for visual breakdowns (doughnut charts) and timelines

Files
 - `swp-sip/index.html` — Main application entry (all UI, styles, and scripts in a single file)
 - `index.html` — (legacy / optional)
 - `script.js` — (legacy / optional)

Run locally
1. Open the project folder in a terminal (PowerShell on Windows):

```powershell
cd "c:\Users\abhis\Desktop\sip calculator\swp-sip"
python -m http.server 8000
```

2. Open your browser and go to `http://localhost:8000`.

3. Use the top navigation or the home tabs to switch calculators. Adjust sliders or input values — charts and results update live.

Notes about dependencies
- Chart.js is loaded from CDN in `swp-sip/index.html`.
- Font Awesome is loaded from CDN for icons.

Development notes
- The app is a static, client-side site. For production consider splitting CSS/JS into separate files and bundling/pinning dependencies.

Committing & pushing to GitHub
If your project is a git repository and has a remote configured, you can commit and push the updated README with these commands (PowerShell):

```powershell
cd "c:\Users\abhis\Desktop\sip calculator"
git add README.md
git commit -m "docs: update README for finCal"
# Check remote and current branch
git remote -v; git branch --show-current
# Push (replace `main` with your branch if different)
git push origin main
```

If you don't have a remote configured, add one (replace with your repo URL):

```powershell
git remote add origin https://github.com/<username>/<repo>.git
git branch -M main
git push -u origin main
```

If push fails due to authentication, configure your Git credentials (SSH key or personal access token) and try again.

License & attribution
 - This project uses libraries loaded from CDNs (Chart.js, Font Awesome). Review their licenses for redistribution.

Contact
 - For questions, email: `support@fincalcpro.com`

---
Created/updated by the development toolchain in the workspace.
