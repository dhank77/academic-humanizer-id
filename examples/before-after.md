# Sebelum / sesudah (register akademik Bahasa Indonesia)

**Sebelum (ciri AI + klaim berlebihan):**
> Dalam beberapa tahun terakhir, pembelajaran representasi graf telah menarik perhatian yang meningkat. Dalam makalah ini, kami mengusulkan metode baru dan membuktikan melalui eksperimen ekstensif bahwa metode ini secara signifikan mengungguli pendekatan yang ada, membuka jalan bagi paradigma baru. Sepengetahuan kami, ini adalah karya pertama yang menggali masalah krusial ini.

**Sesudah (di-humanize akademik):**
> Metode graf yang ada untuk klasifikasi node tak-seimbang membobot ulang loss tetapi mengabaikan label-noise. Kami menambahkan suku pembobot sadar-noise dan mengevaluasinya pada tiga benchmark sitasi, di mana ia meningkatkan F1 kelas-minoritas sebesar 3–6 poin dibandingkan focal loss sementara akurasi kelas-mayoritas tetap dalam 1 poin.

Yang berubah: menghapus pembuka formulaik, "baru", "ekstensif", "secara signifikan" (tanpa kuantifikasi), "membuka jalan", dan "sepengetahuan kami"; menurunkan "membuktikan" menjadi "mengevaluasi"; melampirkan rentang dan pembanding; mempertahankan klaim faktual yang presisi.

---

## Mode proposal pendanaan: pembuka halaman Tujuan (Lapisan 6)

Proposal dinilai dari halaman pertama, dan registernya berbeda dari makalah: visi dan kelayakan adalah produknya, sehingga ambisi *dipertahankan* dan dikaitkan dengan bukti, bukan dipangkas. Contoh buatan ini menunjukkan langkah pembuka halaman Tujuan.

**Sebelum (urgensi samar, metode-sebagai-tujuan, domino, tanpa kelayakan):**
> Deteksi dini sepsis adalah masalah yang sangat penting dan mutakhir dengan banyak aplikasi. Dalam proposal ini kami akan mengeksplorasi apakah machine learning mungkin dapat membantu. Tujuan 1: menerapkan model kami pada data ICU. Tujuan 2: memperluas Tujuan 1 ke data multi-situs. Tujuan 3: jika Tujuan 1–2 berhasil, jalankan pilot. Penelitian ini akan menjadi terobosan dan berdampak besar pada bidang ini.

**Sesudah (gap + komitmen sentral + tujuan paralel berbingkai-luaran + payoff + kelayakan):**
> Sepsis dapat diobati bila tertangkap dini, tetapi skor bedside berbunyi terlambat dan terlalu sering, sehingga klinisi tidak dapat membedakan alarm benar dari noise. **Tujuan aplikasi ini adalah** menghasilkan model peringatan dini yang terkalibrasi dan transferable sehingga dapat ditindaklanjuti. Hipotesis sentral kami, didukung hasil pendahuluan satu-situs (Gbr. 1), adalah bahwa fusi tren vital-sign kontinu dengan lab rutin mendeteksi perburukan beberapa jam lebih awal tanpa menaikkan angka alarm-palsu.
> **Tujuan 1: Menetapkan** batas deteksi-vs-alarm-palsu pada data ICU retrospektif dan model yang mendekatinya, dengan kalibrasi dikuantifikasi via proper scoring rule.
> **Tujuan 2: Menentukan** apakah penambahan lab rutin pada tren vital-sign meningkatkan deteksi dini, dan untuk subkelompok pasien mana ia membantu atau merugikan.
> **Tujuan 3: Mengkuantifikasi** bagaimana kalibrasi alarm tertransfer antar-situs, menggunakan rumah sakit yang di-hold-out secara prospektif.
> Ketiga tujuan independen: masing-masing menghasilkan luaran yang dapat dipakai sendiri. **Dampak:** alat peringatan dini yang terkalibrasi dan transferable, dievaluasi bersama dua rumah sakit mitra (surat terlampir).

