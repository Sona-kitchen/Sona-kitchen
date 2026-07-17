# Sona Kitchen PWA

Single-page mobile-first food ordering web app for Sona Kitchen, built as a Progressive Web App that can be installed on Android and wrapped for Google Play.

## Features

- Beautiful mobile-first single-page ordering experience
- Category filters, search, cart, and checkout flow
- Local cart persistence with `localStorage`
- Installable PWA with manifest and service worker
- Offline-friendly app shell caching
- Ready to wrap with Android WebView or Trusted Web Activity

## Files

- `index.html` — complete app UI, styles, and client logic
- `manifest.webmanifest` — PWA metadata
- `service-worker.js` — offline caching

## Run locally

Because service workers require a web origin, serve the folder with a local static server.

Examples:

- `npx serve .`
- `python -m http.server 8080`

Then open `http://localhost:8080`.

## Google Play wrapping options

### Trusted Web Activity

Best when hosting the PWA online with HTTPS and full PWA compliance.

### WebView wrapper

Best when packaging the local web app inside a lightweight Android shell.

## Notes

- Menu data is currently embedded in `index.html` for a simple single-file app structure.
- Replace demo menu items and checkout handling with your real backend or WhatsApp/payment integration when ready.