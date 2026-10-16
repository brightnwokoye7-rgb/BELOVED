# BELOVED: installable app (Light Developers)

BELOVED installs on a phone like a normal app, works offline once opened, and signs people in with Firebase.

## Put it online (free, phone only)
1. Unzip this file with your phone's Files app.
2. Sign up at github.com. Create a **New repository** named `beloved` and set it to Public.
3. On the new repository, tap **uploading an existing file**. Select ALL the unzipped files (index.html, firebase-config.js, manifest.webmanifest, sw.js and the four .png icons), then tap **Commit changes**.
4. Open **Settings > Pages**. Under Source choose **Deploy from a branch**, pick branch **main** and folder **/ (root)**, then Save. After a minute or two your address appears: `https://YOURNAME.github.io/beloved/`

## Make sign-in work
1. In the Firebase console create a project, add a Web app, and copy its settings into `firebase-config.js`. You can edit it on GitHub with the pencil icon, or send the settings to Claude to rebuild the file for you.
2. Authentication > Sign-in method: turn on Google and Email/Password. Phone is optional and sends SMS, so check Firebase's current pricing first.
3. Authentication > Settings > Authorized domains: add `YOURNAME.github.io`.

## Install on a phone
Open your address in the browser.
- **Android (Chrome):** BELOVED Settings (sliders icon) > Install, or browser menu > Install app.
- **iPhone (Safari):** Share button > Add to Home Screen.

## Offline
After the first visit with internet, the app opens with no internet. Daily scriptures, the saved Bible passages, scriptures for a challenge, and returning users all work offline. Online-only: first sign-in, Bible chapter pages, songs, and teacher links.

## Updating later
Upload the new files to the same repository. In `sw.js` change `beloved-v1` to `beloved-v2` so phones pick up the new version.

## Notes
- The AI scripture picker only runs inside Claude. On your own address the app uses the built-in scripture list.
- You need a privacy policy, because the app collects emails and phone numbers.
