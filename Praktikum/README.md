# IF2514505 - Praktikum Pengolahan Citra Digital

Repositori ini berisi kumpulan tugas, modul, serta hasil pengerjaan praktikum untuk mata kuliah **Pengolahan Citra Digital (IF2514505)** pada Program Studi Informatika, Institut Teknologi Kalimantan (ITK).

---

## 👤 Informasi Mahasiswa

| | |
|---|---|
| **Nama** | Muhammad Wisnu Wardhana |
| **NIM** | 11241063 |
| **Kelas / Kelompok** | Praktikum PCD - Kelas A |
| **Semester** | 5 |
| **Repositori** | [nirvanaguys/IF2514505](https://github.com/nirvanaguys/IF2514505) |

---

## 📖 Deskripsi Mata Kuliah & Praktikum

Mata kuliah **Pengolahan Citra Digital (Digital Image Processing)** mempelajari konsep dasar dan teknik manipulasi citra digital secara algoritmik untuk meningkatkan kualitas citra (*image enhancement*), mengekstraksi informasi, merestorasi citra dari derau, serta melakukan transformasi dan segmentasi citra.

Praktikum ini dirancang untuk memberikan pengalaman langsung dalam mengimplementasikan teori pemrosesan citra digital menggunakan bahasa pemrograman **Python** dan pustaka ilmiah komputasi citra.

### 🎯 Tujuan & Capaian Pembelajaran (CPMK)
1. **Representasi & Manipulasi Dasar Citra**: Memahami struktur citra digital, matriks piksel, resolusi, ruang warna (Grayscale, RGB, HSV), dan transformasi dasar intensitas.
2. **Perbaikan Citra pada Domain Spasial (Sub-CPMK-2)**:
   - Transformasi intensitas melalui Lookup Table (LUT), transformasi logaritmik, dan koreksi gamma (*power-law*).
   - Pengolahan histogram: Histogram Equalization (HE), Histogram Matching (Spesifikasi), dan Contrast Limited Adaptive Histogram Equalization (CLAHE).
   - Penapisan Spasial (*Spatial Filtering*): Korelasi, konvolusi, penghalusan citra (*blurring/smoothing* menggunakan filter rata-rata dan Gaussian), serta penajaman citra (*sharpening* menggunakan Laplacian dan Unsharp Masking).
3. **Transformasi & Penapisan Domain Frekuensi (Sub-CPMK-3)**:
   - DFT 1D dan 2D dari definisi serta pembandingan hasilnya dengan `numpy.fft`.
   - Spektrum amplitudo, pemusatan spektrum (`fftshift`), dan peran informasi fase.
   - Penapis lolos-rendah (Ideal, Butterworth, Gaussian), penapis lolos-tinggi, serta pembuktian kesetaraan domain spasial–frekuensi.
   - Studi kasus: penghapusan derau periodik dengan penapis takik (*notch filter*).
4. **Transformasi Ruang Warna (Sub-CPMK-4)**:
   - Konversi RGB ↔ HSI, HSV, dan CIELAB dari definisi (Gonzalez Bab 6).
   - Ketahanan representasi warna terhadap perubahan pencahayaan dan derau.
   - Pemrosesan citra berwarna: ekualisasi per kanal RGB vs. ekualisasi intensitas.
   - Segmentasi berbasis warna dengan jarak Euclidean dan Mahalanobis.

---

## 📂 Daftar Praktikum

| No | Sub-CPMK | Topik | Berkas | Status |
|:--:|:---------|:------|:-------|:------:|
| 1 | Sub-CPMK-2 | Perbaikan Citra pada Domain Spasial | `11241063_Muhammad_Wisnu_Wardhana_Praktikum1` | ✅ Selesai |
| 2 | Sub-CPMK-3 | Transformasi dan Penapisan pada Domain Frekuensi | `11241063_Muhammad_Wisnu_Wardhana_Praktikum2.ipynb` | ✅ Selesai |
| 3 | Sub-CPMK-4 | Transformasi Ruang Warna untuk Analisis dan Pemrosesan Citra | `11241063_Muhammad_Wisnu_Wardhana_Praktikum3.ipynb` | ✅ Selesai |

> ⚠️ Berkas Praktikum 1 tersimpan **tanpa ekstensi** `.ipynb`, padahal isinya notebook JSON yang valid. Tambahkan ekstensi `.ipynb` setelah mengunduh agar dapat langsung dibuka di Jupyter/Colab.

---

## 📁 Struktur Repositori

```text
IF2514505/
├── README.md                                             # Dokumentasi utama (ringkasan)
└── Praktikum/
    ├── README.md                                         # Dokumentasi praktikum (berkas ini)
    ├── 11241063_Muhammad_Wisnu_Wardhana_Praktikum1       # Sub-CPMK-2: Domain Spasial
    ├── 11241063_Muhammad_Wisnu_Wardhana_Praktikum2.ipynb # Sub-CPMK-3: Domain Frekuensi
    └── 11241063_Muhammad_Wisnu_Wardhana_Praktikum3.ipynb # Sub-CPMK-4: Ruang Warna
```

---

## 🛠️ Kebutuhan Lingkungan & Pustaka (Prerequisites)

Untuk menjalankan notebook praktikum, pastikan telah terpasang **Python 3.8+** (notebook dikembangkan pada Python 3.13) beserta dependensi berikut:

- **Jupyter Notebook / JupyterLab / Google Colab**
- **NumPy** — komputasi matriks dan array numerik (termasuk `numpy.fft`)
- **Matplotlib** — visualisasi citra, grafik perbandingan, dan histogram
- **OpenCV (`opencv-python`)** — manipulasi citra performa tinggi
- **scikit-image** — operasi pemrosesan citra ilmiah (mis. `rgb2hsv`, `rgb2lab`)
- **SciPy** — konvolusi dan statistik pendukung

Pemasangan pustaka via pip:
```bash
pip install numpy matplotlib opencv-python scikit-image scipy jupyter
```

---

## ▶️ Cara Menjalankan Notebook

1. Klon repositori:
   ```bash
   git clone https://github.com/nirvanaguys/IF2514505.git
   cd IF2514505/Praktikum
   ```
2. Jalankan Jupyter Notebook/Lab:
   ```bash
   jupyter notebook
   ```
   atau unggah berkas `.ipynb` ke [Google Colab](https://colab.research.google.com/).
3. Pilih **Run All** untuk menjalankan seluruh sel dari awal. Semua citra uji dibangkitkan secara sintetis pada **Bagian 0**, sehingga tidak diperlukan berkas citra eksternal.

> Sebelum menjalankan, ubah nama berkas Praktikum 1 agar berakhiran `.ipynb`.

---

## 📝 Catatan Pengerjaan

- Setiap notebook terdiri atas **Bagian 0 (Persiapan)**, beberapa bagian materi berisi **TODO**, lalu **blok Analisis** yang dijawab memakai angka dari sel yang dijalankan sendiri.
- Jawaban analisis ditulis berdasarkan hasil eksekusi nyata, bukan perkiraan. Penggunaan alat bantu AI dicantumkan pada bagian *Daftar periksa* di akhir notebook.
- Setiap notebook diakhiri **daftar periksa (checklist)** sebagai verifikasi sebelum dikumpulkan.

---

## 📚 Rujukan Utama

- Gonzalez, R.C. & Woods, R.E. (2018). *Digital Image Processing*, 4th Edition. Pearson.
- Zuiderveld, K. (1994). *Contrast Limited Adaptive Histogram Equalization*. Graphics Gems IV, Academic Press.
- Modul Praktikum Pengolahan Citra Digital, Program Studi Informatika, Institut Teknologi Kalimantan.
