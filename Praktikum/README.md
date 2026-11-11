# IF2514505 - Praktikum Pengolahan Citra Digital

Repositori ini berisi kumpulan tugas, modul, serta hasil pengerjaan praktikum untuk mata kuliah **Pengolahan Citra Digital (IF2514505)** pada Program Studi Informatika, Institut Teknologi Kalimantan (ITK).

---

## 👤 Informasi Mahasiswa

- **Nama**: Muhammad Wisnu Wardhana
- **NIM**: 11241063
- **Kelas**: Praktikum PCD - Kelas A
- **Semester**: 5

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
3. **Pengolahan Citra Lanjutan**: Meliputi perbaikan domain frekuensi (Transformasi Fourier), restorasi citra, operasi morfologi, dan segmentasi citra.

---

## 📂 Struktur Repositori

```text
IF2514505/
└── Praktikum/
    ├── README.md                                                 # Dokumentasi praktikum
    └── PraktikumPCD_SubCPMK2_11241063_Muhammad_Wisnu_Wardhana.ipynb # Modul Sub-CPMK-2 (Perbaikan Domain Spasial)
```

---

## 🛠️ Kebutuhan Lingkungan & Pustaka (Prerequisites)

Untuk menjalankan notebook praktikum, pastikan telah terpasang Python 3.8+ beserta dependensi berikut:

- **Jupyter Notebook / JupyterLab / Google Colab**
- **NumPy**: Komputasi matriks dan array numerik
- **Matplotlib**: Visualisasi citra, grafik perbandingan, dan histogram
- **OpenCV (`opencv-python`)**: Manipulasi citra performa tinggi
- **scikit-image**: Operasi pemrosesan citra ilmiah

Pemasangan pustaka via pip:
```bash
pip install numpy matplotlib opencv-python scikit-image jupyter
```

---

## 📚 Rujukan Utama

- Gonzalez, R.C. & Woods, R.E. (2018). *Digital Image Processing*, 4th Edition. Pearson.
- Modul Praktikum Pengolahan Citra Digital, Program Studi Informatika, Institut Teknologi Kalimantan.
