# RZ Launcher reconstruction starter

## Tujuan tahap ini
Workflow ini menyiapkan tahap pertama: memeriksa APK, mendekompilasi resource/manifest,
dan mencoba rebuild baseline tanpa perubahan. Ini **belum menambahkan widget**.

## Cara pakai dari HP Android
1. Buat repository GitHub baru, misalnya `rzlauncher-widget-mod`.
2. Upload APK yang kamu kirim ke folder `input/` dengan nama persis `rzlauncher.apk`.
3. Upload folder `.github/workflows/` beserta file workflow di dalamnya.
4. Buka tab **Actions** → **RZ Launcher - Decode and Baseline Build** → **Run workflow**.
5. Setelah selesai, buka hasil run dan unduh artifact **RZ-Launcher-Decode-Analysis**.
6. Kirim kembali artifact ZIP hasilnya ke chat ini untuk pemeriksaan struktur aplikasi.

## Catatan penting
- APK hasil baseline memakai kunci uji baru. Karena tanda tangannya berbeda dari APK asli,
  APK itu tidak bisa dipasang sebagai pembaruan langsung di atas aplikasi asli.
- Jangan uninstall aplikasi asli atau memasang APK uji sebelum kita memastikan package ID,
  kompatibilitas, dan hasil pengujian.
- Workflow hanya membuktikan apakah APK dapat didekode dan dibangun ulang. Penambahan widget
  memerlukan analisis kode hasil dekompilasi dan implementasi terpisah.
- Jangan mengunggah ke repository publik jika kamu tidak ingin APK dapat diakses publik.
