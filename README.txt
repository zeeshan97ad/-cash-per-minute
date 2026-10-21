CASH PER MINUTE - Android APK project

OPTION A: Build online (no installs needed)
1. Create a free account at github.com and make a new empty repository.
2. Upload ALL files from this folder, including the hidden .github folder
   (if the .github folder will not upload, use "Add file > Create new file",
   type the path .github/workflows/build-apk.yml and paste the file contents).
3. Open the repository's Actions tab. The "Build APK" workflow runs by itself
   (or click Run workflow). It takes about 5 to 8 minutes.
4. Open the finished run, download the "cash-per-minute-apk" artifact,
   unzip it and you get app-debug.apk.
5. Copy the APK to your phone, tap it, and allow "Install unknown apps".

OPTION B: Build on your computer
Needs Node 20, Java 17 and Android Studio.
  npm install
  npx cap add android
  npx cap sync android
  npx cap open android
Then in Android Studio: Build > Build APK(s).

Notes
- This makes a debug APK, fine for your own phone. Google Play needs a signed
  release build.
- To change the app, edit www/index.html and build again.
