# Silang Waktu

**TTS Sejarah, berebut pakai bottle flip.**

Silang Waktu adalah permainan teka-teki silang (TTS) untuk pembelajaran Sejarah di kelas. Dua tim bersaing menjawab soal, dan **bottle flip dipakai sebagai "bel"**: tim yang botolnya berdiri lebih dulu berhak menjawab. Semuanya berjalan di satu halaman web yang ditampilkan lewat proyektor, lengkap dengan papan skor dan panel kontrol untuk guru.

Proyek ini dibuat sebagai tindakan pada Penelitian Tindakan Kelas (PTK) untuk meningkatkan **motivasi dan keaktifan belajar murid** dengan model *Team Games Tournament* (TGT).

## Demo

https://togetumis.github.io/SilangWaktu/

## Fitur

- **Papan TTS besar** untuk proyektor, dengan 20 soal dan grid 13 x 22 yang kata-katanya saling berpotongan.
- **Dua tim** dengan papan skor terpisah dan warna berbeda.
- **Alur permainan buzzer:** guru membacakan soal, wakil kedua tim bottle flip, tim yang berhasil lebih dulu menjawab.
- **Sistem skor:** jawaban benar +10, merebut jawaban dari tim lawan +5, jawaban dibuka tanpa poin jika tidak ada yang berhasil.
- **Kunci jawaban untuk guru** yang tersembunyi dan hanya tampil bila diaktifkan.
- **Lembar observasi keaktifan dan motivasi** yang bisa diisi di layar dan dicetak, lengkap dengan rekap skor dua pengamat.
- Satu file, tanpa internet dan tanpa instalasi.

## Cara bermain

1. Bagi kelas menjadi dua tim (Tim A dan Tim B).
2. Guru memilih nomor soal, lalu membacakan soalnya.
3. Wakil dari tiap tim melakukan bottle flip bersamaan. Tim yang botolnya berdiri lebih dulu berhak menjawab.
4. Jika jawaban benar, tim mendapat **+10** dan jawabannya muncul di grid dengan warna tim.
5. Jika salah, tim lawan boleh merebut dan mendapat **+5** bila benar.
6. Jika keduanya salah atau tidak ada yang berhasil flip, jawaban dibuka tanpa poin.
7. Setelah semua soal selesai, tim dengan skor tertinggi menang.

Disarankan agar wakil tim bergiliran sehingga setiap murid mendapat kesempatan maju, dan guru memberi satu pertanyaan pemantik setelah tiap jawaban benar.

## Cara menjalankan

- **Lewat web:** buka link demo di atas.
- **Tanpa internet:** unduh `index.html`, lalu klik dua kali sampai terbuka di browser. Sambungkan laptop ke proyektor.

## Cara mengganti soal

Semua soal berada di dalam `index.html`, pada daftar `D` di bagian skrip. Satu soal ditulis dengan format:

```
["JAWABAN", baris, kolom, "H" atau "V", "Teks soal"]
```

`H` berarti mendatar dan `V` berarti menurun. Ukuran grid diatur oleh `R` (jumlah baris) dan `C` (jumlah kolom). Kata-kata harus saling berpotongan dan tidak boleh berdempetan sejajar, jadi mengganti seluruh soal sebaiknya disertai pengecekan ulang posisi kata.

## Lembar observasi

Halaman **Lembar Observasi** berisi:

- **A.** Catatan keaktifan tiap murid (maju bottle flip, menjawab soal, berdiskusi dalam tim, bertanya atau menanggapi, memperhatikan penjelasan).
- **B.** Penilaian keaktifan dan motivasi klasikal dengan 8 indikator dan skala 1 sampai 4.
- **C.** Rekap skor dua pengamat beserta rata-rata dan kategori.
- **D.** Catatan lapangan.

Isian **tidak tersimpan** setelah halaman ditutup. Gunakan tombol **Cetak / Simpan PDF** setelah selesai mengisi. Jangan mengunggah lembar yang sudah berisi nama murid ke repositori publik.

## Struktur berkas

```
SilangWaktu/
  index.html   # permainan dan lembar observasi (semua dalam satu berkas)
  README.md
```

## Kredit

- Materi soal: asal-usul nenek moyang bangsa Indonesia (kelas X), disusun dari bahan ajar yang dipakai guru kelas.
- Dikembangkan oleh Muhammad Ihsan, mahasiswa Pendidikan Sejarah, Universitas Negeri Padang, dalam kegiatan PLK di SMA PGRI 4 Padang.
