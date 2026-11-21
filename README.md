# Tugas Pertemuan 8 - Implementasi Firebase Authentication

Aplikasi mobile berbasis Flutter yang terintegrasi dengan layanan **Firebase Authentication** menggunakan metode Email & Password, dilengkapi halaman **SplashScreen** dan **Login**.

## Identitas & Pembagian Task
- **Fajar Islami** - Setup project Firebase, konfigurasi `firebase_options.dart`, integrasi `firebase_auth`, UI SplashScreen & Login.
- *(Tambahkan nama anggota tim lain di sini jika berkelompok)*

## Langkah Integrasi Firebase
1. Membuat project baru di **Firebase Console** (`myprojectfirebase-ca27e`).
2. Mengaktifkan metode autentikasi **Email/Password** pada menu **Build > Authentication > Sign-in method**.
3. Menambahkan akun pengguna uji coba pada tab **Users**.
4. Menjalankan `flutterfire configure` untuk menghubungkan aplikasi Flutter dengan Firebase dan menghasilkan file `lib/firebase_options.dart`.
5. Menambahkan package `firebase_core` dan `firebase_auth` pada `pubspec.yaml`.
6. Menginisialisasi Firebase di `lib/main.dart` sebelum menjalankan aplikasi melalui `Firebase.initializeApp`.
7. Membuat halaman `SplashScreen` (`lib/pages/splash_screen.dart`) dan `LoginPage` (`lib/pages/login_page.dart`) dengan `FirebaseAuth.instance.signInWithEmailAndPassword`.