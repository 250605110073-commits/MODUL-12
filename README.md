# MODUL 12 – GPS LOCATION

## Deskripsi
Project ini merupakan aplikasi Flutter untuk praktikum Modul 12 yang membahas penggunaan GPS atau layanan lokasi pada perangkat Android.

Aplikasi menggunakan package:
- `geolocator` untuk mengakses layanan lokasi perangkat.
- `geocoding` untuk mengolah koordinat menjadi informasi alamat lokasi.

## Teknologi yang Digunakan
- Flutter
- Dart
- Android Emulator / Perangkat Android
- Geolocator
- Geocoding

## Persiapan Sebelum Menjalankan Aplikasi

Pastikan perangkat sudah memiliki:
1. Flutter SDK dan Dart SDK.
2. Android Studio atau Android SDK.
3. Android Emulator atau perangkat Android.
4. Visual Studio Code.
5. Git (opsional, untuk pengelolaan repository).

Periksa instalasi Flutter dengan perintah:

```powershell
flutter doctor
```

## Instalasi dan Konfigurasi

### 1. Clone Repository

```powershell
git clone https://github.com/250605110073-commits/MODUL-12.git
```

Masuk ke folder project:

```powershell
cd MODUL-12
```

### 2. Instalasi Dependency

Jalankan perintah:

```powershell
flutter pub get
```

Package yang digunakan dalam project ini:
- `geolocator`
- `geocoding`

### 3. Konfigurasi Izin Lokasi Android

Sebelum aplikasi dijalankan, buka file:

`android/app/src/main/AndroidManifest.xml`

Pastikan terdapat izin berikut di dalam tag `<manifest>` dan di luar tag `<application>`:

```xml
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"/>
```

Izin tersebut diperlukan agar aplikasi dapat meminta akses lokasi perangkat.

### 4. Mengaktifkan Lokasi Perangkat

Sebelum mencoba fitur GPS:
1. Jalankan Android Emulator atau hubungkan perangkat Android.
2. Aktifkan layanan lokasi (Location/GPS) pada perangkat.
3. Izinkan akses lokasi ketika aplikasi meminta permission.

## Menjalankan Aplikasi

Karena file utama aplikasi menggunakan `main_modul12.dart`, jalankan dengan perintah:

```powershell
flutter run -t lib/main_modul12.dart
```

## Pengujian

Untuk menjalankan pengujian project:

```powershell
flutter test
```

## Struktur File Utama

```text
MODUL-12/
├── android/
│   └── app/
│       └── src/
│           └── main/
│               └── AndroidManifest.xml
├── lib/
│   └── main_modul12.dart
├── test/
│   └── widget_test.dart
├── pubspec.yaml
├── pubspec.lock
└── README.md
```

## Repository

GitHub: https://github.com/250605110073-commits/MODUL-12

---

**Praktikum Pemrograman Mobile – Modul 12**