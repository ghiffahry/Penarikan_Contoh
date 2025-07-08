
---

## 📌 Deskripsi Proyek

Simulasi ini bertujuan untuk:

- Membandingkan berbagai **desain sampling berpeluang** (SRS, stratifikasi, klaster, multistage) dengan metode non-probabilistik populer yaitu **metode Slovin**.
- Menggunakan dataset sintetis dengan struktur **kabupaten → kecamatan → desa/kelurahan**, dan individu yang memiliki **pendapatan**.
- Mengevaluasi desain sampling berdasarkan **akurasi pendugaan total dan rata-rata** serta **efisiensi ukuran contoh**.

---

## 🔧 Module yang Digunakan

- Python 3.11+
- NumPy, Pandas, SciPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📐 Metodologi Simulasi

### 1. Struktur Populasi
- 15 kabupaten, masing-masing terdiri dari 3–6 kecamatan, dan tiap kecamatan terdiri dari 5–9 desa/kelurahan.
- Desa (60%) memiliki 30–50 penduduk.
- Kelurahan (40%) memiliki 45–88 penduduk.

### 2. Distribusi Pendapatan
- Desa: \( G \sim \Gamma(2,1) \), disesuaikan ke Rp1–3 juta.
- Kelurahan: \( H \sim \Gamma(2,2) \), disesuaikan ke Rp4–8 juta.

### 3. Evaluasi Desain Sampling
- Ukuran sampel tetap (misal: 225).
- Evaluasi error: MAE, ARB, RRMSE.
- Efisiensi: biaya vs akurasi.
- Analisis Slovin untuk pembanding eksploratif.

---

## 🧠 Insight dan Rekomendasi

- Gunakan **Stratified Sampling** bila informasi strata tersedia (desa vs kelurahan).
- Terapkan **Multistage Sampling** jika wilayah luas dan biaya tinggi.
- Hindari **Slovin** untuk survei estimatif serius; gunakan hanya eksploratif.

---
