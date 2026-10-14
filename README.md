# AS 532 AL Trainer

Study app for the AS 532 AL (ALe) Cougar: QRH emergency procedures (annunciators, failures by chapter, step drills) and RFM limitations and normal procedures, including the UZB appendix, with spaced-repetition review. Works offline; progress is saved on the device.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole app |
| `manifest.json`, `sw.js` | Install as a web app, offline support |
| `icon-*.png`, `icon.svg` | App icons |
| `debug.keystore` | Signing key for the Android APK (keeps updates installable) |
| `.github/workflows/build-apk.yml` | Builds the Android APK on GitHub (Actions tab) |
| `.nojekyll` | Tells GitHub Pages to publish files as they are |

## Android APK

Actions → **Build APK** → **Run workflow**. About 4–6 minutes later the APK is under **Releases** (`AS532-Trainer.apk`).
The workflow also runs by itself every time `index.html` changes.

## Website

Settings → Pages → Deploy from a branch → `main` / `(root)`.

## Updating the content

Replace `index.html`, and change `VERSION` in `sw.js` (for example `as532-v3`) so the website picks up the new copy.
