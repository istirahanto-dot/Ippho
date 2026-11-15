# ippho — Kubus 3×3

Game Rubik 3×3 untuk Android. Nama aplikasi: **ippho**.

- Kubus 3D digeser untuk memutar, tombol Acak / Urungkan / Notasi, timer + penghitung langkah.
- Bisa dimainkan tegak maupun miring (mode landscape: kubus di kiri, tombol di kanan).
- Game tersimpan di dalam aplikasi, jadi bisa dimainkan offline.

## Build (GitHub Actions)

1. Push kode ke branch `main` → APK jadi di Artifacts (`ippho-debug-apk`).
2. Untuk dibagikan ke teman: buat tag `v1` (lalu `v2`, ...) → otomatis dibuat
   **Release** dengan file `app-debug.apk` terlampir. Teman mengunduhnya dari
   halaman Releases (repo harus **Public** supaya bisa diunduh tanpa login GitHub).

## Struktur

- `app/src/main/assets/rubik-3x3.html` — game lengkap satu file (Three.js di dalamnya)
- `app/src/main/java/id/ippho/MainActivity.kt` — WebView pemutar game
- `app/src/main/res/mipmap-*` — ikon launcher kubus
