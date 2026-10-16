---
name: academic-humanizer-id
version: 0.3.3-id
description: |
  Perbaiki kejelasan dan gaya naskah akademik berbahasa Indonesia yang dibantu AI
  (makalah, skripsi, tesis, disertasi, sanggahan reviewer) dan proposal pendanaan
  (hibah Kemdiktisaintek/DRTPM, LPDP, BRIN, serta NSF/NIH): menjaga kaidah ilmiah,
  mengaitkan setiap klaim dengan bukti (dan, untuk proposal, klaim dengan kelayakan),
  serta menyesuaikan dengan gaya penulis. Tidak pernah mengubah angka, hasil, atau
  sitasi, dan bukan untuk menghindari deklarasi penggunaan AI. Gunakan saat menyunting
  prosa akademik berbahasa Indonesia yang dibantu AI atau proposal hibah.
license: MIT
compatibility: claude-code codex morphmind opencode
allowed-tools: [Read, Write, Edit, Grep, Glob, AskUserQuestion]
---

# Academic Humanizer — Versi Bahasa Indonesia

Perbaiki kejelasan dan gaya naskah akademik berbahasa Indonesia yang dibantu AI, dengan tetap menjaga presisi dan gaya berbasis bukti yang dituntut karya ilmiah, serta menyesuaikan dengan gaya penulis. Pertahankan setiap angka, hasil, dan sitasi apa adanya, dan bukan sebagai alat untuk menghindari deklarasi penggunaan AI.

## Kapan digunakan
Menyunting atau menelaah prosa akademik: bagian makalah, abstrak, sanggahan reviewer, tinjauan pustaka, skripsi/tesis/disertasi, dan **proposal pendanaan** (hibah Kemdiktisaintek/DRTPM, LPDP, BRIN, NSF Project Summary/Description, NIH Specific Aims, hibah yayasan/fellowship; lihat Lapisan 6). **Bukan** untuk blog, marketing, atau esai pribadi, dan **jangan pernah** menyuntikkan opini, humor, atau kepribadian orang-pertama yang kasual ke dalam naskah. Untuk tulisan teknis, netral dan presisi *adalah* suara manusiawi. Satu catatan untuk proposal: registernya berbeda dari makalah, karena proposal dinilai dari visi dan kelayakan, sehingga bahasa ambisi yang akan dipangkas di makalah justru tepat di sana; terapkan Lapisan 6, bukan pemangkasan ketat lapisan makalah, untuk pernyataan visi.

## Prinsip inti
Tulisan akademik sudah memiliki suara manusiawi yang benar: netral, presisi, orang-pertama jamak ("kami"), setiap klaim terikat pada buktinya. Tugasnya adalah (1) menghapus *ciri khas AI* tanpa menjadikannya kasual, dan (2) menegakkan disiplin yang dilewatkan humanizer umum: **setiap klaim harus memiliki angka, gambar, tabel, atau sitasinya, dan tidak ada kata kerja yang lebih kuat dari buktinya.**

## Proses
1. **Baca** naskah dan contoh tulisan penulis; catat jenis dokumen (makalah vs. proposal pendanaan) dan target venue atau lembaga pendana. Untuk proposal, terapkan juga Lapisan 6 dan jaga visi yang semestinya.
2. **Audit** (jangan sunting dulu): daftarkan setiap pola yang terdeteksi beserta lokasi dan usulan perbaikan, serta status bukti setiap klaim empiris.
3. **Tulis ulang**: struktur dan isi sama, semua klaim dan sitasi dipertahankan, ciri AI dihapus, klaim berlebihan disesuaikan dengan bukti, hedging yang sah dipertahankan.
4. **Laporkan**: teks bersih plus log perubahan singkat (pola yang dihapus, klaim yang dilunakkan atau diberi penunjuk bukti, catatan gaya). Cakup semua yang dicakup naskah asli: jika aslinya lima paragraf, hasil suntingan pun lima paragraf.

---

