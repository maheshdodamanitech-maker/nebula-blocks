# Nebula Blocks

A block-puzzle mobile game, packaged with Capacitor and built into an
Android APK automatically by GitHub Actions — no Android Studio required.

## How the build works
Every time you push a change to the `main` branch (or click "Run workflow"
in the Actions tab), GitHub's own servers:
1. Install Node.js, Java, and the Android SDK
2. Wrap the game in `www/index.html` into a native Android project
3. Compile it into `app-debug.apk`
4. Attach that APK as a downloadable "artifact" on the finished run

## Getting your APK
1. Go to the **Actions** tab of this repository
2. Click the most recent workflow run (it should show a green checkmark
   once finished, usually 3-6 minutes)
3. Scroll down to **Artifacts** and download `nebula-blocks-debug-apk`
4. Unzip it — inside is `app-debug.apk`
5. Transfer that file to an Android phone and tap it to install
   (you'll need to allow "install unknown apps" for whichever app you
   use to open the file)
