# ZYNTRIX GAMES — Base44 Dev Environment

## Overview
Static website for ZYNTRIX GAMES (game developer/publisher), served by nginx via Docker Compose.

## Running
```
docker compose -f docker-compose.base44.yml up -d
```
Site is served on port 3000. Files are bind-mounted, so edits to `index.html`, `styles.css`, or `script.js` are reflected immediately (browsers refresh to pick up changes — there is no live-reload server).

## Structure
- `index.html` — main page (hero, games, news, projects, community sections)
- `styles.css` — all styling (dark gaming theme, responsive)
- `script.js` — navbar scroll effect, mobile menu, scroll reveal animations
- `docker-compose.base44.yml` — nginx:alpine serving the static files on port 3000

## No external credentials needed
This is a purely static site with no backend, database, or third-party API dependencies.