## Lapisan 1: Katalog umum ciri tulisan AI
Pindai dan perbaiki pola umum berikut, dengan memperhatikan pengecualian akademik di Lapisan 3:

- klaim penting yang digelembungkan ("menandai momen penting", "tonggak penting");
- ekor "-ing" / anak kalimat dangkal yang memalsukan kedalaman ("..., sehingga menyoroti...", "..., yang menggarisbawahi...");
- bahasa promosi/figuratif ("kaya", "vibrant", "inovatif", "terobosan", "mutakhir");
- atribusi samar ("para ahli berpendapat" tanpa sitasi);
- kosakata khas AI bahasa Inggris: *delve, underscore, intricate, tapestry, testament, landscape (abstrak), pivotal, showcase, foster, leverage (pengisi), realm, seamless*;
- padanan Indonesia-nya: *menggali lebih dalam, menggarisbawahi, lanskap, ranah, memamerkan, memfasilitasi, memanfaatkan (sebagai pengisi), mulus, rumit, permadani, bukti (testament)*;
- penghindaran kopula ("berfungsi sebagai" -> "adalah");
- paralelisme negatif ("bukan hanya X, tetapi juga Y");
- padding aturan-tiga (tiga kata sifat/frasa berderet yang isinya sama);
- variasi elegan (memutar sinonim untuk satu rujukan yang sama);
- pengisi ("perlu dicatat bahwa", "perlu ditekankan bahwa", "dalam rangka untuk", "dapat dikatakan bahwa", "pada dasarnya");
- **kalimat terlalu panjang dan bertumpuk anak kalimat (pecah; lihat 2.11)**;
- **em-dash (hapus seluruhnya; ganti dengan koma, titik dua, tanda kurung, atau kalimat terpisah)**.

**Sebelum:** *Selain itu, bukti abadi atas nilai metode ini adalah kemampuannya menggali ketergantungan yang rumit, menampilkan integrasi mulus yang menggarisbawahi peran pentingnya.*
**Sesudah:** *Metode ini juga menangkap ketergantungan orde-tinggi yang tidak tertangkap baseline (Tabel 2).*

---

## Lapisan 2: Ciri khas AI akademik (hapus atau perbaiki)

### 2.1 Kata kerja klaim berlebihan
Karya empiris *menunjukkan* dan *memberikan bukti*; ia tidak *membuktikan* atau *menegaskan* kebenaran universal.
**Waspadai:** membuktikan, menunjukkan (sebagai kebenaran mutlak), menetapkan, menjamin, mengonfirmasi; "secara signifikan" tanpa uji/angka.
**Sebelum:** *Kami membuktikan bahwa metode kami secara signifikan mengungguli semua pendekatan sebelumnya.*
**Sesudah:** *Metode kami meningkatkan akurasi held-out sebesar 4–7 poin dibandingkan pendekatan sebelumnya yang terkuat (Tabel 3); peningkatan signifikan pada p < 0,01 dengan uji berpasangan.*

### 2.2 Hype signifikansi
**Waspadai:** membuka jalan bagi, langkah krusial/penting menuju, berpotensi merevolusi, membuka cakrawala baru, memberikan pencerahan tentang, sangat penting, menjembatani kesenjangan.
**Sebelum:** *Penelitian ini membuka jalan bagi paradigma baru dan memberi pencerahan atas masalah yang sangat penting.*
**Sesudah:** *Penelitian ini mengatasi satu modus kegagalan metode sebelumnya: akumulasi galat pada rollout horizon-panjang (Bagian 4).*

### 2.3 Penguat kosong
**Waspadai:** eksperimen ekstensif/komprehensif/mendalam, berbagai macam, beragam, sejumlah, banyak.
**Sebelum:** *Kami melakukan eksperimen ekstensif pada berbagai macam dataset.*
**Sesudah:** *Kami mengevaluasi pada tiga dataset (ImageNet, CIFAR-100, dan iNaturalist).*

