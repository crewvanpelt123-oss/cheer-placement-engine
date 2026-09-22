# Cheer Gym Tryout Evaluator

An automated team placement and roster management engine built for competitive cheer gyms. This application streamlines the annual tryout process by instantly sorting athletes into optimal teams based on their scores, ages, and USASF rules. Originally built to help a family owned gym reduce their tryout placement time from two weeks down to a couple of days.

## Key Features

* **Automated Smart Routing:** Instantly evaluates tryout data to place athletes on the most appropriate teams based on the USASF 2025 to 2026 Official Age Grid.
* **Flexible Data Import:** Supports direct copy and paste from spreadsheets or file uploads in CSV, TSV, TXT, and PDF formats.
* **Customizable Team Offerings:** Coaches can toggle specific USASF divisions on or off depending on the teams their gym plans to field for the season.
* **Rule Compliance Alerts:** Automatically flags crossover limit violations to ensure no athlete exceeds the maximum allowed routines per competition.
* **Tier Restrictions:** Prevents illegal roster combinations by locking Prep tier options when an athlete is already assigned to an Elite team.
* **Manual Override Console:** Provides a dedicated dashboard for coaches to review current scores, view all legal alternative placements, and manually edit team assignments.

## How It Works

1. **Load Data:** Drop your tryout roster file or paste the text directly into the application.
2. **Select Divisions:** Check the boxes for the specific divisions your gym is offering this season.
3. **Run Analysis:** The engine processes the roster and generates leaderboards.
4. **Refine:** Use the Edit Placement tool to make manual adjustments while the system tracks USASF compliance in real time.

## Tech Stack

* **Frontend:** Standalone HTML, CSS, and vanilla JavaScript application.
* **PDF processing:** PDF.js 3.11.174 loaded from the Mozilla CDN for in-browser PDF roster extraction.
* **Data handling:** Client-side CSV, TSV, TXT, and pasted-text parsing with no server-side runtime required.
* **Hosting:** Any static web server, including GitHub Pages.

## Run locally

From this directory, start a static server:

```sh
python3 -m http.server 4173
```

Open `http://127.0.0.1:4173/` in a browser.

The primary app is contained in `index.html`. `cheer_tryout_verified_v4.html` is preserved as the alternate standalone export found alongside the source material.