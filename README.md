# Introduction to Machine Learning
Studi kasus sesi **Introduction to Machine Learning** - *Informatics Practitioner Lecture Series, Informatika Unib*.

**Tema:** deteksi dan atribusi penyebab deforestasi di Provinsi Bengkulu. Data **sintetis** (untuk pembelajaran).

**Tujuan:** Membangun dan mengevaluasi model klasifikasi (supervised learning) untuk memprediksi penyebab deforestasi.

## Hasil singkat
- Model terbaik: **RandomForest**, akurasi uji **0.86**, macro-F1 **0.835**
- Spatial CV (leave-kabupaten-out) macro-F1 0.830

| Model | CV macro-F1 (5-fold) |
|---|---|
| LogisticRegression | 0.821 +/- 0.009 |
| RandomForest | 0.835 +/- 0.011 |
| HistGradientBoosting | 0.827 +/- 0.003 |

## Struktur
```
src/generate_data.py   # data sintetis
src/features.py        # rekayasa fitur
src/train_model.py     # training, CV, evaluasi
reports/  models/
```

## Menjalankan
```bash
pip install -r requirements.txt
python -m src.generate_data
python -m src.train_model
```

## Laporan
Lihat [`docs/studi_kasus.md`](docs/studi_kasus.md).

## Repo lain dalam rangkaian studi kasus ini
- `01-data-analysis-and-ai`
- `02-hpc-parallel-processing`
- `03-gis-spatial-analysis`
- `05-hci-data-visualization`
- `06-deforestation-drivers-satellite-ai`
