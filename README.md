# Neuron School (Android app)

A web app that teaches C++ and neural networks, wrapped with Capacitor so GitHub can build it into an APK.

## Get your APK
1. Create a new empty repository on github.com.
2. Upload this project. The folder `.github` is hidden, so the easiest way is git:
   ```
   git init
   git add .
   git commit -m "First commit"
   git branch -M main
   git remote add origin https://github.com/YOUR-NAME/YOUR-REPO.git
   git push -u origin main
   ```
3. Open the **Actions** tab. The "Build Android APK" workflow starts by itself (about 5 to 8 minutes). You can also run it with **Run workflow**.
4. When it finishes, open the run and download **neuron-school-apk** under Artifacts. Unzip it to get `app-debug.apk`.
5. Copy the APK to your phone and open it. Android will ask you to allow installs from unknown sources.

## Change the app
Edit `www/index.html`, push to GitHub, and download the new APK.

## Notes
- The APK is a debug build. That is fine for installing on your own phone. Publishing to Google Play needs a signed release build.
- To rename the app, edit `appName` and `appId` in `capacitor.config.json`.
