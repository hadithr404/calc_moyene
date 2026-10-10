Calculate Moyen: build the Android APK with GitHub

1. Make a free account at github.com and sign in.
2. Click the + at the top right, then "New repository". Name it calculate-moyen
   and click "Create repository".
3. On the new repository page click "uploading an existing file".
   Drag the CONTENTS of this folder into the page (package.json,
   capacitor.config.json, www, .github, .gitignore), then click "Commit changes".
   Make sure the .github folder went up with the rest.
4. Open the "Actions" tab. A run called "Build APK" starts by itself and takes
   about 5 to 10 minutes. Wait for the green check.
   (If nothing runs, open "Build APK" in the left list and click "Run workflow".)
5. Click the finished run, scroll to "Artifacts" at the bottom and download
   calculate-moyen-apk. Unzip it to get app-debug.apk.
6. Send app-debug.apk to your phone and open it. Android will ask you to allow
   installing from that app (Files, Telegram, Chrome...). Allow it, then install.

If the run shows a red cross, open the failed step and send the error text to Claude.

The app is the same page as calculate_moyen_mobile.html. To change it, edit
www/index.html on GitHub and commit: a new APK is built automatically.
