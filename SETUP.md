# Going live with real accounts (Firebase)

Until these steps are done, Classroom Arena runs in **preview mode**: everything works, but accounts are stored only in the browser being used.

## 1. Create the Firebase project (about 10 minutes)
1. Go to <https://console.firebase.google.com> → **Add project** → name it `classroom-arena` (Google Analytics is optional).
2. **Build → Authentication → Get started → Sign-in method**, then enable:
   - **Email/Password** (teacher accounts)
   - **Anonymous** (students joining with a class code)
3. **Authentication → Settings → Authorized domains → Add domain:** `etothesmith.github.io`
4. **Build → Firestore Database → Create database** → *Production mode* → location `nam5 (us-central)`.
5. **Firestore → Rules:** paste the contents of `firestore.rules` from this repo → **Publish**.
6. **Project settings (⚙️) → Your apps → Web (`</>`)** → register an app named `Classroom Arena` → copy the `firebaseConfig` object.

## 2. Connect the app
Send the `firebaseConfig` to Claude, or paste it yourself into `index.html`: search for `const FIREBASE_CONFIG = null;` and replace `null` with the config object. Commit, and GitHub Pages updates in about a minute.

## Notes
- The Firebase SDK is **bundled inside `index.html`** — nothing loads from `gstatic.com`, so district web filters that block Google's CDN don't break it. The app does need to reach `firestore.googleapis.com` and `identitytoolkit.googleapis.com`.
- Password-reset emails come from Firebase; you can customize the email template under Authentication → Templates.
- Requests from the **For Schools** form are saved in Firestore under `leads`. View them in the Firebase console.
- The free Spark plan comfortably covers a pilot (50K reads/day, 20K writes/day).
