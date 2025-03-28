# **Machine Learning for Beverage Sales: Clustering & Classification**

Repositori ini berisi proyek **Machine Learning untuk analisis penjualan minuman (Beverage Sales)**. Proyek ini mencakup dua bagian utama:

1. **Clustering** - Mengelompokkan pelanggan berdasarkan pola pembelian mereka menggunakan metode unsupervised learning.
2. **Classification** - Memprediksi kategori pelanggan berdasarkan fitur transaksi menggunakan supervised learning.

## **📊 Clustering Analysis**

- **Metode yang digunakan:** K-Means Clustering
- **Tujuan:** Mengelompokkan pelanggan berdasarkan transaksi untuk memahami pola pembelian mereka.
- **Hasil utama:**
  - Terbentuk **7 cluster** dengan karakteristik yang berbeda.
  - **Cluster 0:** Cluster ini terdiri dari pelanggan dengan harga produk rendah dan jumlah pembelian yang kecil. Mereka mungkin adalah pelanggan yang melakukan pembelian eceran atau hanya mencoba produk dalam jumlah kecil.
  - **Cluster 1:** Pelanggan dalam cluster ini membeli dalam jumlah lebih besar dibandingkan Cluster 0, namun masih dengan harga produk yang terjangkau. Mereka mungkin adalah pelanggan bisnis skala kecil yang membeli dalam jumlah sedang.
  - **Cluster 2:** Cluster ini mencakup pelanggan yang membeli produk dengan harga lebih mahal dan dalam jumlah besar. Mereka kemungkinan besar merupakan pembeli korporat atau distributor yang membeli untuk dijual kembali.
  - **Cluster 3:** Ini adalah cluster pelanggan dengan daya beli tinggi yang membeli produk premium dalam jumlah besar. Mereka bisa jadi pelanggan bisnis besar atau pelanggan loyal yang memiliki kebutuhan besar untuk produk tertentu.
  - **Cluster 4:** Pelanggan dalam cluster ini membeli produk dengan harga tinggi tetapi dalam jumlah kecil. Mereka mungkin adalah pelanggan ritel yang mencari produk premium dalam jumlah terbatas.
  - **Cluster 5:** Cluster ini mencerminkan pelanggan yang membeli produk murah dalam jumlah besar. Ini bisa jadi pelanggan bisnis yang ingin mendapatkan keuntungan dari diskon volume atau toko yang mengisi ulang stok
  - **Cluster 6:** Pelanggan ini membeli produk dengan harga sangat tinggi tetapi dalam jumlah kecil. Mereka bisa jadi pelanggan eksklusif atau niche market yang hanya tertarik pada produk tertentu.

### **Strategi Bisnis**
### **1. Loyalty Program untuk Cluster 3 & 2**
📌 Berikan insentif seperti diskon khusus atau program membership untuk mempertahankan pelanggan bernilai tinggi.

### **2. Paket Grosir untuk Cluster 5 & 1**
📌 Tawarkan paket hemat atau harga spesial untuk pembelian dalam jumlah besar agar mereka semakin loyal.

### **3. Eksklusivitas untuk Cluster 6 & 4**
📌 Berikan layanan premium, produk eksklusif, atau pengalaman belanja VIP untuk menarik pelanggan kelas atas.

### **4. Promosi untuk Cluster 0**
📌 Berikan promo diskon atau bundling produk agar mereka lebih sering berbelanja dan meningkatkan daya beli.


## **Classification Model**

- **Model yang digunakan:** Random Forest & Support Vector Mechine(SVM)
- **Tujuan:** prediksi jenis pelanggan ke dalam kategori tertentu berdasarkan fitur transaksi yang dilakukannya.

### **Evaluasi Model Sebelum dan Setelah Hyperparameter Tuning**

| **Metrik**       | **Sebelum Tuning** | **Setelah Tuning** |
|------------------|------------------|------------------|
| **Accuracy**     | 0.9983              | 0.9985              |
| **Precision** | 0.9977       |  0.9985       |
| **Recall**    | 0.9950       |  0.9985       |
| **F1-Score**  | 0.9963       | 0.9985       |

🔹 **Kesimpulan:**

#### Kesimpulan
- **Random Forest memiliki performa yang sangat baik**, dengan akurasi yang sangat tinggi hampir 100%.
- **SVM memiliki performa yang mirip Random Forest**, tetapi accuracy masih sedikit dibawah **Random Forest**.
