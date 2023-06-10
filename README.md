# Demand-Forecasting

Proyek ini akan membahas tentang bagaimana melakukan peramalan atau prediksi terhadap permintaan jumlah produk pada perusahaan menggunakan analisis time series. Proyek ini akan mencakup pengumpulan data, analisis data, pemilihan model terbaik, dan prediksi untuk memperkirakan jumlah permintaan produk pada perusahaan dalam jangka waktu tertentu. Dalam proyek ini, teknik time series analysis akan digunakan untuk mengevaluasi data historis dan membuat prediksi terhadap permintaan di masa depan untuk membantu perusahaan untuk mempersiapkan stok produk yang diperlukan secara lebih efektif.

## Objektif:

1. Mengembangkan model yang dapat memprediksi dengan akurat nilai penjualan produk tertentu di masa depan berdasarkan data historis.
2. Proyek ini juga bertujuan untuk memperkenalkan teknik dan konsep dasar dalam analisis time series, khususnya dalam pembuatan model forecasting dengan menggunakan metode-metode seperti ARIMA, SARIMA, dan Holt-Winters.

## Deployment Link
[HuggingFace](https://huggingface.co/spaces/bagushakim-id/demand-forecas)

## Tools and Library
- Pyhton
- Pandas
- Seaborn
- Matplotlib
- Statsmodel
- Scikit-learn

## Conclusion
1. Based on EDA

  - Terdapat 2309 unique value/product yang berbeda pada kolom "product_item" di dalam dataset dengan terdapat beberapa product item yang memiliki jumlah maksimum sebanyak 67 item dan beberapa product item yang memiliki jumlah paling sedikit sebanyak 1 item.
Berdasarkan observasi awal, dapat diketahui bahwa proses yang diamati tidak stasioner dan sulit untuk menentukan adanya seasonality. Namun, setelah dilakukan decomposing, dapat dipastikan bahwa data yang kita temui merupakan data seasonality.

2. Based on Model Evaluation

  - Pada model Holt Winters menghasilkan MAE sebesar 642372.03134607994 pada data train dan 658142.587849 pada data test. Dengan nilai MAE Train yang lebih rendah dari model-model SARIMA dan MAE Test yang juga relatif rendah.

  - Kelebihan dari model Holt Winters adalah mampu menangani data time series yang memiliki musimanitas dan tren secara bersamaan. Selain itu, model ini dapat menghasilkan hasil prediksi yang akurat dalam jangka waktu yang cukup lama.

Namun, kelemahan dari model Holt Winters adalah model ini kurang fleksibel dalam menangani perubahan yang tiba-tiba pada data, seperti perubahan kebijakan atau situasi yang tidak terduga lainnya. Selain itu, model ini juga memerlukan banyak waktu dan komputasi yang tinggi untuk menghasilkan hasil prediksi pada jangka waktu yang panjang.
