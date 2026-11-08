# Ay Kilidi – Firebase + GitHub Pages kurulumu

1. https://console.firebase.google.com → "Proje ekle" (Analytics gerekmez).
2. Build → Authentication → Başlayın → Sign-in method:
   - "Anonymous" (Anonim) → Etkinleştir
   - "Email/Password" → Etkinleştir
   Users sekmesi → "Add user": öğretmen e-postası + güçlü şifre (en az 6 karakter). Bu hesap öğretmen paneli içindir.
3. Build → Firestore Database → Create database (production mode, size yakın bir bölge, örn. eur3).
   Rules sekmesine firestore.rules içeriğini yapıştır, OGRETMEN_E_POSTASI_BURAYA yerine 2. adımdaki e-postayı yaz → Publish.
4. Proje ayarları (⚙) → Genel → "Web uygulaması ekle (</>)" → verilen firebaseConfig değerlerini al.
5. index.html içinde FIREBASE_CONFIG bölümüne apiKey, authDomain, projectId, appId değerlerini yapıştır.
6. Authentication → Settings → Authorized domains: kullaniciadin.github.io ekle.
7. index.html'i GitHub deposuna yükle, Settings → Pages → main / root.
