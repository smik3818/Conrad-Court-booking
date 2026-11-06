# Conrad Maldives Court Booking

## Files
- `index.html` — the booking website.
- `manifest.webmanifest` — installable PWA information.
- `service-worker.js` — basic offline caching for the app shell.
- `icon-192.svg` and `icon-512.svg` — app icons.

## Publish with GitHub Pages
1. Upload all files from this folder into the **root** of your `Conrad-Court-booking` GitHub repository.
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/(root)**, then Save.
5. Wait for GitHub Pages to publish, then open the URL shown on that page.

## Important: live multi-device bookings are NOT connected yet
This version keeps bookings in the browser's `localStorage`. That means bookings are only stored on the device/browser where they were entered. The browser `storage` event does not sync different phones or computers.

To share bookings live between all staff devices, the next step is to connect a shared database such as Supabase or Firebase and add secure staff access. Do not use this version as the resort's shared production booking register until that is done.

## Current slot length
The supplied code creates 30-minute slots from 06:00 to 21:00. The code has been kept at 30-minute intervals in this package.
