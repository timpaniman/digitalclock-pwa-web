# Digital Clock (PWA Web)

A Progressive Web App version of the digital clock.

Same look as the other clock apps. Time and date come from **your device’s local clock** via JavaScript. GitHub Pages only hosts the files.

## Live site

https://timpaniman.github.io/digitalclock-pwa-web/

## What makes it a PWA

- `manifest.webmanifest` — name, icons, standalone display
- `sw.js` — service worker for offline/caching
- Installable from the browser (Add to Home Screen / Install app)

## Run locally

Open `index.html` in a browser, or:

```bash
npx serve .
```

For full PWA install behavior, use HTTPS or localhost.

## Install on a phone

1. Open the live site in Chrome
2. Browser menu → **Install app** or **Add to Home Screen**
3. Open it from the home screen (fullscreen, no browser chrome)

## Modify the UI

Edit `index.html` (HTML/CSS/JS). Icons are in `icons/`.

## License

MIT
