IZYPAYS SCHOOL CRM — PWA

UPLOAD ALL FILES AND THE icons FOLDER TO THE ROOT OF A GITHUB REPOSITORY OR YOUR GITHUB PAGES SITE.

FILES:
- index.html: the CRM application
- manifest.webmanifest: installable PWA metadata
- sw.js: offline app-shell cache
- icons/: app icons

IMPORTANT:
1. Host over HTTPS (GitHub Pages does this automatically).
2. Open the published site in Chrome on Android.
3. Use the browser menu > Install app / Add to Home screen.
4. The school database uses IndexedDB, which persists across normal app/browser restarts on the same device and browser profile.
5. The app can migrate records from the previous CRM's Local Storage if that older app was opened in the same browser origin. If the old version was opened from a different file:// URL or different browser, export its CSV and import it into this version.
6. Export CSV regularly. Local data is not cloud-synced and is not shared across devices.
7. If you replace the app files in a deployed site, refresh the app; the service worker updates the app shell.

DEFAULT STATUS: Yet to contact.
OTHER STATUSES: Contacted, Started, Paying.
