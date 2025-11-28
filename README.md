# Prediksi Biaya Tagih Fasilitas Kesehatan (Tuberkulosis) 🏥💰

![Python](https://img.shields.io/badge/Python-3.11-blue)

## 📊 Deskripsi Proyek
Proyek ini menggunakan **Random Forest Regression** untuk memprediksi **biaya tagih oleh fasilitas kesehatan (provider)** untuk pasien dengan penyakit **Tuberkulosis**, berdasarkan data **BPJS Kesehatan Tahun 2021**.  

Model ini berguna untuk:
- Analisis biaya kesehatan
- Perencanaan anggaran di fasilitas kesehatan
- Pemahaman pola klaim biaya pasien Tuberkulosis

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

## 🧩 Struktur Proyek
```
📦 Prediksi-Biaya-Tagih-TB
├── prediksi Biaya Tagih - oleh fasilitas kesehatan (provider)penyakit TB.ipynb           # Script utama untuk preprocessing, training, dan prediksi
├── data/
|   └── data_baru_tb_fkrtl.csv        # data baru
|   └── data_baru_tb_kepesertaan.csv  # data baru
|   └── tb_2021_kepesertaan.csv       # data training
│   └── tb_fkrtl.csv                  # Data training
├── model/
│   └── random_forest_model.pkl       # Model Random Forest yang telah dilatih
└── README.md                         # Dokumentasi proyek
```

## 📈 Hasil
- Model mampu memprediksi biaya tagih dengan akurasi tinggi menggunakan Random Forest
- Dapat membantu analisis biaya dan perencanaan anggaran di fasilitas kesehatan
