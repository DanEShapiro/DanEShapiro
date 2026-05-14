# Hi there 👋

I'm Dan — a back-end software engineer who builds and operates things end-to-end.

## 🛠️ Open Source Tools

- **[pin-unpin-all](https://github.com/DanEShapiro/pin-unpin-all)** — A Chrome extension that adds a button to pin or unpin all tabs in the window. Over 5,000 users.
- **[git-stash2d](https://github.com/DanEShapiro/git-stash2d)** — Stash the changes between two commits to the file system as human-readable patches. Great for saving branches to cloud storage and patching them back later — if a patch doesn't apply cleanly, the stash itself serves as a readable code reference.

## 🎸 [Everett Rock Rocks](https://everettrockrocks.com)

An interactive map of live music events north of Seattle. The backend scrapes and parses a PDF schedule, geocodes venues via Google Places, and decodes genre abbreviations. The frontend renders everything on a Leaflet map with filtering and search.

**Next.js · React · TypeScript · Flask · Leaflet · Google Places API · Docker**

## ⌚ Pebble Smartwatch Apps & Weather API

I built a watchface and an app for the Pebble smartwatch, which led me to build full weather and earth-data API's to power them.

### Watchfaces
- **[Day Marine US](https://apps.repebble.com/day-marine-us_5664e0d92369a756d700000a)** — A watchface for boaters showing tides (with rising/falling indicator), wind speed and direction, sunset time, temperature, and forecast. Displays a propeller loading graphic.
- **[Weather Text US](https://apps.repebble.com/weather-text-us_68fc478d54ffd600097bbb60)** — Displays a plain-text weather summary on the watch.

**C · Pebble SDK**

### Weather API
The backend that powers the watchface apps — serves smartwatch-friendly summaries including forecasts, tides, sunrise/sunset, and wind conditions. HMAC-authenticated, with request logging and monitoring built in.

**Python · Flask · Redis · Docker · OpenAI API · NOAA**

### [Platform](https://platform.ev0lut1on.com)
An admin dashboard for viewing API logs on an interactive map, tracking service health, and monitoring request patterns. Authenticated with Flask-Login and visualized with Leaflet marker clusters.

**Python · Flask · Leaflet · Docker**

## 🏠 [ev0lut1on.com](https://ev0lut1on.com)

My personal site and the support site for all of these projects, self-hosted on Azure.

**Next.js · React · TypeScript · Tailwind CSS**

## 📡 Monitor

A health and uptime monitor that runs scheduled checks against all ev0lut1on services — weather, platform, rocks, and the landing page. Authenticates where needed (HMAC for weather endpoints) and sends email alerts on failure. Self-monitoring via its own [`/health`](https://monitor.ev0lut1on.com/health) endpoint and [UptimeRobot](https://uptimerobot.com/).

**Python · Flask · SMTP · Docker**

## 🔧 Infrastructure

The shared infrastructure layer that ties everything together — Caddy as a reverse proxy with automatic HTTPS, plus Redis for caching, request logging, and temporary storage across services. Everything runs in Docker Compose.

**Caddy · Redis · Docker Compose**
