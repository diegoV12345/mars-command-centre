# MARS — Home Screen PWA (v1)

This is a functional local-first Progressive Web App. It uses HTML, CSS, JavaScript, a web manifest, app icons, and a service worker. No npm, build step, or computer required.

## Host using only iPad/iPhone (GitHub Pages)

1. In Safari, sign in to https://github.com and create a new repository named `mars-command-centre` (public for free GitHub Pages). **Do not upload personal financial data, secrets, API keys, or private files.**
2. Open the repository's **Add file > Upload files** screen. In iPad Files, unzip this archive, open the `MARS-PWA` folder, and select/upload all eight app files from INSIDE that folder (not the ZIP itself and not the enclosing folder). Ensure `index.html` is at the repository root. Commit changes. If selecting multiple files is difficult, use Safari's Request Desktop Website or upload in batches.
3. In the repository, go to **Settings > Pages**. Set **Source: Deploy from a branch**, **Branch: main**, **Folder: /(root)**, then Save.
4. After deployment, open `https://YOUR-GITHUB-USERNAME.github.io/mars-command-centre/` in Safari. The GitHub Pages screen in Settings will also show the exact live URL.
5. Tap **Share > Add to Home Screen**, enable **Open as Web App**, then **Add**. Repeat on the second device.

## Features
- Home Screen standalone experience and offline shell after first successful visit.
- Local account balances, liabilities and net worth in CAD.
- Tasks/missions stored in browser localStorage.
- Offline scripted Mars chat and spoken replies using speech synthesis when supported.
- Experimental speech recognition button (browser support varies; use keyboard dictation as fallback).

## Limitations and security
- This is NOT a hosted app until you deploy it. No real AI model or banking integration is connected.
- The published static site is public. Do not place personal data or credentials in the repository.
- Account balances and missions are saved ONLY on the current device/browser storage, not synced between devices; storage can be cleared by iOS or user actions. There is no authentication or encryption of local data beyond device/browser protections. **Do not enter sensitive real banking information in this public prototype**; use non-sensitive test amounts.
- A real private version needs authenticated backend, encrypted server storage, explicit consent, read-only financial aggregator access, and secure server-held API credentials. Never embed banking tokens or AI API keys in these files.
- A true always-listening wake phrase is not supported by this PWA in the background.
