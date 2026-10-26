# Location-Gated Video (GitHub Pages)

This static page unlocks a video after the visitor taps **Check location**, grants browser location permission, and the browser obtains a location reading.

## Privacy and limitations
- Coordinates are intentionally ignored: they are not shown, saved, or transmitted.
- Geolocation requires HTTPS; GitHub Pages supports HTTPS.
- A website cannot switch the device's Location/GPS setting on. If location services are off, the visitor must enable them in device settings.
- Video playback is unlocked after a successful location reading; the visitor must press Play.
- This is a client-side gate, not strong access control: it can be bypassed by someone who knows web development. Do not use it to protect confidential video.

## Publish to GitHub Pages
1. Create a GitHub repository (for example `location-gated-video`).
2. Upload `index.html` to the repository root.
3. Upload your MP4 video to the same root folder and name it exactly `video.mp4`.
4. Open **Settings → Pages**.
5. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
6. Wait for the published HTTPS URL and open it on a phone.

No external libraries or server are required.
