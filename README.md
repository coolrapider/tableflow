# TableFlow – Free Dining Arrangement & Table Turnover Manager

A free, no-install web tool that helps **small restaurants, cafés and food stalls** arrange seating, spot tables that are staying too long, and see how table use affects revenue.

Built for the *AI in Commerce* portfolio (CA1 Discover → CA2 Design → CA3 Build).

## Problem
Full tables do not always mean full revenue. Low-spend long stays (laptop users, groups chatting after the meal) block seats at peak time while dining groups leave the queue. TableFlow makes this visible and gives staff polite, data-backed actions.

## Features
- **Live floor view** – every table with colour status and a running timer (free / dining / meal finished / over limit / reserved)
- **Smart seating suggestion** – rule-based scoring: solo/laptop guests → communal tables, groups → booths, 1–2 guests → small tables
- **Waitlist** – suggests the best free table for each waiting party
- **Dwell alerts** – nudges when the dining limit or "meal finished, still seated" limit is crossed
- **Insights** – average stay, turns per table, RevPASH, lingering share, ₹ per seat-hour by table zone, CSV export
- **Zero cost, zero setup** – single `index.html`, no server, no database, no sign-up; data stays in the user's own browser (localStorage)

## Run locally
Open `index.html` in any browser.

## Host free on GitHub Pages
1. Create a new public repository and upload these files.
2. Go to **Settings → Pages**.
3. Under *Build and deployment* choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
4. After about a minute the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Important notes
- The **"Load SAMPLE data"** button creates *simulated* sessions for demonstration only – never present them as real results.
- Current AI scope: a rule-based recommendation engine (explainable, runs offline). Camera-based computer vision from CA1 is a **future extension**, not part of this build.
- Data is stored per device/browser; there is no cloud sync yet.

## Tests
18 automated browser checks were run with Playwright (seating logic, status engine, waitlist, clearing, RevPASH maths, persistence, no JS errors) – all passed on the build submitted.

## Licence
MIT – free for anyone to use and adapt.
