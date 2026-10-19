# Analisis Karakteristik Aerodinamika dan Prediksi Tekanan Suara

Proyek Machine Learning menggunakan dataset **Airfoil Self-Noise** untuk menganalisis karakteristik aerodinamika dan memprediksi tekanan suara menggunakan K-Means Clustering dan Random Forest Regression.

## Dataset
- Jumlah data: 1.503 baris
- Fitur: Frequency, Angle of Attack, Chord Length, Free-stream Velocity, dan Suction-side Displacement Thickness
- Target: Scaled Sound Pressure

Sumber: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/291/airfoil+self+noise)

## Metode
- **EDA:** Eksplorasi distribusi data dan hubungan antarvariabel.
- **K-Means Clustering:** Mengelompokkan data berdasarkan karakteristik aerodinamika.
- **Random Forest Regression:** Memprediksi tekanan suara dan melakukan optimasi hyperparameter.
- **Evaluasi:** MAE, MSE, RMSE, dan R².
- **Feature Importance:** Mengidentifikasi fitur yang berpengaruh terhadap prediksi.

## Hasil
Random Forest Regression setelah optimasi memperoleh hasil pada data uji:

| Metrik | Nilai |
|---|---:|
| R² | 0,9377 |
| MAE | 1,2789 dB |
| MSE | 3,1207 |
| RMSE | 1,7666 dB |

K-Means menghasilkan dua cluster dengan Silhouette Score 0,3261. Hasil ini menunjukkan pemisahan cluster yang relatif lemah.

## Teknologi
Python, Jupyter Notebook, pandas, NumPy, Matplotlib, Seaborn, dan scikit-learn.

## Kesimpulan
Random Forest Regression memberikan performa prediksi yang baik pada data uji. Frequency dan Suction-side Displacement Thickness menjadi fitur yang menonjol dalam analisis kepentingan fitur, sedangkan K-Means digunakan untuk mengeksplorasi pola pengelompokan data.
