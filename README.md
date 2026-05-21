# 💧 Water Bill (PDAM) Finance App - React Native

[![React Native](https://img.shields.io/badge/React_Native-0.81-61DAFB?logo=react&logoColor=black)](https://reactnative.dev/)
[![Expo](https://img.shields.io/badge/Expo-54-000000?logo=expo&logoColor=white)](https://expo.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.9-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![UKL Project](https://img.shields.io/badge/Project-UKL-blue)](#)

Aplikasi mobile **PDAM Finance & Billing** ini dirancang menggunakan **React Native** dan **Expo** sebagai proyek **Uji Kompetensi Keahlian (UKL)**. Aplikasi ini mempermudah pelanggan dalam memantau penggunaan air, melihat rincian tagihan bulanan secara real-time, melakukan simulasi pembayaran, serta melaporkan keluhan atau gangguan secara cepat dan efisien.

---

## 🌟 Fitur Utama

Aplikasi ini dilengkapi dengan berbagai fitur penting untuk manajemen keuangan dan layanan pelanggan PDAM:

1. **Dashboard & Monitoring Penggunaan**: 
   - Menampilkan ringkasan tagihan air aktif secara langsung di halaman utama.
   - Grafik atau visualisasi sederhana konsumsi air bulanan dalam satuan meter kubik ($m^3$).
2. **Detail & Riwayat Tagihan**:
   - Informasi lengkap mengenai stand meter awal, stand meter akhir, volume air yang digunakan, golongan tarif, dan biaya admin.
   - Riwayat pembayaran bulan-bulan sebelumnya yang memudahkan pencatatan keuangan rumah tangga.
3. **Simulasi Pembayaran (Payment Gateway Simulation)**:
   - Fitur pembayaran tagihan secara instan menggunakan metode simulasi e-wallet, transfer bank, atau gerai pembayaran.
   - Status tagihan otomatis berubah menjadi "Lunas" setelah simulasi pembayaran berhasil.
4. **Sistem Pengaduan Gangguan (Customer Service)**:
   - Pelanggan dapat membuat laporan jika terjadi kendala seperti pipa bocor, air keruh, atau gangguan aliran.
   - Dukungan unggah foto/lampiran untuk mempermudah identifikasi masalah oleh admin PDAM.
5. **Manajemen Profil & Akun**:
   - Informasi lengkap mengenai profil pelanggan, Nomor ID Pelanggan, alamat instalasi, dan golongan tarif sosial/rumah tangga.

---

## 🛠️ Tech Stack & Dependencies

Proyek ini dibangun menggunakan teknologi modern:

- **Framework**: [React Native](https://reactnative.dev/) dengan [Expo SDK 54](https://expo.dev/)
- **Bahasa Pemrograman**: [TypeScript](https://www.typescriptlang.org/)
- **Routing**: [Expo Router v6](https://docs.expo.dev/router/introduction/) (File-based Routing)
- **Animasi & Transisi**: [React Native Reanimated](https://reactnative.dev/docs/animations)
- **UI & Icons**: Expo Vector Icons (`@expo/vector-icons`) & Expo Symbols
- **Tampilan Gambar**: Expo Image untuk rendering gambar yang efisien dan cepat.

---

## 🚀 Cara Memulai (Panduan Instalasi)

Ikuti langkah-langkah di bawah ini untuk menjalankan proyek ini di perangkat lokal Anda:

### 1. Prasyarat (Prerequisites)
Pastikan Anda telah menginstal aplikasi pendukung berikut pada komputer Anda:
- **Node.js** (Versi LTS terbaru direkomendasikan)
- **Git** untuk kloning repositori
- **Expo Go** pada perangkat smartphone Anda (iOS/Android) atau emulator Android Studio / Xcode Simulator.

### 2. Kloning Repositori
Jalankan perintah berikut di terminal Anda untuk mengkloning proyek:
```bash
git clone https://github.com/NauvalFaiz/app-react-native-ukl.git
```

### 3. Masuk ke Direktori Proyek
```bash
cd app-react-native-ukl
```

### 4. Instalasi Dependensi
Instal seluruh library dan komponen yang dibutuhkan dengan perintah:
```bash
npm install
```

### 5. Jalankan Aplikasi
Jalankan server pengembangan Expo menggunakan perintah:
```bash
npx expo start
```

Setelah server berjalan, Anda dapat:
- **Android**: Tekan `a` untuk membuka di Android emulator.
- **iOS**: Tekan `i` untuk membuka di iOS simulator.
- **Scan QR Code**: Buka aplikasi **Expo Go** pada ponsel Anda dan pindai kode QR yang muncul di terminal untuk membukanya secara langsung di perangkat fisik.

---

## 📁 Struktur Folder Proyek

```text
app-react-native-ukl/
├── app/                  # File routing utama (Expo Router)
│   ├── (tabs)/           # Halaman dengan navigasi Tab bawah (Dashboard, Explore)
│   │   ├── _layout.tsx   # Konfigurasi layout tab bar bawah
│   │   ├── explore.tsx   # Halaman eksplorasi / transaksi
│   │   └── index.tsx     # Halaman Dashboard Utama (Home)
│   ├── _layout.tsx       # Root layout aplikasi
│   └── modal.tsx         # Modal screen untuk pop-up info
├── assets/               # Gambar, font, dan aset statis aplikasi
├── components/           # Komponen UI reusable (Button, Input, Cards)
│   └── ui/               # Komponen UI khusus (Icon, Collapsible, dll)
├── constants/            # Variabel konstan (Warna, Konfigurasi, Tema)
├── hooks/                # Custom React hooks
├── scripts/              # Helper scripts
├── package.json          # Konfigurasi dependensi npm
└── tsconfig.json         # Konfigurasi compiler TypeScript
```

---

## 🔄 Alur Jalannya Aplikasi (Workflow)

Berikut adalah alur penggunaan aplikasi PDAM Finance:
1. **Autentikasi**: Pengguna masuk menggunakan akun pelanggan yang telah terdaftar.
2. **Dashboard**: Pengguna dapat melihat total tagihan bulan berjalan dan total pemakaian air ($m^3$).
3. **Simulasi Transaksi**: Pengguna memilih tagihan aktif, memilih metode pembayaran simulasi, dan menyelesaikan pembayaran.
4. **Riwayat**: Setelah pembayaran sukses, status tagihan diperbarui dan tercatat pada riwayat pembayaran.
5. **Pengaduan**: Jika ada kendala, pengguna dapat mengirimkan laporan pengaduan langsung dari aplikasi.

---

## 💻 Kontributor & Pengembang

Proyek ini dibuat dan dikembangkan oleh:

- **Nama**: Nauval Faiz Luthf Hisyam
- **Peran**: Full Stack Mobile Developer / UI Designer
- **Instansi**: Uji Kompetensi Keahlian (UKL) React Native App

Jika Anda memiliki pertanyaan atau masukan mengenai proyek ini, silakan hubungi pengembang melalui repositori GitHub resmi ini.

---
⭐ *Jangan ragu untuk memberikan star jika proyek ini bermanfaat bagi Anda!*
