# Danest IT Consult website (PWA)

## 1. Firebase
1. Create a project at console.firebase.google.com and add a Web app.
2. Paste its config into `firebaseConfig` in `index.html`, and set `ADMIN_EMAIL`.
3. Authentication > Sign-in method: enable Email/Password. Add your user (same email as ADMIN_EMAIL).
4. Firestore Database: create it, then paste `firestore.rules` into the Rules tab (replace danestitconsult@gmail.com).
5. Authentication > Settings > Authorized domains: add `<username>.github.io` (and your custom domain, if any).

## 2. GitHub Pages
1. Create a repository and upload ALL files in this folder (keep the `icons` folder and `.nojekyll`).
2. Settings > Pages > Deploy from branch > main > / (root).
3. Site goes live at https://<username>.github.io/<repo>/

## 3. PWABuilder
1. Open pwabuilder.com and enter your live GitHub Pages URL.
2. Fix any warnings it shows, then Package for Stores (Android, Windows, iOS).
3. Android: PWABuilder generates a signing key. Keep it safe.
