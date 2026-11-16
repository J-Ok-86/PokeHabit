PokéRoutine V1.7.81 · Android Back/Exit confirmation fix

Changes:
- Android Back: dismiss dialog first, navigate to Today from other tabs, open in-app exit confirmation on Today.
- Modern Android Chrome: CloseWatcher handles hardware Back without depending on synthetic history entries.
- Fallback for browser/older engines: arm synthetic history only after genuine user interaction.
- Replaces window.confirm in popstate with a compact app-owned modal.
- When exit is approved, release Back interception. Due to PWA platform limitations, one more physical Back may be required to close.
- Existing reward, move skip, time log, account/JSON storage unchanged.

Update GitHub Pages: back up user JSON, upload index.html, moves.html, sw.js, then reload/PWA restart. Deployment is not performed by this archive.
