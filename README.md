# Prediksi Biaya Tagih Fasilitas Kesehatan (Tuberkulosis) 🏥💰

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.2.2-orange)

## 📊 Deskripsi Proyek
Proyek ini menggunakan **Random Forest Regression** untuk memprediksi **biaya tagih oleh fasilitas kesehatan (provider)** untuk pasien dengan penyakit **Tuberkulosis**, berdasarkan data **BPJS Kesehatan Tahun 2021**.  

Model ini berguna untuk:
- Analisis biaya kesehatan
- Perencanaan anggaran di fasilitas kesehatan
- Pemahaman pola klaim biaya pasien Tuberkulosis

---
## 📂 Data
- **Sumber:** BPJS Kesehatan Tahun 2022  
- **Jenis Data:** CSV
- **Fitur Utama:**
  - Tanggal lahir peserta
  - Tanggal kunjungan dan pulang fasilitas kesehatan
  - Jenis layanan dan diagnosa
  - Fasilitas kesehatan (provider)
  - Biaya tagih  
---

## ⚙️ Metodologi
1. **Preprocessing**
   - Tangani missing values
   - Transformasi tanggal menjadi fitur numerik (usia, durasi rawat)
   - Encoding fitur kategori (misal: provider, diagnosa)

2. **Feature Selection**
   - Memilih fitur relevan untuk prediksi biaya tagih

3. **Modeling**
   - Algoritma: `RandomForestRegressor`
   - Split data: Training & Testing

4. **Evaluasi Model**
   - Metrics: RMSE, MAE, R² Score
---

## 🛠️ Cara Menjalankan
```bash
# Clone repository
git clone https://github.com/username/repo.git

# Masuk ke folder proyek
cd repo

# Install dependencies
pip install -r requirements.txt

# Jalankan model
python run_model.py
```

## 🧩 Struktur Proyek
```
📦 Prediksi-Biaya-Tagih-TB
├── run_model.py           # Script utama untuk preprocessing, training, dan prediksi
├── data/
│   └── bpjs_tb_2022.csv  # Data klaim pasien Tuberkulosis
├── model/
│   └── random_forest.pkl  # Model Random Forest yang telah dilatih (opsional)
├── requirements.txt       # Library yang dibutuhkan
└── README.md              # Dokumentasi proyek
```

## 📈 Hasil
- Model mampu memprediksi biaya tagih dengan akurasi tinggi menggunakan Random Forest
- Dapat membantu analisis biaya dan perencanaan anggaran di fasilitas kesehatan