### 2.4 Bantalan kebaruan
**Waspadai:** "novel/baru" dipakai lebih dari sekali per bagian; "sepengetahuan kami"; "untuk pertama kalinya".
**Sebelum:** *Kami mengusulkan kerangka baru dan, sepengetahuan kami, pertama kali mengkaji hal ini.*
**Sesudah:** *Kami mengkaji kalibrasi daring dengan label tertunda, yang tidak dibahas pada kajian kalibrasi sebelumnya (luring).*

### 2.5 Pembuka formulaik
**Waspadai:** "Dalam beberapa tahun terakhir, X telah menarik perhatian..."; "Dengan pesatnya perkembangan..."; "Terlepas dari kemajuan terkini,...".
**Sebelum:** *Dalam beberapa tahun terakhir, deep learning tabular telah menarik perhatian yang meningkat.*
**Sesudah:** *Deep learning tabular memiliki keterbatasan struktural: sebagian besar model membuang metadata tipe-fitur dan harus mempelajarinya ulang dari data.*

### 2.6 Penggunaan konjungsi berlebihan
Jangan mulai kalimat berurutan dengan Selain itu/Selanjutnya/Lebih lanjut/Khususnya; biarkan logika yang memikul.
**Sebelum:** *Selain itu, metode ini cepat. Selanjutnya, sederhana. Lebih lanjut, dapat diskalakan.*
**Sesudah:** *Metode ini cepat dan sederhana, serta dapat diskalakan hingga satu juta baris (Bagian 5).*

### 2.7 Klise daftar kontribusi
Setiap kontribusi menyebut *hasil spesifik*, bukan pengulangan abstrak.
**Sebelum:** *Kontribusi kami adalah: (1) metode baru; (2) eksperimen ekstensif; (3) hasil yang kuat.*
**Sesudah:** *Kami (1) memperkenalkan encoder sadar-metadata yang mencapai AUROC 0,91 berbanding 0,86 untuk baseline terkuat; (2) menunjukkan kinerjanya tetap dalam 2 poin pada 20% label-noise sementara baseline turun 9 poin; (3) merilis benchmark-nya.*

### 2.8 Penimbunan sitasi
Sitir satu atau dua karya yang relevan dan jelaskan alasannya, bukan daftar kurung.
**Sebelum:** *Terdapat banyak metode [3, 7, 9, 12, 15].*
**Sesudah:** *Metode sebelumnya yang paling dekat adalah TabNet [7], yang mengenkode semua fitur secara gabungan; kami sebaliknya mengondisikan pada metadata tipe-fitur.*

### 2.9 Hedging dengan kesamaran
**Waspadai:** agak, relatif, cukup, sampai batas tertentu. Kuantifikasi atau potong.
**Sebelum:** *Kinerja agak lebih baik dan relatif robust.*
**Sesudah:** *Akurasi 3 poin lebih tinggi dan bervariasi kurang dari 1 poin pada lima seed.*

### 2.10 Penekanan boilerplate
**Waspadai:** "Perlu dicatat bahwa", "Perlu ditekankan bahwa", "Terutama,", "Pentingnya,". Jika penting, kalimatnya sendiri yang menunjukkannya.
**Sebelum:** *Perlu dicatat bahwa, yang penting, peningkatan berlaku di semua skenario.*
**Sesudah:** *Peningkatan berlaku di ketiga skenario (Tabel 4).*

### 2.11 Kalimat terlalu panjang dan bertumpuk
AI menyukai kalimat panjang yang merangkai tiga atau empat klausa dengan koma dan "yang", "sementara", "dengan", "di mana". Pecah: satu ide per kalimat, dan potong anak kalimat yang tidak berbobot. **Waspadai:** kalimat lebih dari ~30 kata, atau dengan 3+ anak kalimat.
**Sebelum:** *Metode yang ada, meskipun menjanjikan, sebagian besar bersifat empiris, dengan prinsip yang tidak jelas mendasari perilakunya, sehingga membatasi keandalan dan kemajuan lebih lanjut.*
**Sesudah:** *Metode yang ada tetap bersifat empiris. Prinsipnya tidak jelas, sehingga membatasi keandalan dan kemajuan.*

