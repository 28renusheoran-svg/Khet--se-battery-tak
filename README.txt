# Khet Se Battery Tak — Phone App

This is a Progressive Web App (PWA) package for the science exhibition project.

## Features
- Energy dashboard with manual readings
- Peltier / steam turbine / micro-hydro power calculations
- Parali Mitra estimates
- Silica yield calculator
- Experiment log with CSV export
- Installable on compatible phones and supports offline loading after first visit

## Important
The app currently uses manual entry and illustrative sample readings. It is not connected to the ESP32 or physical sensors yet. The emission factor and all demonstration readings should be replaced with locally verified assumptions and measured results.

## How to make a QR code that works for everyone
A QR code needs a public HTTPS link. This package is not yet hosted online, so a public download QR cannot be finalized until the folder is uploaded to a hosting service.

### Simple hosting option: GitHub Pages
1. Sign in to GitHub and create a new public repository, for example `khet-se-battery-tak`.
2. Upload all four files from this folder (`index.html`, `manifest.json`, `service-worker.js`, `icon.svg`) to the repository root.
3. In the repository, open **Settings → Pages**.
4. Choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. GitHub will provide a public HTTPS address, usually `https://YOUR-USERNAME.github.io/khet-se-battery-tak/`.
6. Open that address on a phone. On Android Chrome, choose **Install app** or **Add to Home screen**. On iPhone Safari, use **Share → Add to Home Screen**.
7. Use the final HTTPS address to generate the QR code. Anyone who scans it can open the app and install it.

For a QR that downloads the ZIP itself, upload the ZIP to a public file host and make a QR from its direct public download URL. For the best phone experience, use the hosted app URL instead of a ZIP-download QR.

## Local testing
You can open `index.html` directly for basic testing, but install/offline PWA features require HTTPS hosting (or localhost).
