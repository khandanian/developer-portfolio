# khandanian — Portfolio 2.0

A Persian-first, RTL, responsive showcase for **10 real GitHub repositories**.

## Live portfolio
https://khandanian.github.io/developer-portfolio/

## Included repositories
1. [developer-portfolio](https://github.com/khandanian/developer-portfolio)
2. [smart-business-dashb](https://github.com/khandanian/smart-business-dashb)
3. [taskflow-pwa](https://github.com/khandanian/taskflow-pwa)
4. [autofinder-ira](https://github.com/khandanian/autofinder-ira)
5. [moneyflow-pwa](https://github.com/khandanian/moneyflow-pwa)
6. [clienthub-crm](https://github.com/khandanian/clienthub-crm)
7. [novashop-store](https://github.com/khandanian/novashop-store)
8. [bookify-booking](https://github.com/khandanian/bookify-booking)
9. [stockpilot-inventory](https://github.com/khandanian/stockpilot-inventory)
10. [teamforge-projects](https://github.com/khandanian/teamforge-projects)

## Portfolio features
- Responsive dark visual design and Persian RTL interface
- 10 project cards with direct source and expected GitHub Pages demo URLs
- Category filters, instant search and accessible buttons
- Project-specific descriptions, technology labels and graphic illustrations
- SEO description, Open Graph metadata and keyboard skip link
- No external JavaScript dependencies, no backend or secrets

## Audit (2026-11-08)
All 10 repositories were inspected for their default-branch file tree and most recent GitHub Actions runs. Every repository contains an HTML entry point, stylesheet, JavaScript, README and Pages deployment workflow. `taskflow-pwa` and `moneyflow-pwa` additionally include a manifest and service worker. The latest Actions run for each of the 10 repositories was **completed/success** when checked. This is **not** a browser-based functional audit or guarantee of live site availability. Older runs include failures in some repositories. Demo links assume GitHub Pages uses the conventional project URL; verify live availability separately.

## Architecture and limitations
Each showcased app is a separate portfolio demonstration. Most persist data locally in the browser and do not have server-side authentication, shared databases or multi-user synchronization. Some use fictional seed data. The portfolio does not claim production readiness.

## Local preview
Open `index.html` or run `python -m http.server 8080`.

## Deployment
The existing `.github/workflows/deploy.yml` remains unchanged. In **Settings → Pages**, choose **GitHub Actions** as the source. The workflow deploys the static `main` branch.

## Update projects
Edit the `projects` array in `assets/app.js`. The filters and cards update automatically.