---

## Lapisan 3: Pertahankan ini (jangan koreksi berlebihan)
Humanizer umum meratakan konstruksi ilmiah yang sah. Pertahankan:

- **Hedging berbasis bukti adalah benar dan wajib.** Pertahankan "menunjukkan", "konsisten dengan", "kami menduga bahwa", "dapat mengindikasikan", "tampaknya" ketika klaim memang belum pasti.
  *Perbaikan salah:* mengubah *"hasil menunjukkan X"* menjadi *"hasil membuktikan X"*: ini memproduksi klaim berlebihan. Pertahankan kata kerja yang terkalibrasi.
- **Kalimat pasif** boleh ketika pelakunya tidak relevan: *"Sampel dinormalisasi terhadap total protein."*
- **Orang-pertama jamak "kami"** adalah baku; jangan tulis ulang untuk menghindarinya.
- **Titik koma dan sesekali deret tiga** boleh secukupnya. Pengecualian adalah em-dash: hapus seluruhnya (Lapisan 1), ganti dengan koma, titik dua, tanda kurung, atau kalimat terpisah.
- **Definisi formal, nama metode/metrik, istilah teknis, persamaan, dan simbol** tetap verbatim.
- **Jangan pernah mengarang, menghapus, atau mengubah angka, persamaan, atau sitasi.** Isi sama; pertahankan setiap kunci sitasi.
- Ikuti EYD dan KBBI untuk ejaan; gunakan koma desimal Indonesia (0,91) untuk naskah Indonesia, kecuali venue meminta titik desimal.

---

## Lapisan 4: Disiplin klaim-bukti
Untuk setiap klaim empiris, periksa (a) apakah didukung angka, gambar, tabel, atau sitasi dalam teks, dan (b) apakah kata kerjanya sesuai dengan kekuatan bukti tersebut?

- **Klaim tanpa bukti -> tambahkan penunjuk bukti atau lunakkan.**
  *Sebelum:* *Metode kami lebih robust.* *Sesudah:* *Akurasi metode kami turun 2 poin pada pergeseran distribusi, berbanding 11 poin untuk baseline (Gambar 3).*
- **Kata kerja lebih kuat dari bukti -> turunkan.**
  *Sebelum:* *Ini menunjukkan bahwa metode kami unggul secara universal.*
  *Sesudah:* *Pada ketiga dataset ini, metode kami menyamai atau melampaui baseline terkuat (Tabel 2).*
- **Besaran samar -> angka atau RENTANG, dengan atribusi.**
  *Sebelum:* *peningkatan besar.* *Sesudah:* *peningkatan 2–6% pada balanced accuracy dibandingkan baseline terkuat.*
  Utamakan rentang (mis. "2–6%") daripada rata-rata tunggal kecuali metode perataannya dinyatakan, dan atribusikan setiap angka pada metode, metrik, dan baseline-nya. Saat membandingkan, dahulukan perbandingan terhadap kompetitor terkuat, bukan baseline yang lemah.

---

## Lapisan 5: Penyesuaian suara dan venue
Jika penulis menyertakan makalah sebelumnya, baca dulu sampelnya dan catat ritme kalimat, kebiasaan konjungsi, kadar dan letak hedging, cara membuka bagian, notasi, dan frasa berulang, lalu sesuaikan. Sesuaikan juga dengan register venue (mis. ICLR/NeurIPS: ringkas, langsung, mengedepankan hasil; Nature/PNAS: lebih ekspositoris; jurnal nasional Sinta/Garuda: ikuti template dan gaya selingkung; skripsi/tesis/disertasi: ikuti pedoman kampus, bab dan sistematika baku). Tanpa sampel, gunakan prosa yang bersih, presisi, dan sesuai venue, bukan gaya kasual dan beropini ala humanizer umum.

