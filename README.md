# Laura-Personal Assistance: paket PWA dan APK (versi 1.1)

## Memperbarui dari versi sebelumnya
1. Di repositori GitHub Anda, unggah ulang seluruh isi folder ini dan **timpa** file lama (folder `docs`, `resources`, `.github`, `package.json`, `capacitor.config.json`).
2. Tab Actions, **Build Laura APK**, Run workflow. Tunggu centang hijau, lalu unduh **Laura-APK**.
3. **Copot dulu aplikasi Laura lama** di HP (tanda tangan APK berbeda tiap build, jadi tidak bisa menimpa). Data lokal di aplikasi lama ikut terhapus. Setelah itu pasang APK baru.
4. PWA: otomatis ikut terbarui setelah GitHub Pages selesai deploy. Jika tampilan lama masih muncul, tutup aplikasi lalu buka lagi.

## Mengaktifkan chat AI Laura (gratis)
1. Buka https://aistudio.google.com/apikey, masuk dengan akun Google, lalu **Create API key**.
2. Di Laura, buka panel Laura, **Pengaturan suara**, lalu tempel di kolom **API key Gemini**.
3. Jika Google meminta pengaktifan billing atau paket prabayar untuk akun baru, itu ketentuan Google. Tanpa itu pun jadwal, pengingat, dan salat tetap berfungsi.
4. Paket gratis Google memiliki batas permintaan per menit dan per hari. Pada paket gratis, isi percakapan dapat dipakai Google untuk memperbaiki produknya, jadi jangan mengirim data sensitif.
5. Alternatif: **API key Anthropic** (berbayar per pemakaian).

## Mikrofon dan suara
- **APK:** Laura memakai layanan suara Android (jendela Google "Silakan bicara"). Izinkan **Mikrofon** saat diminta. Perlu aplikasi Google dan internet aktif.
- **PWA di Chrome:** izinkan mikrofon untuk situs (ikon gembok, Izin). Jika muncul pesan galat, pesannya menyebut penyebabnya.
- Tombol **Mic: ID/EN** mengganti bahasa yang dikenali.
- Suara Laura memakai suara teks-ke-ucapan HP. Jika tidak ada suara Indonesia atau Inggris (UK), pasang lewat Pengaturan HP, Bahasa, Output teks-ke-ucapan, Layanan suara Google, lalu unduh data suaranya. Pilihan suara ada di Pengaturan suara.

## Nama dan ikon
- Nama aplikasi: **Laura-Personal Assistance**. Ikon launcher dan ikon PWA memakai avatar Laura. Nama di layar utama mungkin dipotong oleh Android.

## Jalur A: PWA (Android dan Windows)
Repositori **Public**, lalu Settings, Pages, Source: Deploy from a branch, Branch `main`, folder `/docs`. Alamatnya `https://NAMA-GITHUB-ANDA.github.io/NAMA-REPO/`. Pasang: Chrome Android (menu, Instal aplikasi) atau Edge Windows (menu, Apps, Install this site as an app).

## Jalur B: APK Android (pengingat jalan saat aplikasi tertutup)
Actions, Build Laura APK, Run workflow, unduh **Laura-APK**, ekstrak, pasang `app-debug.apk`. Izinkan Notifikasi dan Alarm dan pengingat, lalu atur baterai ke **Tanpa pembatasan**.

## Pengingat
- APK: dijadwalkan ke sistem Android untuk 7 hari ke depan dan diperbarui tiap Laura dibuka. Saat tertutup muncul notifikasi bersuara. Suara Laura hanya terdengar saat aplikasi terbuka.
- PWA: hanya saat aplikasi terbuka.
- Waktu salat adalah perkiraan untuk Jakarta. Cocokkan dengan jadwal resmi.

## Keamanan
Jangan menaruh API key atau link D-ID di file repositori public. Isi hanya lewat Pengaturan di perangkat.
