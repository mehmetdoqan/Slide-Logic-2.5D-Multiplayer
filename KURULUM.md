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


apiKey: "AIzaSyAf_evTEmSZ0Q30maUEBpznrm-3MuXq_kA",
  authDomain: "slide-logic-46078.firebaseapp.com",
  projectId: "slide-logic-46078",
  storageBucket: "slide-logic-46078.firebasestorage.app",
  messagingSenderId: "438427541870",
  appId: "1:438427541870:web:e4fa94260483921d4f617f"
