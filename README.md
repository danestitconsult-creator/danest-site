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

## 4. Learning platform (learn.html)
1. Firebase > Storage > Get started (needs the Blaze plan on new projects; set a budget alert). Paste `storage.rules` in the Storage Rules tab and Publish.
2. Firestore > Rules: paste the updated `firestore.rules` and Publish.
3. Open `learn.html`, sign in with the admin email, and use the Facilitator dashboard:
   - Subscription settings: set price, days of access, payment link/MoMo instructions.
   - Courses & materials: add a course, add lessons (video/slides link, uploaded PDF/image/audio/video, or written lesson), then Publish the course.
   - Payments: approve a learner's payment reference to activate their access. Learners tab can also grant or revoke days manually.
4. Export PowerPoint decks to PDF before uploading; they display slide-by-slide inside the site.
