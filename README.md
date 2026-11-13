# Nerve Ledger — Cricket Pressure Dashboard

**Who actually holds their nerve?** An interactive analytics dashboard exploring how IPL and T20I players perform when the match is on the line.

## Dashboard

Once GitHub Pages is enabled, open the live dashboard here:

https://dhruvbansal0509.github.io/nerve-ledger-cricket-pressure-dashboard/

The dashboard is also available directly in the repository as [`index.html`](./index.html).

## What it explores

- **Ball-by-ball pressure:** Follow the chasing side's win-probability trajectory through a match and inspect high-leverage pressure zones.
- **Player rankings:** Compare the most reliable batters and bowlers under pressure, with player-level detail views.
- **Pressure vs. ordinary performance:** Explore which players improve or decline when the match becomes more demanding.
- **Robustness checks:** See how rankings hold up across alternative rule sets and repeated resampling.
- **Evidence and limitations:** Review pressure summaries, leverage patterns, and the model's stated caveats.

## Data coverage shown in the dashboard

The embedded dashboard data covers:

- 812 IPL and T20I matches
- 192,056 ball-by-ball records
- 891 players in the source summary
- Match dates from 22 January 2022 to 1 November 2026
- 38,200 balls classified as pressure balls using the dashboard's 1.4× leverage threshold

The figures above describe the dataset embedded in this dashboard.

## How to run

This is a self-contained HTML dashboard with its styling, JavaScript, charts, interactive controls, and embedded data in one file.

1. Clone or download this repository.
2. Open `index.html` in a modern web browser.

An internet connection is used for the Google Fonts referenced in the page; the dashboard's core content and embedded data are included in the HTML file.

## Publish with GitHub Pages

To provide judges with a browser-accessible dashboard:

1. Open the repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch **`Try`** and folder **`/(root)`**.
4. Save and wait for GitHub Pages to publish the site.

Live URL: https://dhruvbansal0509.github.io/nerve-ledger-cricket-pressure-dashboard/

## Methodology and caveats

The dashboard describes each delivery using a win-probability model and identifies pressure stretches from ball-level leverage. Player ratings and rankings are accompanied by resampling-based stability information and alternative-rule-set checks.

Please consult the **“How the rating is built”** section inside the dashboard for the on-page methodology details. Interpret rankings in light of the dashboard's eligibility and sample-size rules.

**Limitations stated by the dashboard:** the analysis uses only the supplied ball-by-ball, matches, competitions, and teams data pack. Contest-level and venue effects are not modelled. The ratings are analytical estimates, not definitive measures of a player's temperament.

## Repository contents

- `index.html` — complete interactive Nerve Ledger dashboard.
- `README.md` — project overview, data coverage, usage, methodology context, and publishing instructions.
