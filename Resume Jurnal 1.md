Nama : Muhammad Fairus Ramadhani  
NPM : 21081010090  
Kelas : Riset Informatik C

# 1. Pendahuluan

Makalah ini membahas pendekatan unsupervised learning untuk ekstraksi fitur visual melalui metode clustering. Dengan menggunakan metode yang disebut DeepCluster, makalah ini menyajikan pendekatan baru yang menggabungkan pembelajaran jaringan saraf convolutional (convnet) dengan algoritma clustering seperti k-means untuk meningkatkan pelatihan fitur visual dari dataset skala besar tanpa supervisi. Hasilnya menunjukkan kinerja yang lebih baik dibandingkan metode sebelumnya dalam benchmark visual transfer task seperti klasifikasi dan image retrieval.

# 2. Metode

Metode yang diusulkan dalam makalah ini menggunakan pendekatan clustering iteratif. Proses dimulai dengan ekstraksi fitur dari gambar menggunakan convnet, kemudian fitur tersebut dikelompokkan menggunakan algoritma k-means. Hasil dari pengelompokan ini digunakan sebagai label semu (pseudo-labels) untuk memperbarui bobot jaringan saraf. Pendekatan ini dilakukan secara end-to-end tanpa memerlukan label supervisi. Selain itu, metode ini juga menggunakan augmentasi data dan regularisasi selama pelatihan untuk meningkatkan kinerja.

# 3. Pembahasan

Pembahasan utama dalam makalah ini mencakup evaluasi metode DeepCluster terhadap dataset besar seperti ImageNet dan YFCC100M. Hasil eksperimen menunjukkan bahwa metode ini memberikan hasil yang signifikan dalam tugas-tugas transfer seperti klasifikasi dan deteksi objek. DeepCluster juga menunjukkan ketahanan terhadap perubahan arsitektur dan dataset. Misalnya, ketika menggunakan arsitektur jaringan yang lebih dalam seperti VGG-16, metode ini meningkatkan kinerja dibandingkan dengan AlexNet. DeepCluster juga bekerja dengan baik pada dataset yang tidak terstruktur, menunjukkan fleksibilitasnya dalam berbagai skenario.

# 4. Kesimpulan

DeepCluster menawarkan pendekatan efisien dan fleksibel untuk pembelajaran tanpa supervisi pada dataset gambar besar. Dengan memanfaatkan clustering untuk pelatihan fitur, metode ini mencapai kinerja yang melampaui metode pembelajaran tanpa supervisi lainnya. Selain itu, DeepCluster tidak memerlukan asumsi domain tertentu, menjadikannya kandidat yang baik untuk diterapkan pada berbagai jenis gambar dan modalitas visual yang tidak memiliki label anotasi.
