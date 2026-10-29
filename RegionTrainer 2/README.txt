REGION TRAINER — INSTALLABLE IPHONE WEB APP

This is a private-use, installable Progressive Web App (PWA), NOT an App Store app.

IMPORTANT: iPhone Safari requires HTTPS for the offline service worker. Opening this
folder via a local Mac IP address over HTTP does not produce a working standalone
offline installation. You must serve these files at an HTTPS URL at least once.

EASIEST ONE-TIME SETUP (GitHub Pages)
1. Create a GitHub repository, for example "region-trainer".
2. Upload the CONTENTS of this folder into the repository root.
3. Under Settings > Pages > Build and deployment, choose "Deploy from a branch",
   branch "main", folder "/ (root)". Save.
4. Visit https://YOUR-USERNAME.github.io/region-trainer/ in iPhone Safari.
5. Keep the page open online until the bottom of the country selection screen
   says "All three maps saved for offline use". It may take a moment to load.
6. Tap Safari Share > Add to Home Screen > Add.
7. Launch the app from your Home Screen. You can now disconnect from Wi-Fi and
   cellular and use it without your computer running.

You don't need an Apple Developer account or App Store submission.
NOTE: On standard GitHub plans, GitHub Pages content is publicly accessible even if
it is just your personal quiz app. Avoid uploading personal data or secrets.
An alternate HTTPS host works too (for example, Netlify Drop).

The first visit must be online, and all three maps need to have loaded before
reliable offline use. iOS may discard locally stored web-app data if storage is
low; reconnect to restore it. For the clearest install experience, use Safari.

DESKTOP TESTING
cd to the folder, then run python3 -m http.server 8765
Open http://localhost:8765 on your Mac. Service workers work on localhost.

Map sources: geoBoundaries (CC BY 4.0), plus community geography sources.
Administrative boundaries may vary by provider and some are disputed.
