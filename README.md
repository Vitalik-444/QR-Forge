# QRForge

**Create. Scan. Connect.** QRForge is a client-side QR code studio built with React, TypeScript, Vite, Tailwind CSS, and Lucide React.

## Features
- Nine QR payload types: Website, Text, Wi-Fi, Contact/vCard, Email, Phone, SMS, Location, and Event.
- Live QR preview, foreground/background colors, presets, output sizes, quiet-zone controls, and optional center logo.
- Export to PNG, SVG, JPEG, and PDF.
- Scan QR codes from uploaded PNG/JPEG/WebP images or with a device camera.
- Local history with edit, download, rename, and delete actions.
- Batch generation from line-based data, exported as a ZIP.
- Responsive layout and grayscale QRForge brand palette.
- QR generation, scanning, and saved history stay in the browser.

## Requirements
- Node.js 18 or newer
- npm

## Run locally
```bash
npm install
npm run dev
```
Open the local URL shown by Vite. Camera scanning works on `localhost` and HTTPS deployments because browsers require a secure context for camera access.

## Production build
```bash
npm run build
npm run preview
```

## Batch format
Enter one item per line. Use `Title,content` to choose a filename. If no comma is present, the full line is treated as the QR content.

## Privacy
QRForge has no backend, account system, or external QR API. History is stored in local browser storage. The Google Fonts stylesheet is optional presentation-only network access; system font fallbacks remain available.
