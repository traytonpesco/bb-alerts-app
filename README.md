# BB Alerts

View-only alerts for the SecretLab machines in BB Cloud dev. Watches the
incident feed around the clock and pushes an immediate notification for any
**vend failure** (or other machine incident) — on wifi or mobile data.
Nothing is ever changed in the cloud.

**Live app:** https://traytonpesco.github.io/bb-alerts-app/

## Install on iPhone

1. Open https://traytonpesco.github.io/bb-alerts-app/ in **Safari**, then tap
   Share → **Add to Home Screen** (required for iOS push notifications).
2. Open the installed **BB Alerts** app from your home screen and tap
   **Enable push alerts on this device**.
3. Tap **send test push** — you should get a notification within seconds.

That's it. FAILURE and WARNING alerts arrive automatically from then on,
whether the app is open or not.

## Notes

- This repo contains only the built app. Source lives in the private
  `bb alerts` project (see its `PRD.md` / `README.md`).
- The app contains no portal credentials — it reads a mirrored feed from a
  read-only backend. Anyone with the link can view the feed and subscribe to
  alerts, so share it only with people who should receive them.
- Times are shown relative and in UK time (the portal's timezone).
