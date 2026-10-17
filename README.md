# DJ FUEL WEBDECK v0.2 - persistent library beta

Changes: IndexedDB MP3 persistence, automatic restore on reload, persistent library order, remove saved track, storage usage display, service worker for offline app shell when served over HTTPS. Existing cue and comment localStorage logic retained.

## Important
- **Not verified for live ceremonies**. Test on the actual iPad before relying on it. Bring a backup playback device.
- On iPad use HTTPS hosting (such as GitHub Pages) in Safari. `file://`/Files previews are not a reliable way to run the app. Service worker requires HTTPS.
- GitHub Pages on Free needs a **public** repository. Do not upload music to GitHub; only app files. Private development repo can remain private.
- Imported music is saved in the browser's IndexedDB, not the iPad Music app. iOS may evict website storage. Never delete browser website data or assume imported tracks are permanent; keep copies of all MP3s.
- First visit needs internet; later visits can load offline if the service worker has installed and cached successfully. Test airplane mode before a gig.
- Wi-Fi transfer from Windows is not yet implemented. Use Import Music on the iPad from Files.
- Long audio files may not show a detailed waveform to avoid memory pressure. Playback should still work.
- To update your existing hosted app, upload `index.html`, `manifest.webmanifest`, and `sw.js` to the web root. Reload online and test; offline caching may require an extra reload.
