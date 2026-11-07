JARVIS SMART DRESSING — PWA prototype 0.2

IMPORTANT
- This version is designed to run directly in the Samsung Galaxy Tab A browser.
- It does not require Raspberry Pi or a continuously running Lenovo.
- Clothing records and photos are stored in IndexedDB in the browser on the device.
- Do not clear browser/site data unless you have exported a backup.
- Voice recognition depends on browser support and may require internet. Text-based outfit selection works locally.
- This is a prototype; outfit matching currently uses simple local rules, not a generative AI model.

HOW TO TEST ON LENOVO
1. Unzip the project.
2. Open the folder in VS Code or another editor.
3. For a quick preview, use a local development server. A Python option:
   py -m http.server 8000
4. Open http://localhost:8000

HOW TO INSTALL AS AN APP ON ANDROID
A PWA requires HTTPS (or localhost) for service workers and reliable installation.
1. Publish these files to an HTTPS static host, for example GitHub Pages, using an account managed with a parent/guardian if needed.
2. Open the HTTPS address in Chrome on the Samsung tablet.
3. Use Chrome menu > Add to Home screen / Install app.
4. Open JARVIS from its icon.
5. Export a JSON backup occasionally from Settings.

LOCAL NETWORK NOTE
Opening this project at http://192.168.x.x is not considered a secure context by Android Chrome. The service worker/offline install feature may not work there. Use an HTTPS host for PWA installation. The app's data remains on the tablet browser, not on the hosting service.

DATA BACKUP
Settings > Exporter une sauvegarde downloads a JSON file containing the clothing details and photos. Keep a copy somewhere safe.
