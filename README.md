# Kouzina Area Analysis

A web tool for the Kouzina BD team to analyse areas on a map. It is a finished static site: `index.html` contains all the code, data and libraries, except the population grid in the `pop/` folder.

**Open it here: https://shantanu1930.github.io/kouzina-area-analysis/**

Always open it from that link, not as a downloaded file. The free OpenStreetMap map servers it uses only answer pages opened from a web address, so a copy opened from your computer will not load maps or search.

## Updating the tool

Upload the new build's files (`index.html`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`) over the old ones in this repository (**Add file → Upload files** on `main`). The site updates on its own within a few minutes. There is no build step. Leave the `pop/` folder in place: the page loads it for the population card.

## Population data

"Population in this area" is an estimate: the [WorldPop](https://www.worldpop.org) 2025 India population grid (Global2 R2025A, 100 m, constrained; CC BY 4.0), summed to a 0.005° (~550 m) grid and cut into 1° tiles in `pop/` (about 9.4 MB in total). The page adds up the cells inside the chosen circle. WorldPop spreads people fairly evenly over built-up land, so the very densest cores (for example central Mumbai) may read low. City figures in the tool are still Census 2011.
