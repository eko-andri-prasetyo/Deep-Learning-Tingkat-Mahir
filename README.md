# DLTM - Multivariate Multi-Horizon Time Series Forecasting (Bitcoin Close)

Folder ini berisi:
- Notebook: SyaikhEko_Submission_Akhir_DLTM.ipynb
- Model mandatory (akan terbuat saat notebook dijalankan):
  - model_baseline_LSTM.keras
  - model_seq2seq_LSTM.keras
- Model opsional (terbuat saat training selesai):
  - best_model_seq2seq_LSTM.keras
- requirements.txt
- Dataset lokal (opsional): Bitcoin3.csv

## Cara pakai (disarankan Colab)
1) Upload folder ini ke Google Drive atau upload file notebook ke Colab.
2) Jalankan notebook dari atas sampai bawah (tanpa skip).
3) Pastikan cell terakhir menampilkan:
   - Tabel perbandingan aktual vs prediksi 24 step
   - Plot garis aktual vs prediksi
   - Test MAE (scaled)
4) Pastikan file .keras tersimpan di folder kerja.
5) ZIP ulang folder (berisi .ipynb + .keras + requirements.txt) untuk submission.

Catatan:
- Notebook sudah memproteksi dari data leakage (scaler fit di train saja).
- Target prediksi: Close (multi-step 24).
- Input minimal 3 fitur (default 6 fitur), bisa ditambah rolling feature.
