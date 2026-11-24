# Adamsville at the Crossroads

A neighborhood case study of Adamsville (NPU-H), Atlanta, built as a Quarto website in R.
CP 6036 Community Dynamics and Engagement, Georgia Tech, Fall 2026. Author: Faisal Kaamah Abdallah.

## Project layout

- `_quarto.yml`: site settings and navigation
- `index.qmd` ... `sources.qmd`: one page per chapter
- `data/`: ACS figures (ARC), places, timeline, and the NSA H02 boundary
- `images/`: archival scans (GSU Library) and photographs (Wikimedia Commons)
- `docs/`: the rendered website (created when you render; GitHub Pages serves this folder)

## Render it

1. Install R, RStudio and Quarto (https://quarto.org/docs/get-started/).
2. Open `adamsville-ncs.Rproj` in RStudio.
3. In the Console, install the packages once:

   ```r
   install.packages(c("readr", "dplyr", "tidyr", "ggplot2", "leaflet",
                      "jsonlite", "htmltools", "visNetwork", "tibble"))
   ```

4. In the Terminal tab, run `quarto render` (or click **Build > Render Website**).
5. The finished site is in `docs/`. Open `docs/index.html` to check it.

## Put it on GitHub and publish

1. Create a new **public** repository on github.com named `adamsville-ncs` (no README).
2. In the RStudio Terminal, inside this folder:

   ```bash
   git init
   git add .
   git commit -m "Adamsville neighborhood case study"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/adamsville-ncs.git
   git push -u origin main
   ```

3. On GitHub: **Settings > Pages > Build and deployment**, Source: *Deploy from a branch*, Branch: `main`, folder `/docs`. Save.
4. After about a minute the site is live at `https://YOUR-USERNAME.github.io/adamsville-ncs/`.
5. After any edit: render again, then `git add . && git commit -m "update" && git push`.
