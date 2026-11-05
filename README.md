# Noyon Sheikh – Portfolio App (PWA)

Your portfolio as an installable app. It works offline after the first visit and installs on Android, iPhone and desktop.

## Files

- `index.html` – the portfolio (same look as `port.html`, plus an app-style bottom tab bar on phones)
- `manifest.json` – app name, colors and icons
- `sw.js` – service worker for offline use
- `icons/` – app icons (`icon.svg`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`)

## Before you publish

1. Copy your profile photo `FB_IMG_1747563290330.jpg` into the same folder as `index.html`.
2. In `index.html`, change `CONTACT_EMAIL` (near the bottom) to your real email address.
3. Replace the `#` links for LinkedIn, Twitter and Instagram in the footer with your own profiles.

## Host it free on GitHub Pages

1. Put all these files in your `noyon9o/Web` repo (keep the `icons` folder).
2. Repo **Settings → Pages → Deploy from a branch → `main` / root → Save**.
3. Open `https://noyon9o.github.io/Web/` after a minute.

## Install it

- **Android (Chrome):** tap **Install App** in the header, or the browser menu → *Install app*.
- **iPhone (Safari):** Share → *Add to Home Screen*.
- **Desktop (Chrome/Edge):** click the install icon in the address bar.

The app must be served over HTTPS (GitHub Pages does this) for install and offline mode to work.

## Updating

After you change files, bump `CACHE` in `sw.js` (for example `noyon-portfolio-v2`) so visitors get the new version.