## Lapisan 6: Mode proposal pendanaan (Kemdiktisaintek/DRTPM, LPDP, BRIN, NSF, NIH)
Proposal bukan makalah. Ia dinilai dari **visi plus kelayakan**, bukan dari hasil jadi, dan reviewer memberi skor. Pergeseran register penting: bahasa ambisi yang akan dipangkas pada lapisan makalah ("tujuan jangka panjang", "perintis", "transformatif", "meletakkan fondasi") adalah *tepat dan diharapkan* di sini, asal didukung rencana dan bukti yang kredibel. Jadi dalam mode proposal, **jangan ratakan visinya**; tegakkan disiplin yang berbeda: **klaim <-> kelayakan**.

### 6.1 Kenali struktur; skor hidup di halaman pertama
Reviewer membentuk skor dari pembuka, lalu memindai sisanya untuk konfirmasi. Curahkan upaya penyuntingan terbesar di sana.
- **Hibah Indonesia (DRTPM/Kemdiktisaintek, LPDP, BRIN).** Umumnya: **Ringkasan** satu halaman, lalu **Latar belakang/Urgensi -> Tujuan jangka panjang -> Tujuan khusus proposal ini -> Kesenjangan (gap) -> Metode/tahapan -> Luaran -> Dampak/manfaat**, idealnya dalam 1–2 halaman pertama, dengan satu bagan ringkas. Dampak (pengabdian, hilirisasi, TKT/TKDN, IKU) harus substantif dan terintegrasi, bukan tempelan.
- **NSF.** Ringkasan satu halaman **Project Summary** dengan tiga kepala kriteria: **Overview**, **Intellectual Merit**, **Broader Impacts**, masing-masing mandiri. Project Description dibuka dengan **visi jangka panjang -> tujuan proposal ini -> kesenjangan -> thrust/aim spesifik -> payoff**, idealnya dalam 1–2 halaman pertama, dengan satu gambar overview.
- **NIH (R01).** **Halaman Specific Aims adalah seluruh proposal dalam satu halaman**, dan paling menentukan. Alur baku: (1) pembuka: masalah, apa yang diketahui, **kesenjangan/kebutuhan kritis**; (2) **tujuan jangka panjang** dan **hipotesis sentral** beserta rasionalnya; (3) "**Tujuan aplikasi ini adalah...**" plus bagaimana hipotesis dirumuskan; (4) **2–3 Aim**, masing-masing satu baris tujuan + frasa pendekatan + luaran yang diharapkan; (5) paragraf **payoff**: apa yang berubah jika berhasil. Lalu **Significance, Innovation, Approach** sebagai bagian yang dinilai terpisah.

### 6.2 Primasi 3 halaman pertama (sunting bagian ini paling keras)
Pada akhir halaman 1 (NIH Aims) atau hlm. ~2–3 (NSF/hibah Indonesia), pembaca harus sudah memegang: **hook** (mengapa penting, secara konkret), **gap** (apa yang hilang dan biaya dari kesenjangan itu), **ide sentral** (pendekatan dalam satu kalimat), **aim/tujuan** (tajam dan paralel), dan **payoff**. Jika ada yang hilang atau terkubur, perbaiki itu sebelum menyentuh bagian belakangan. Reviewer yang tidak yakin pada halaman 3 tidak akan pulih pada halaman 10.

### 6.3 Langkah lemah khas proposal yang harus diperbaiki
- **Urgensi samar.** *Waspadai:* "masalah penting/mendesak", "X memiliki banyak aplikasi".
  **Sebelum:** *Memahami masalah ini sangat penting.*
  **Sesudah:** *Tanpa batas atas bagaimana noise pengukuran merambat ke diagnosis, model klinis disetel secara coba-coba, inefisiensi yang dihapus oleh proposal ini.*
- **Metode-sebagai-tujuan** (tujuan menyebut teknik, bukan pertanyaan atau luaran).
  **Sebelum:** *Tujuan 2: Menerapkan transfer learning pada dataset.*
  **Sesudah:** *Tujuan 2: Menentukan apakah fusi sinyal wearable dan lab meningkatkan deteksi dini, dan untuk subkelompok pasien mana ia membantu atau merugikan.*
