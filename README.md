# Tugas Pertemuan 8 - Implementasi Firebase Authentication

Aplikasi mobile berbasis Flutter yang terintegrasi dengan **Firebase Authentication** menggunakan metode Email & Password.

## Identitas & Pembagian Task
- **Fajar Islami** - Setup Firebase project, integrasi `firebase_auth`, halaman SplashScreen, Login, Register, dan Dashboard Home.

## Fitur Aplikasi
- **SplashScreen** (`lib/pages/splash_screen.dart`): Layar pembuka aplikasi dengan durasi 3 detik sebelum masuk ke halaman Login.
- **Login & Validasi** (`lib/pages/login_page.dart`): Autentikasi pengguna memakai `signInWithEmailAndPassword` lengkap dengan validasi input kosong serta dialog informasi UID dan Email.
- **Register Akun** (`lib/pages/register_page.dart`): Pendaftaran pengguna baru langsung ke Firebase Authentication menggunakan `createUserWithEmailAndPassword`.
- **Dashboard Home & Logout** (`lib/pages/home_page.dart`): Halaman utama setelah login berhasil yang menampilkan profil Email, UID, dan tombol Logout.

## Langkah Integrasi Firebase
1. Membuat project di **Firebase Console** (`myprojectfirebase-ca27e`) dan mengaktifkan metode login **Email/Password**.
2. Menjalankan `flutterfire configure` untuk menghasilkan file konfigurasi `lib/firebase_options.dart`.
3. Menambahkan dependency `firebase_core` dan `firebase_auth` di `pubspec.yaml`.
4. Menginisialisasi Firebase di `lib/main.dart` melalui `Firebase.initializeApp`.