Yang berubah: mengganti "sangat penting dan mutakhir … banyak aplikasi" dengan gap klinis spesifik dan biayanya; mengubah klaim sentral yang ragu menjadi hipotesis falsifiable yang terikat data pendahuluan; menulis ulang metode-sebagai-tujuan menjadi tujuan berbingkai-luaran dan menghapus domino Tujuan-3-tergantung-1-dan-2 (kini paralel); menyebut jangkar rigor konkret (proper scoring rule untuk kalibrasi); mengganti "terobosan … dampak besar" dengan payoff konkret dan bukti kelayakan (gambar pendahuluan, surat mitra). Ambisi tetap, dan kini didukung. *(Contoh ini generik; pada pemakaian nyata, sitir hanya rekam jejak PI sendiri, dan jangan mengarang data pendahuluan, pendanaan, atau surat.)*

---

## Mode proposal: Ringkasan hibah (gaya DRTPM/LPDP/BRIN, diadaptasi dari contoh NSF CAREER)

**Sebelum (buatan AI; visi tenggelam dalam ciri AI):**
> Dalam beberapa tahun terakhir, kecerdasan artifisial telah menarik perhatian yang meningkat dan mencapai kesuksesan luar biasa di berbagai bidang. Namun, terlepas dari kemajuan ini, continual learning tetap menjadi tantangan krusial dan penting yang sangat utama. Dalam proposal ini, kami mengusulkan kerangka baru dan komprehensif yang memanfaatkan teknik mutakhir untuk menggali tantangan rumit continual learning, membuka jalan bagi paradigma baru yang transformatif. Sepengetahuan kami, ini adalah kerangka pertama yang secara mulus menyatukan aspek-aspek ini, menggarisbawahi potensinya untuk merevolusi bidang ini. Melalui eksperimen ekstensif, kami akan membuktikan bahwa pendekatan terobosan kami secara signifikan mengungguli metode yang ada. Rencana pendidikan kami juga akan memfasilitasi generasi peneliti berikutnya.

**Sesudah (diadaptasi dari Ringkasan NSF CAREER yang didanai, Overview):**
> Seiring meluasnya data dan lingkungan belajar, nilai AI bergantung pada kemampuannya untuk diskalakan dan beradaptasi. Continual learning menjawab ini: pembelajar yang mempertahankan kinerja pada tugas lama sambil mengintegrasikan informasi baru, beradaptasi ke lingkungan baru dengan mengingat pengetahuan lama, dan secara aktif meminta informasi sampingan untuk belajar lebih cepat dan akurat. Metode continual-learning yang ada, meskipun menjanjikan, sebagian besar bersifat empiris, dengan prinsip yang tidak jelas mendasari perilakunya, sehingga membatasi keandalan maupun kemajuan lebih lanjut. Proposal ini membangun kerangka berprinsip yang menyatukan ciri-ciri tersebut melalui desain teori dan algoritma yang terkopel, dalam tiga lapis: memori evolutif untuk pertumbuhan kapabilitas, supervisi lunak untuk akselerasi belajar, dan pengetahuan lintas-domain untuk akurasi. Pekerjaan ini akan memajukan teori continual learning, memperkaya algoritmanya, dan merilis paket yang skalabel, didemonstrasikan pada mengemudi otonom dan manajemen kinerja seluler. Rencana pendidikan terintegrasi melatih generasi ilmuwan data berikutnya melalui program STEM baru dan platform open-source.

Yang berubah: memotong pembuka formulaik dan kosakata AI (menggali, rumit, mulus, memanfaatkan, mutakhir); menghapus klaim berlebihan (baru, terobosan, merevolusi, "sepengetahuan kami", "secara signifikan mengungguli" tanpa bukti); mengganti "sangat utama" dengan gap konkret (metode bersifat empiris, prinsip tidak jelas) dan biayanya (keandalan, kemajuan). Yang **dipertahankan** justru yang akan dipangkas berlebihan oleh lapisan makalah tetapi dibutuhkan proposal: visi jangka panjang, kerangka tiga-lapis, domain demonstrasi bernama, dan rencana pendidikan terintegrasi. Dalam mode proposal, ambisi tetap; hanya dibuat spesifik dan kredibel.
