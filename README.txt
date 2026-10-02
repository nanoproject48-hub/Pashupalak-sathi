PASHUPALAK SATHI (React web app / PWA) - Google + Email login

KYA CHAHIYE (sirf ek baar):
1. Firebase Console > Authentication > Sign-in method > GOOGLE enable karo (+ Email/Password bhi).
2. Is app ko kisi https website par daalo (neeche), phir uska domain
   Firebase Console > Authentication > Settings > Authorized domains mein ADD karo.
   (Bina iske Google login "unauthorized-domain" error dega.)
3. Firestore rules: Dairysathii zip wali firestore.rules Publish karo.
4. Agar Google Cloud Console mein API key par "Android apps" restriction lagi hai to hata do
   (ya "Websites" mein apna domain daalo).

HOSTING (koi ek):
- GitHub Pages: nayi repo banao, in 4 files upload karo (index.html, manifest.json, icon-192.png, icon-512.png),
  Settings > Pages > main branch. Domain: <username>.github.io
- Netlify Drop (app.netlify.com/drop): folder drag-drop.
- Firebase Hosting: firebase deploy (computer / CLI chahiye).

PHONE PAR INSTALL: Chrome mein site kholo > menu > "Add to Home screen" / "Install app".

NOTE: Google login Android WebView ke andar nahi chalta (Google block karta hai), isliye ise
Chrome / home-screen app ki tarah chalao, AIDE app ke WebView mein nahi.
