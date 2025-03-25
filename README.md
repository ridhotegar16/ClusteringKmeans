# ClusteringKmeans
# README - Clustering dengan K-Means

## Deskripsi Proyek
PT 456 adalah platform yang menyediakan penjualan voucher digital dan gift card dalam satu platform. Saat ini PT 456 mulai beralih ke bisnis digital. PT 456 menyediakan voucher, gift card, reward untuk memberikan kemudahan kepada pelanggan dalam berbelanja.

Perusahaan ingin mengetahui analisis untuk mendapatkan insight terkait dengan segmentasi customer pada aplikasi yang telah mereka kembangkan. Analisis ini diharapkan dapat membantu PT 456 dalam mengembangkan strategi penjualan produk bagi platform mereka.

Variabel yang ada pada data antara lain, yaitu:
* Nomor transaksi = Nomor transaksi yang dibuat
* Status transaksi = Status transaksi yang dipilih (Reguler atau Promo)
* Order At = Timestamp masuknya transaksi
* Date = Tanggal transaksi dibuat
* Merchant ID = ID Merchant yang dipilih oleh cust pada transaksi
* Kategori = Kategori merchant yang dipilih oleh cust pada transaksi
* SKU Product Name = Nama product
* Nomor Customer = ID/Nomor customer yang membuat transaksi
* Register Date= Tanggal registrasi akun oleh customer
* Amount = Harga barang
* Selling price = Harga jual
* Quantity = Total barang yang dibeli
* Total Amount = Total harga barang
* Total Selling Price = Total harga jual

## Fitur Utama
- **Preprocessing Data**: Membersihkan dan menyiapkan data sebelum clustering.
- **Implementasi K-Means**: Menggunakan algoritma K-Means untuk melakukan segmentasi data.
- **Evaluasi Cluster**: Menggunakan metode evaluasi seperti Elbow Method dan Silhouette Score.
- **Visualisasi Hasil**: Menampilkan hasil clustering dalam bentuk grafik yang mudah dipahami.

## Teknologi yang Digunakan
- Python
- Pandas untuk manipulasi data
- Scikit-learn untuk implementasi K-Means
- Matplotlib dan Seaborn untuk visualisasi data

## Kesimpulan dan Insight
Clustering dengan K-Means dapat digunakan untuk mengidentifikasi pola tersembunyi dalam data dan membantu dalam pengambilan keputusan berbasis data. Dari hasil clustering, kita dapat memahami bagaimana data tersegmentasi dan menemukan kelompok dengan karakteristik yang mirip. 

Beberapa insight yang diperoleh dari proyek ini:
- **Identifikasi Segmen**: Data dapat dibagi menjadi beberapa kelompok dengan karakteristik yang berbeda.
- **Pola dalam Data**: Clustering membantu dalam mengenali pola yang sebelumnya tidak terlihat.
- **Optimasi Jumlah Cluster**: Penggunaan metode seperti Elbow Method membantu menentukan jumlah cluster yang optimal untuk analisis lebih lanjut.

* Segment 0 : Memberikan promo pada pembelian  dengan quantity > 75.
Ex: untuk pembelian voucher lebih dari 75 dalam satu kali transaksi akan mendapatkan diskon voucher sekitar 5% - 10%.


* Segment 1 : Memberikan promo berupa bundling pada setiap pembelian voucher berkategori App & Lifestyle.
Ex: Setiap customer pada segment 1 yang membeli voucher berkategori App & Lifestyle akan mendapatkan tambahan promo bundling ketika membeli satu voucher atau lebih pada kategori lainnya.

* Segment 2 : Menyajikan jenis jenis voucher berkategori luxury untuk meningkatkan spending dari segment 2.
Ex: Merekomendasikan voucher luxury pada halaman utama customer  jika sesuai dengan algoritma pembelian customer pada segment 2.

* Segment 3 : Menyediakan lebih banyak voucher berkategori promo dengan selling price bersyarat.

**Saran keseluruhan:**

* Menambah varians merchant untuk kategori-kategori yang masih sedikit jumlah penjualannya seperti Gold & Investment, Activity & Entertainment, Hotel & Travel, dan Lain-lain.

* Menambahkan Sistem PayLater karena masih banyak yang memiliki monetary rendah untuk meningkatkan penjualan.

* Ketika di akhir transaksi mengadakan survei untuk user terkait perkembangan aplikasi.

* Mengadakan promosi secara digital dan berkolaborasi dengan publik figur agar demand dari aplikasi meningkat.


