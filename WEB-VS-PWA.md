# Web vs PWA Digital Clock

Short reference for the two browser-based clock apps:

| | Regular web | PWA web |
|---|---|---|
| **Repo** | [digitalclock-web](https://github.com/timpaniman/digitalclock-web) | [digitalclock-pwa-web](https://github.com/timpaniman/digitalclock-pwa-web) |
| **Live URL** | https://timpaniman.github.io/digitalclock-web/ | https://timpaniman.github.io/digitalclock-pwa-web/ |
| **UI** | Same dark green digital clock | Same UI |
| **Time source** | Device local time (`new Date()`) | Same |
| **Core file** | `index.html` | `index.html` |
| **Extra files** | None required | `manifest.webmanifest`, `sw.js`, `icons/` |
| **Installable** | No (bookmark only) | Yes (Install app / Add to Home Screen) |
| **Window** | Normal browser tab (URL bar visible) | Standalone window (no URL bar) when launched from install |
| **Offline** | Needs network for first load; no service worker | Cached via service worker after first visit |
| **Desktop shortcut command** | Opens the site URL in a browser | `chrome_proxy.exe --profile-directory=Default --app-id=<id>` (Chrome/Edge/Thorium) |
| **What it really is** | A static website | The same website + install metadata + offline cache |

## When to use which

- Use **regular web** for the simplest demo: one HTML file, open in any browser.
- Use **PWA web** when you want an installable icon and an app-like window without building a native `.exe` or APK.

## Important

Installing the PWA does **not** create a native Windows/Android binary. The browser still renders the page; it only hides most browser chrome and stores an app id in the browser profile under `Web Applications/`.
