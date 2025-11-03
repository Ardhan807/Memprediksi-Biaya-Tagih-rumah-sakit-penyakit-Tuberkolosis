# Prediksi Biaya Tagih Fasilitas Kesehatan (Tuberkulosis) 🏥💰

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.2.2-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## 📊 Deskripsi Proyek
Proyek ini menggunakan **Random Forest Regression** untuk memprediksi **biaya tagih oleh fasilitas kesehatan (provider)** untuk pasien dengan penyakit **Tuberkulosis**, berdasarkan data **BPJS Kesehatan Tahun 2022**.  

Model ini berguna untuk:
- Analisis biaya kesehatan
- Perencanaan anggaran di fasilitas kesehatan
- Pemahaman pola klaim biaya pasien Tuberkulosis

---

## 📂 Data
- **Sumber:** BPJS Kesehatan Tahun 2022  
- **Jenis Data:** Klaim dan biaya layanan pasien Tuberkulosis  
- **Fitur Utama:**
  - Tanggal lahir peserta
  - Tanggal kunjungan dan pulang fasilitas kesehatan
  - Jenis layanan dan diagnosa
  - Fasilitas kesehatan (provider)
  - Biaya tagih  

> Data sudah dianonimkan sesuai kebijakan privasi.

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
   - Hyperparameter tuning (opsional)

4. **Evaluasi Model**
   - Metrics: RMSE, MAE, R² Score
   - Visualisasi prediksi vs nilai aktual  

Contoh visualisasi prediksi vs aktual (placeholder):

![Prediksi vs Aktual](docs/prediction_plot.png)

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
