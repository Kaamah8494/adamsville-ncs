# Adamsville at the Crossroads

A neighborhood case study of Adamsville (NPU-H), Atlanta, built as a Quarto website in R.
CP 6036 Community Dynamics and Engagement, Georgia Tech, Fall 2026. Author: Faisal Kaamah Abdallah.

## Project layout

- `_quarto.yml`: site settings and navigation
- `index.qmd` ... `sources.qmd`: one page per chapter
- `data/`: ACS figures (ARC), places, timeline, and the NSA H02 boundary
- `images/`: archival scans (GSU Library) and photographs (Wikimedia Commons)
- `docs/`: the rendered website (created when you render; GitHub Pages serves this folder)

## How the site is published

The site is rendered and published automatically by GitHub Actions (`.github/workflows/publish.yml`).
Every time files are committed to the `main` branch on GitHub, the workflow installs R, Quarto and the
R packages, renders the site into `docs/`, and deploys it to GitHub Pages
(Settings > Pages > Source: GitHub Actions). Nothing needs to be rendered on a local computer.

Live site: https://kaamah8494.github.io/adamsville-ncs/

## Images

Archival scans are from Georgia State University Library digital collections. Recent photographs are
from Wikimedia Commons (open licenses), the websites of the organizations pictured, Homes.com and
Google Street View; non-openly-licensed images are used for educational purposes only and are credited
in captions and on the Sources page.
