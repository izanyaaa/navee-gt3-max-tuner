# ESCOOTER TUNER — NAVEE GT3 Max

A static HTML prototype for Bluetooth discovery and read-only GATT diagnostics.

## Publish it (free option: GitHub Pages)

1. Sign in to GitHub and create a **new public repository** named `navee-gt3-max-webapp`.
2. Upload `index.html` from this folder to the repository root and commit it.
3. Open **Settings → Pages**.
4. Under build/deployment, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then save.
5. Wait for GitHub Pages to publish. The site URL will be shown in Settings → Pages.
6. On iPhone, open the HTTPS URL in an iOS browser that explicitly supports Web Bluetooth (for example Bluefy). Safari on iOS does not expose Web Bluetooth.

## Current scope

- Requests a Bluetooth device named with the `NAVEE` prefix, or optionally lists all devices.
- Attempts a GATT connection and lists services/characteristics exposed by the browser.
- Attempts reads and notifications only where the device reports those capabilities.

## Important limitations

- The real NAVEE GT3 Max protocol has not been validated against a physical scooter in this project.
- The browser may require services to be explicitly allow-listed; service discovery can therefore be incomplete.
- Live telemetry decoding and model-specific controls are not implemented yet.
- No write commands, speed unlocking, firmware updates, or safety-critical changes are sent.
- Use diagnostics while stationary and keep the official app closed during testing if pairing conflicts occur.

GitHub Pages publishes this repository as a public website. Do not upload secrets or personal information.
