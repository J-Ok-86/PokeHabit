PokeHabit v1.7.130 · Android wrapper bridge support

1. Deploy index.html, moves.html, sw.js to your existing GitHub Pages /PokeHabit/ site.
2. PWA/Chrome remains independent and receives foreground-only reminders.
3. Separate Android WebView wrapper loads the same URL and schedules alarms using Android.
4. APK has its own browser storage; export JSON from PWA then import into APK.
5. Native bridge is injected only by trusted Android wrapper and is absent in ordinary Chrome.
6. Native JSON backup uses chunked transfer and Android file picker; import uses WebView file chooser.
7. First install requires internet; offline use after initial load depends on cached content.
8. APK build project is supplied separately.
