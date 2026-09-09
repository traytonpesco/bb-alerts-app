# BB Alerts

View-only alerts for the SecretLab machines in BB Cloud dev. Watches the
incident feed around the clock and pushes an immediate notification for any
**vend failure** (or other machine incident) — on wifi or mobile data.
Nothing is ever changed in the cloud.

**Live app:** https://traytonpesco.github.io/bb-alerts-app/

## Install on iPhone

1. Ask a team member to add you (in the app: **Settings → Team access**).
   They'll give you a temporary password — no email is sent.
2. Open https://traytonpesco.github.io/bb-alerts-app/ in **Safari**, then tap
   Share → **Add to Home Screen** (required for iOS push notifications).
3. Open the installed **BB Alerts** app, sign in, and change your password
   under **Settings → Your account**.
4. Tap **Enable push alerts on this device**, then **Test push** — you should
   get a notification within seconds.

FAILURE and WARNING alerts arrive automatically from then on, whether the
app is open or not — while monitoring is **active**.

## Active vs inactive

Monitoring follows the event: in **Auto** mode it runs from the day before
the event start date to the day after the end date (set in **Settings →
Monitoring**), and can be forced **Active** or **Inactive**. When inactive
there is no polling, no pushes and no watcher warnings; the history stays
visible and the header shows **Inactive**.

## Notes

- This repo contains only the built app. Source lives in the private
  `bb alerts` project (see its `PRD.md` / `README.md`).
- Access is team-only: you must sign in and be on the team allowlist. The app
  contains no portal credentials — it reads a mirrored feed from a read-only
  backend.
- Times are shown relative and in UK time (the portal's timezone).
