# Abdulfattah Islamic Portal v3

Upload all files in this folder to the root of your GitHub Pages repository.

## Features
- Arabic, English, French and Luganda interface
- All 114 Quran surahs in Arabic
- Reciter selector and ayah-by-ayah audio with optional automatic next ayah
- Location-based prayer times, selectable calculation method and next-prayer countdown
- Browser prayer notifications while the page remains open
- Qibla bearing calculation and optional device compass
- Tasbeeh saved with localStorage
- Ramadan panel and curated daily hadith cards with references
- Dark/light theme, adjustable website/Arabic/brand fonts
- Browser speech commands with an animated glow only while microphone recognition is active
- PWA manifest, icon and service worker

## GitHub Pages deployment
1. Extract this ZIP.
2. In your repository choose **Add file → Upload files**.
3. Upload `index.html`, `manifest.json`, `sw.js`, `icon.svg`, and `README.md` into the repository root.
4. Commit to `main`.
5. Open **Settings → Pages**, choose **Deploy from a branch**, `main`, `/(root)`, then Save.

## Important limitations
- Use the HTTPS GitHub Pages URL for geolocation, notifications, microphone and installation.
- Notifications work only while this page is open. Background push notifications after the browser is closed need a server/push service and are not included.
- The voice glow reflects real browser speech-recognition listening; it is not connected to Gemini or a Gemini API. Browser support varies.
- Quran text/audio uses AlQuran Cloud; prayer calculations use AlAdhan. Internet is needed for fresh data and audio.
- Device compass support varies by phone/browser and may need calibration.
- The PWA caches the app shell only. Quran, audio and prayer API data need internet.
- Prayer method defaults to Muslim World League. Choose the method used by your local mosque or authority.
- Daily hadith entries include references; verify against trusted editions before quoting or republishing.
