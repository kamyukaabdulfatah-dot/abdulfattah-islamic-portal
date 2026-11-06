# عبد الفتاح | Islamic Portal

A responsive, static Islamic portal built with HTML, CSS and JavaScript.

## Features
- Arabic, English, French and Swahili interface
- Live clock and Gregorian/Hijri date display
- Location-based prayer times using the AlAdhan API
- Next-prayer countdown and upcoming-prayer highlight
- All 114 Quran surahs, with Arabic text
- Audio recitation with selectable reciters, play/pause, previous/next ayah, progress and playback speed
- Morning/evening adhkar with copy controls
- Tasbeeh counter saved in the browser on the current device
- Qibla bearing calculation based on device location

## Run locally
Open `index.html` in a browser. For geolocation, use HTTPS or localhost. Prayer times and location features need permission and an internet connection.

## Publish with GitHub Pages
1. Create a new repository on GitHub.
2. Upload `index.html` and this `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select **main** and **/(root)**, then save.
6. Wait for GitHub to publish the site. Your public URL will appear in the Pages section.

## APIs and notes
- Quran text and recitation: [AlQuran Cloud API](https://alquran.cloud/api)
- Prayer times: [AlAdhan API](https://aladhan.com/prayer-times-api)
- Prayer calculation method is currently set to method `3` (Muslim World League). Adjust it in `fetchPrayerTimes()` if your local authority uses another method.
- The Qibla display shows the bearing clockwise from true north. It is not a live magnetic compass sensor.
- External fonts, icons and APIs require internet access.
- This is a client-side static site. No personal location is sent to a custom server by this project; coordinates are used in the prayer-times API request.
