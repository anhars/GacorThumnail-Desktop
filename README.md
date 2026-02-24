# GacorThumnail Desktop (Native App)

Ini versi **desktop native** (Electron) — tidak perlu Python, tidak perlu localhost, tidak perlu browser.
User tinggal install EXE, lalu aplikasi terbuka seperti app biasa.

## Fitur
- Canvas editor 16:9 (preview 960x540)
- Export output 1280x720 (16:9) PNG
- Drag & drop teks langsung di canvas
- Multi text layer (add/remove, enable/disable)
- Resize teks via transform handle
- Glow + outline per layer
- Save file pakai dialog Windows (native)

## Cara build paling gampang (tanpa install apa-apa di PC kamu)
Pakai GitHub Actions:
1) Buat repo GitHub baru, upload semua file project ini.
2) Tab Actions → jalankan workflow **Build Desktop Windows Installer**
3) Download artifact: `GacorThumnail_Desktop_Windows`
4) Di dalamnya ada installer `.exe` (NSIS)

## Build lokal (butuh Node.js)
1) Install Node.js 20
2) Jalankan:
   npm install
   npm run dev     (untuk test)
   npm run dist    (buat installer)

Output installer ada di folder `release/`.

## Catatan
- Default font: Impact. (Windows biasanya punya)
- Nanti bisa kita tambah: JPEG export + auto <2MB + batch export.