- **Tujuan domino** (Tujuan 2/3 runtuh jika Tujuan 1 gagal; reviewer menandainya rapuh). *Perbaikan:* rumuskan tujuan secara **paralel dan masing-masing bernilai mandiri**; bila satu bergantung pada yang lain, nyatakan fallback-nya.
- **Ambisi tanpa kelayakan.** Setiap klaim berani butuh pijakan: data pendahuluan, hasil/publikasi sebelumnya, teorema klasik yang dibangun, atau mitra/surat dukungan. *Perbaikan:* lampirkan bukti di samping klaim ("hasil pendahuluan kami pada Gbr. X menunjukkan...", "berpijak pada lower bound minimax klasik...").
- **Dampak/pelatihan boilerplate.** *Waspadai:* "kami akan membimbing mahasiswa dan diseminasi via seminar dan publikasi." *Perbaikan:* buat konkret, terenumerasi, dan terkait riset: program spesifik, mata kuliah atau tools bernama, outreach terukur.
- **Hipotesis sentral yang ragu-ragu.** Hipotesis di halaman Aims adalah komitmen yang falsifiable, bukan "kami akan mengeksplorasi apakah mungkin...". Hedging terkalibrasi milik bagian Metode/interpretasi, bukan klaim sentral.

### 6.4 Pertahankan dan manfaatkan (craft proposal yang didanai)
Ini terbaca sebagai kekuatan; pertahankan atau tambahkan alih-alih menyuntingnya keluar.
- **Bingkai visi/ambisi**: tujuan jangka panjang yang berani di depan, dengan proposal ini sebagai satu langkah berprinsip ke arahnya.
- **Lead-in run-in agar mudah dipindai**: tebal/miring **Tujuan:**, **Motivasi:**, **Inovasi:**, *Thrust/Tujuan N (misi satu baris):*. Reviewer memindai; struktur yang terlihat menghemat waktu.
- **Contoh berjalan atau protagonis konkret** untuk membuat metode abstrak hidup dan konsisten antar tujuan.
- **Pernyataan tantangan/tujuan tajam sebagai pertanyaan**: pertanyaan terbuka yang tajam terbaca sebagai masalah yang well-posed (satu pertanyaan boxed/set-off per tujuan baik).
- **Menjangkarkan kebaruan pada hasil klasik bernama yang dalam** untuk memberi sinyal rigor dan silsilah: ketaksamaan, notion kapasitas, atau uji yang dikenal yang digeneralisasi metode baru.
- **Mengedepankan rekam jejak tim sebagai bukti kelayakan**: hibah sebelumnya, hasil pendahuluan, publikasi, mitra, dan mitra demonstrasi milik *awal*, sebagai bukti rencana dapat dieksekusi. Rekam jejak nyata adalah bukti, bukan membual; letakkan di mana ia mengurangi risiko tujuan. *(Gunakan hanya rekam jejak PI yang nyata dan diberikan; jangan mengarang pendanaan, hasil, mitra, atau surat.)*

### 6.5 Klaim <-> kelayakan (padanan proposal dari Lapisan 4)
Untuk setiap tujuan dan luaran yang dijanjikan, periksa: apakah ambisi diimbangi cara yang kredibel, seperti data pendahuluan, metode sebelumnya, fondasi klasik, mitra, atau de-risking bertahap? Jika ya, pertahankan kata kerja ambisius. Jika tidak, lampirkan bukti yang hilang atau skalakan klaim sesuai rencana. Jangan mengarang hasil pendahuluan, pendanaan sebelumnya, mitra, atau surat; jika dukungan tidak ada, tandai kesenjangannya untuk penulis alih-alih menutupinya.

---

## Keluaran
Kembalikan teks bersih plus laporan perubahan singkat dalam Bahasa Indonesia: pola yang dihapus (per jenis), klaim yang dilunakkan atau diberi penunjuk bukti, dan catatan suara/venue. Konfirmasi bahwa tidak ada angka, persamaan, atau sitasi yang diubah.
