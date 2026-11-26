# Prediksi SAS Ganjil Matematika Kelas VI SD/MI

**Pendamping Akademik · Paket statis GitHub Pages + satu halaman Blogger**  
Versi 1.0.0 · 26 November 2026

## Isi paket

- `index.html` — aplikasi tes mandiri, penilaian otomatis, timer, navigasi, hasil, pembahasan.
- `data/bank-soal.json` — tepat **800 soal pilihan ganda + 200 soal isian**, kunci dan penjelasan tiap soal.
- `data/bank-soal.csv` — data yang sama untuk pemeriksaan dan pengeditan manual.
- `assets/gambar-001.jpg` s.d. `assets/gambar-200.jpg` — **200 gambar soal** berformat JPG: 160 PG dan 40 isian.
- `assets/foto-1.jpg` s.d. `foto-4.jpg` — empat foto ilustrasi realistis hasil generasi AI, untuk tampilan antarmuka.
- `blogger-embed.html` — kode satu halaman Blogger.
- `AUDIT.txt` — audit jumlah item dan validasi data.

**Tidak menggunakan file SVG, emoji, ataupun ikon.** Ilustrasi matematika JPG digambar secara digital dengan objek dua dimensi dan efek bayangan; bukan foto dokumentasi.

## Cakupan & sifat soal

- Kurikulum Merdeka, Matematika Kelas VI, fokus **semester ganjil**: Bab 1 Pecahan dan Desimal; Bab 2 Rasio.
- Tahun contoh SAS yang ditinjau: 2023/2024, 2024/2025, 2025/2026. Soal di paket **orisinal yang dihasilkan lewat rancangan parametrik**, bukan salinan dari naskah sekolah, bukan bocoran soal resmi, dan belum divalidasi melalui uji empiris pada siswa.
- Komposisi per sesi: 32 PG + 8 isian = 40 soal, 90 menit; tingkat mudah 30%, sedang 50%, sulit 20%. Konfigurasi internal, **bukan peraturan wajib pemerintah**.
- Soal dipilih secara acak tanpa pengulangan per sesi, berimbang Bab 1 dan 2 jika memilih 'gabungan'. Setiap paket menggunakan soal bergambar minimal 6 PG + 2 isian selama ketersediaan pada subkelompok terpilih.
- Penilaian: nilai = jumlah benar / 40 × 100. Semua soal berbobot sama. Isian menerima pecahan senilai, tanda koma/titik desimal, dan rasio senilai sesuai format jawabannya.
- Jawaban disimpan di `localStorage` perangkat setempat; **tidak** disimpan ke server atau Supabase. Jangan gunakan hasil ini sebagai penilaian sekolah tanpa validasi dan pengawasan guru.
- Mengulang soal antar **sesi berbeda** tetap mungkin dan wajar karena semua sesi mengambil dari bank yang sama.

## Langkah 1: Unggah ke GitHub Pages

1. Masuk GitHub menggunakan akun yang Anda gunakan untuk Pendamping Akademik.
2. Buat repository publik bernama **`sas-ganjil-matematika-vi`**.
3. Unggah **semua isi folder ini ke root** repository (termasuk folder `data` dan `assets`). Jangan hanya mengunggah ZIP mentah.
4. Buka **Settings → Pages → Build and deployment → Deploy from a branch → main / (root)**, kemudian simpan.
5. Jika nama pengguna Anda `asyiknyabelajar`, alamat yang diharapkan adalah:  
   `https://asyiknyabelajar.github.io/sas-ganjil-matematika-vi/`
6. Tunggu hingga GitHub Pages menampilkan alamat yang benar, lalu buka dan uji 40 soal. **Alamat di atas belum otomatis terbit karena paket ini dibuat secara lokal.**

GitHub Pages: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## Langkah 2: Pasang satu halaman Blogger

1. Blogger → **Halaman → Halaman baru**.
2. Judul halaman: **Prediksi SAS Ganjil Matematika Kelas 6 SD/MI | Pendamping Akademik**.
3. Pindah editor ke **Tampilan HTML**, kemudian salin seluruh isi `blogger-embed.html`.
4. Bila username/repository berbeda, ganti seluruh URL `https://asyiknyabelajar.github.io/sas-ganjil-matematika-vi/` di iframe dan tautan layar penuh, serta nilai `appUrl` dalam script.
5. Tambahkan deskripsi penelusuran:  
   **Prediksi SAS Ganjil Matematika Kelas 6 SD/MI: 1.000 soal, 40 soal acak, 90 menit, soal bergambar, nilai otomatis dan pembahasan Kurikulum Merdeka.**
6. Publikasikan. Periksa tampilan desktop dan ponsel. Navigasi kembali sudah disiapkan ke:  
   https://pendampingakademik.blogspot.com/p/kelas-6-sdmi.html

Catatan: beberapa tema atau editor Blogger dapat memproses `<script>` secara berbeda. Bila tinggi iframe tidak menyesuaikan, nilai tinggi tetap 1.250px pada iframe masih dapat dipakai, atau ubah CSS ketinggiannya secara manual.

## Pengujian yang dianjurkan

- Pilih Gabungan Bab 1–2 → mulai → pastikan muncul 40 soal: 32 pilihan ganda dan 8 isian.
- Lompat nomor, jawab, tutup dan buka ulang pada perangkat sama → lanjutkan sesi.
- Jawab pecahan dengan bentuk senilai, misalnya `1/2` dan `2/4`; desimal `0,5` dan `0.5`.
- Kumpulkan → lihat nilai dan pembahasan → unduh TXT hasil.
- Verifikasi gambar JPG tampil, dan timer otomatis mengumpulkan setelah 90 menit.
- Buka di Blogger dan layar penuh, termasuk tampilan ponsel.

## Referensi pemetaan (tidak disalin verbatim)

1. Kemdikbudristek (2022), *Matematika untuk SD/MI Kelas VI* — https://static-sc.cloudapp.web.id/content/pdf/bukuteks/kurikulum21/Matematika_BS_KLS_VI.pdf
2. Kemendikdasmen (2025), *Panduan Pembelajaran dan Asesmen*, edisi revisi — https://kurikulum.kemendikdasmen.go.id/file/1755668120_manage_file.pdf
3. Sinau-Thewe (2023), contoh soal SAS Matematika VI 2023/2024 — https://www.sinau-thewe.com/2023/11/soal-kunci-saspas-semester-1-matematika.html
4. SD Inpres Appdt Batui (2024), contoh SAS Matematika VI 2024/2025 (salinan dokumen): https://id.scribd.com/document/797824245/SAS-1-Kelas-VI-MTK
5. Contoh SAS Matematika VI 2025/2026, soal perkalian, pembagian, rasio, desimal: https://id.scribd.com/document/951732726/SAS-KELAS-6-2025-MM-1
6. Contoh SAS Matematika VI 2025/2026, rasio dan penguatan hitung: https://id.scribd.com/document/967093896/SAS-MATEMATIKA

Penting: keragaman cakupan ujian sekolah dapat berbeda dari alur semester contoh. Sesuaikan pada ATP dan kalender pendidikan sekolah masing-masing.
