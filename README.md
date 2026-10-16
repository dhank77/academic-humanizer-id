# Academic Humanizer — Versi Bahasa Indonesia

Menghapus ciri tulisan AI dari makalah, skripsi, tesis, disertasi, dan proposal hibah berbahasa Indonesia — tanpa meratakan presisi ilmiah. Menjaga gaya penulis dan mengaitkan setiap klaim dengan bukti.

Adaptasi Bahasa Indonesia dari [AIScientists-Dev/academic-humanizer](https://github.com/AIScientists-Dev/academic-humanizer) (MIT).

## Untuk apa

- **Menajamkan kejelasan dan gaya:** memangkas frasa generik AI ("Dalam beberapa tahun terakhir...", "membuka jalan bagi", "eksperimen ekstensif", "sepengetahuan kami", kalimat >30 kata, em-dash) dan mendekatkan draf ke gaya penulis.
- **Menjaga klaim terikat bukti:** tidak ada kata kerja yang lebih kuat dari data (`membuktikan` → `menunjukkan secara empiris`), besaran samar menjadi rentang dengan atribusi.
- **Membiarkan kaidah ilmiah:** hedging berbasis bukti, kalimat pasif yang tepat, `kami`, definisi, simbol, dan setiap sitasi. Tidak mengubah angka atau referensi.
- **Mode khusus proposal hibah (DRTPM/Kemdiktisaintek, LPDP, BRIN, NSF, NIH):** menjaga visi yang akan dipangkas di makalah, dan mencurahkan upaya pada halaman pertama, karena di situlah reviewer memberi skor.

## Install

```bash
git clone https://github.com/dhank77/academic-humanizer-id ~/.claude/skills/academic-humanizer-id
```

Ini `SKILL.md` biasa plus contoh, jadi juga jalan sebagai skill/system prompt untuk **Codex** dan **MorphMind**. Arahkan agen ke `SKILL.md`.

## Pakai

```
/academic-humanizer-id
[tempel satu bagian, atau arahkan ke main.tex]
# opsional: "samakan dengan gaya saya dari paper_lalu.pdf; target: jurnal Sinta 2"
```

## Contoh

Lihat [`examples/before-after.md`](examples/before-after.md): contoh umum, pembuka halaman Tujuan proposal, dan Ringkasan hibah.

## Cara kerja

Enam lapis: katalog umum ciri AI → ciri AI akademik → menjaga konvensi ilmiah → pencocokan klaim↔bukti → kalibrasi suara/venue → mode proposal pendanaan (struktur hibah Indonesia + NSF/NIH, primasi halaman pertama, klaim↔kelayakan). Loop audit→tulis ulang didefinisikan di [`SKILL.md`](SKILL.md).

## Etika dan disclosure

Ini alat bantu penyuntingan untuk kejelasan dan gaya, dikalibrasi ke karya penulis sebelumnya yang sudah diterima. Tidak membuat temuan, mengarang data, atau mengubah sitasi, dan bukan untuk menghindari deteksi penggunaan AI. Penggunaannya tidak menghapus kewajiban deklarasi bantuan AI: selalu ikuti kebijakan disclosure venue yang dituju.

## Acknowledgments

- **[AIScientists-Dev/academic-humanizer](https://github.com/AIScientists-Dev/academic-humanizer)** (MIT). Karya asli berbahasa Inggris yang diadaptasi di sini.
- **[blader/humanizer](https://github.com/blader/humanizer)** (MIT). Katalog umum ciri AI untuk blog/teks kasual. Skill ini memakai ulang katalognya (Lapisan 1) dan memperluas untuk prosa akademik.
- **[koaeraser/ARMS](https://github.com/koaeraser/ARMS)**. Pipeline otonom untuk makalah riset statistik/metodologi. Menginformasikan penekanan klaim-bukti dan presisi numerik.

## Lisensi

MIT.
