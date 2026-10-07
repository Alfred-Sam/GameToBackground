# 🎮 Game To Background

> Mengubah game, video, atau aplikasi yang sedang aktif menjadi latar belakang desktop Windows secara otomatis ketika komputer tidak digunakan — dan mengembalikannya hanya dengan satu klik!
>
> **Dibuat oleh Zlac — We Love Gembull**

---

## 📖 Gambaran Umum

**Game To Background** adalah utilitas Windows ringan yang memantau waktu ketika komputer tidak digunakan. Ketika pengguna tidak melakukan aktivitas selama waktu yang telah ditentukan, aplikasi yang sedang berada di depan, seperti Google Chrome, video YouTube, Twitch, game singleplayer/idle, atau pemutar media, akan dipindahkan ke belakang ikon desktop sebagai latar belakang Windows.

Aplikasi memanfaatkan lapisan wallpaper **`WorkerW`** pada Windows sehingga aplikasi yang sedang berjalan dapat tetap aktif di latar belakang desktop.

---

## ⚙️ Cara Kerja

### 1. ⏱️ Deteksi Tidak Aktif Otomatis

- Atur batas waktu tidak aktif sesuai kebutuhan (default: **30 detik**).
- Jika tidak ada aktivitas keyboard atau mouse selama waktu tersebut, jendela aplikasi yang sedang aktif akan secara otomatis diubah ukurannya dan dipindahkan ke latar belakang desktop.

### 2. 🖥️ Tetap Bisa Melakukan Aktivitas Lain

Ketika game atau video sedang berjalan sebagai latar belakang desktop, Anda tetap dapat menggunakan komputer seperti biasa.

Anda dapat menekan **`Windows Key`**, mencari dan membuka **Microsoft Word**, **Steam**, **Calculator**, **Discord**, atau aplikasi lainnya.

Aplikasi yang berada di latar belakang akan tetap berjalan tanpa mengganggu pekerjaan atau aktivitas Anda pada aplikasi lain.

### 3. 🖱️ Mengembalikan dengan Satu Klik

Ketika ingin kembali menggunakan aplikasi yang sebelumnya dijadikan latar belakang:

- Cukup **klik kiri pada area kosong desktop**.
- Aplikasi akan segera dikembalikan ke ukuran jendela sebelumnya.
- Jendela aplikasi akan kembali berada di depan.
- Latar belakang desktop akan diperbarui secara otomatis.

### 4. 🛡️ Mode Perlindungan Anti-Cheat

**Game To Background** menyediakan perlindungan untuk game yang menggunakan sistem anti-cheat ketat.

Game kompetitif seperti:

- **Counter-Strike 2 / CS:GO**
- **VALORANT / Riot Vanguard**
- **Apex Legends**
- **Fortnite**
- **Rainbow Six Siege**
- **Overwatch**
- **League of Legends**
- dan game kompetitif lainnya

dapat secara otomatis dikecualikan dari proses pemindahan ke latar belakang.

Mode ini bertujuan untuk mengurangi risiko masalah kompatibilitas dengan sistem anti-cheat, termasuk potensi crash atau perilaku yang tidak diinginkan pada game.

> **Catatan:** Perlindungan anti-cheat bukan jaminan resmi bahwa game tertentu tidak akan mendeteksi atau memblokir aplikasi pihak ketiga. Tetap gunakan dengan risiko Anda sendiri dan periksa kebijakan anti-cheat dari game yang digunakan.

---

## 🚀 Cara Menggunakan

1. Jalankan **`GameToBackgroundGUI.exe`**.
2. Atur **Idle Threshold** dalam satuan detik.
3. Pastikan **Anti-Cheat Protection** tetap dicentang (disarankan).
4. Klik **Start Service**.
5. Biarkan game, video, atau browser yang ingin digunakan tetap terbuka.
6. Setelah komputer tidak digunakan selama waktu yang ditentukan, aplikasi tersebut akan otomatis dipindahkan menjadi latar belakang desktop.

---

## 🔨 Build & Publish Executable Standalone

Untuk membuat file **`.exe` standalone** yang dapat dijalankan pada Windows 10/11 64-bit tanpa perlu menginstal .NET terlebih dahulu, jalankan perintah berikut melalui PowerShell:

```powershell
dotnet publish GameToBackgroundGUI\GameToBackgroundGUI.csproj -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true -p:EnableCompressionInSingleFile=true
```

File executable yang telah dikompilasi akan berada di:

```text
GameToBackgroundGUI\bin\Release\net8.0-windows\win-x64\publish\GameToBackgroundGUI.exe
```

---

## 💻 Persyaratan Sistem

- **Sistem Operasi:** Windows 10 / Windows 11
- **Arsitektur:** 64-bit (x64)
- **.NET:** Tidak diperlukan pada komputer pengguna jika menggunakan versi standalone hasil publish.

---

## 👨‍💻 Kredit & Lisensi

- **Developer:** Zlac
- **Special Note:** *We Love Gembull* ❤️
- Didistribusikan di bawah **MIT License**.

Lihat file [`LICENSE`](LICENSE) untuk informasi lengkap mengenai lisensi.
