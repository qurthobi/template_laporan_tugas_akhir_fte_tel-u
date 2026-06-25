# Template LaTeX Laporan Tugas Akhir FTE Telkom University

Template LaTeX untuk penyusunan **Laporan Tugas Akhir Fakultas Teknik Elektro (FTE), Universitas Telkom**.

Template ini dikembangkan untuk membantu mahasiswa dalam menyusun laporan tugas akhir secara lebih konsisten, terstruktur, dan efisien dengan memanfaatkan ekosistem LaTeX. Selain menyediakan format dokumen yang telah disesuaikan dengan pedoman umum penulisan tugas akhir, template ini juga mendukung pengelolaan referensi secara otomatis menggunakan BibLaTeX dan Biber.

> **Catatan:** Template ini merupakan proyek independen dan bukan produk resmi Universitas Telkom. Pengguna tetap disarankan untuk memeriksa kesesuaian format dengan pedoman tugas akhir terbaru yang berlaku.

---

## Fitur Utama

* Format halaman sesuai pedoman umum Tugas Akhir FTE
* Struktur laporan tugas akhir lengkap
* Dukungan Bahasa Indonesia
* Daftar Isi otomatis
* Daftar Gambar otomatis
* Daftar Tabel otomatis
* Penomoran bab dan subbab otomatis
* Dukungan glosarium dan daftar singkatan
* Sitasi dan daftar pustaka format IEEE
* Manajemen referensi menggunakan BibLaTeX dan Biber
* Kompatibel dengan TeX Live, MiKTeX, dan Overleaf
* Template abstrak Bahasa Indonesia dan Bahasa Inggris
* Template lampiran
* Template lembar orisinalitas dan lembar pengesahan

---

## Struktur Dokumen

```text
.
├── Chapters/
│   ├── 1_Pendahuluan.tex
│   ├── 2_Tinjauan_Pustaka.tex
│   ├── 3_Perancangan_Sistem.tex
│   ├── 4_Hasil_Pengujian_dan_Analisis.tex
│   └── 5_Kesimpulan_dan_Saran.tex
│
├── FrontMatter/
│   ├── HalamanCover.tex
│   ├── LembarPengesahan.tex
│   ├── LembarOrisinalitas.tex
│   ├── Abstrak.tex
│   ├── Abstract.tex
│   ├── KataPengantar.tex
│   └── UcapanTerimaKasih.tex
│
├── Gambar/
├── lampiran.tex
├── glossaries.tex
├── referensi.bib
├── main.tex
├── template_tugas_akhir_fte.sty
└── indonesian.lbx
```

---

## Persyaratan

Template ini dapat digunakan pada:

* TeX Live
* MiKTeX
* Overleaf

Bibliografi menggunakan:

* BibLaTeX
* Biber

Pastikan proses kompilasi menggunakan **Biber**, bukan BibTeX.

---

## Cara Penggunaan

### 1. Clone Repository

```bash
git clone https://github.com/qurthobi/template_laporan_tugas_akhir_fte_tel-u.git
```

### 2. Edit Informasi Awal

Lengkapi informasi pada folder:

```text
FrontMatter/
```

seperti:

* Nama mahasiswa
* NIM
* Judul tugas akhir
* Program studi
* Dosen pembimbing
* Abstrak Bahasa Indonesia
* Abstract Bahasa Inggris

### 3. Tulis Isi Tugas Akhir

Isi setiap bab pada folder:

```text
Chapters/
```

yang terdiri dari:

* BAB I Pendahuluan
* BAB II Tinjauan Pustaka
* BAB III Perancangan Sistem / Metodologi
* BAB IV Hasil dan Analisis
* BAB V Kesimpulan dan Saran

### 4. Tambahkan Referensi

Simpan seluruh referensi pada file:

```text
referensi.bib
```

Contoh:

```bibtex
@article{example2025,
  author  = {John Doe},
  title   = {Example Paper},
  journal = {IEEE Access},
  year    = {2025}
}
```

Kemudian sitasikan pada dokumen:

```latex
\cite{example2025}
```

### 5. Tambahkan Gambar

Simpan gambar pada folder:

```text
Gambar/
```

dan panggil menggunakan:

```latex
\begin{figure}[ht]
\centering
\includegraphics[width=0.8\textwidth]{Gambar/nama_gambar}
\caption{Contoh gambar}
\label{fig:contoh}
\end{figure}
```

---

## Kompilasi Dokumen

### Menggunakan Terminal

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

### Menggunakan Overleaf

Atur compiler ke:

```text
LaTeX → Biber → PDF
```

atau gunakan fitur build otomatis yang tersedia pada Overleaf.

---

## Sitasi dan Daftar Pustaka

Template ini menggunakan gaya sitasi **IEEE**.

Contoh:

```latex
Penelitian sebelumnya menunjukkan hasil yang baik \cite{example2025}.
```

Hasil:

```text
Penelitian sebelumnya menunjukkan hasil yang baik [1].
```

Seluruh referensi dikelola melalui file:

```text
referensi.bib
```

Pengguna disarankan menggunakan perangkat lunak manajemen referensi seperti:

* Zotero
* Mendeley
* JabRef

untuk menghasilkan entri BibTeX secara otomatis.

---

## Pelaporan Masalah

Apabila menemukan:

* Bug pada template
* Kesalahan format
* Ketidaksesuaian dengan pedoman terbaru
* Kesalahan terjemahan
* Saran fitur baru

silakan membuat Issue pada repository GitHub atau menghubungi pengembang.

---

## Kontribusi

Kontribusi sangat terbuka untuk seluruh pengguna.

Langkah kontribusi:

1. Fork repository.
2. Buat branch baru.
3. Lakukan perubahan.
4. Commit perubahan.
5. Buat Pull Request.

Seluruh masukan dan kontribusi akan sangat membantu dalam pengembangan template ini.

---

## Pengembang

Dikembangkan oleh:

**Ahmad Qurthobi**

GitHub:
https://github.com/qurthobi

---

## Dukungan

Apabila template ini membantu dalam penyusunan tugas akhir Anda, pertimbangkan untuk memberikan ⭐ pada repository GitHub agar proyek ini dapat menjangkau lebih banyak pengguna.

---

## Lisensi

Template ini didistribusikan untuk keperluan pendidikan, penelitian, dan pengembangan akademik.

Silakan gunakan, modifikasi, dan distribusikan sesuai kebutuhan dengan tetap mencantumkan atribusi kepada pengembang asli.
