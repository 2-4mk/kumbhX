# Kumbh Rakshak 2027 — patched build

## Files
- `index.html` — app with existing design and scripts plus targeted compatibility fixes.
- `safety.html` — standalone Safety Band QR landing page.

## Deploy to GitHub Pages
1. Upload both `index.html` and `safety.html` to the same folder in your repository.
2. Open **Settings → Pages**.
3. Select **Deploy from a branch**, choose your branch and `/ (root)`, then Save.
4. Wait for GitHub Pages to publish the site over HTTPS.
5. If your published URL differs, update `BASE_URL` in the `kr-consolidated-fixes` script in `index.html`.
6. Test registration and scanning on a second device.

## Notes
- Geolocation, camera, clipboard and share APIs require HTTPS or localhost in supported browsers.
- Demo account: phone `9000000000`, password `1234` (demo only).
- Data remains in each browser's localStorage and does not sync across devices. A shared backend is not connected in this patched build.
- The static Safety Band QR encodes the profile fields needed by `safety.html`. Anyone with the QR/link can view those details; do not encode sensitive information.
- This is not a security audit. Server-side authentication, verified password reset and cross-device data synchronization require a backend.
