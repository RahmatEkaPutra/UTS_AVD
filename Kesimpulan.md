
## **Kesimpulan**

Berdasarkan analisis yang telah dilakukan terhadap dataset Pokémon, diperoleh beberapa temuan penting sebagai berikut:

1. **Pra-pemrosesan Data**  
   Dataset Pokémon berhasil dibersihkan dari nilai-nilai yang hilang dan kolom kategori telah diubah menjadi format numerik menggunakan `LabelEncoder`. Selain itu, dilakukan standarisasi pada fitur numerik agar seluruh data berada dalam skala yang sebanding.

2. **Pemodelan Supervised Learning**  
   Lima algoritma supervised learning telah digunakan untuk memprediksi nilai **`Total`** (sebagai representasi kekuatan/power total Pokémon), yaitu:
   - **Linear Regression**
   - **Naive Bayes**
   - **Decision Tree Regressor**
   - **Support Vector Regressor (SVR)**
   - **K-Nearest Neighbors Regressor (KNN)**

3. **Evaluasi Model**  
   Model-model diuji menggunakan metrik seperti **Mean Squared Error (MSE)** dan **R² Score**. Hasil menunjukkan bahwa:
   - **Linear Regression** memberikan hasil yang sangat akurat, dengan nilai R² mendekati 1.
   - **Decision Tree Regressor** dan **SVR** juga menunjukkan performa yang baik.
   - **KNN Regressor** memberikan hasil yang kompetitif, tetapi performanya sangat dipengaruhi oleh jumlah tetangga (nilai k) dan skala fitur.
   - **Naive Bayes** kurang cocok untuk tugas regresi karena model ini secara alami lebih tepat digunakan pada tugas klasifikasi.

4. **Kesimpulan Akhir**  
   Untuk prediksi nilai kekuatan total Pokémon, model regresi seperti **Linear Regression** dan **Decision Tree Regressor** terbukti lebih akurat dan stabil. Oleh karena itu, model regresi merupakan pendekatan yang sesuai dalam kasus ini.
