# Analisis metode dan metodologi

### **1. Jurnal Pertama**:

**Judul**: _An Anomaly Detection Approach Based on Isolation Forest Algorithm for Streaming Data using Sliding Window_

- **Penggunaan Istilah Metode**:
  Dalam jurnal ini, istilah yang digunakan adalah "Anomaly Detection Approach," yang mengacu pada **metode** deteksi anomali. Penggunaan kata "metode" di sini menunjukkan bahwa jurnal ini berfokus pada langkah-langkah teknis atau pendekatan spesifik yang digunakan untuk mendeteksi anomali dalam data streaming. Pendekatannya berdasarkan algoritma Isolation Forest, yang merupakan sebuah algoritma yang telah dikenal dalam _machine learning_ dan disesuaikan untuk skenario data streaming dengan tambahan konsep _sliding window_.

- **Apa Itu Metode?**:
  Metode mengacu pada teknik, prosedur, atau alat yang digunakan untuk mencapai suatu tujuan tertentu. Dalam hal ini, _metode_ merujuk pada algoritma Isolation Forest dan bagaimana cara penerapannya dalam mendeteksi anomali pada data streaming. Pendekatannya sangat praktis dan langsung ke penerapan teknis.

### **2. Jurnal Kedua**:

**Judul**: _Time Series Contextual Anomaly Detection for Detecting Stock Market Manipulation_

- **Penggunaan Istilah Metodologi**:
  Dalam jurnal ini, tidak secara eksplisit menyebutkan kata "metodologi" dalam judul, tetapi penggunaan konteks "Contextual Anomaly Detection" merujuk pada **metodologi** yang lebih komprehensif dalam analisis anomali. Istilah metodologi mencakup lebih dari sekadar metode spesifik, karena menyiratkan adanya kerangka kerja atau pendekatan menyeluruh untuk memahami, menganalisis, dan menyelesaikan masalah tertentu. Dalam kasus ini, deteksi anomali tidak hanya dilakukan dengan satu metode, tetapi juga mencakup pengintegrasian elemen lain, seperti analisis sentimen dari media sosial (Twitter), yang mengindikasikan pendekatan multi-aspek terhadap masalah manipulasi pasar saham.

- **Apa Itu Metodologi?**:
  Metodologi merujuk pada keseluruhan pendekatan, teori, dan prinsip yang digunakan untuk mendefinisikan dan menjalankan penelitian atau eksperimen. Ini mencakup lebih dari sekadar langkah-langkah teknis atau alat yang digunakan, tetapi juga cara pandang yang lebih luas terhadap masalah, alasan pemilihan metode tertentu, serta bagaimana metode tersebut diimplementasikan. Dalam hal ini, metodologi mencakup CAD, analisis sentimen, dan pendekatan berbasis _time series_ dalam mendeteksi anomali.

### **Perbedaan Utama Antara Metode dan Metodologi dalam Kedua Judul**:

1. **Fokus pada Metode di Jurnal Pertama**:

   - Di jurnal pertama, fokusnya adalah pada **metode spesifik** (algoritma Isolation Forest) yang digunakan untuk mendeteksi anomali pada data streaming. Judulnya langsung merujuk pada teknik atau alat tertentu yang digunakan untuk mencapai tujuan, yaitu mendeteksi anomali. Metode ini lebih bersifat teknis dan menyarankan langkah-langkah praktis.

2. **Pendekatan Metodologi di Jurnal Kedua**:
   - Di jurnal kedua, meskipun judulnya tidak secara eksplisit menyebut "metodologi," pendekatannya lebih bersifat metodologis karena menggabungkan beberapa **pendekatan** yang mencakup analisis kontekstual _time series_, CAD, serta analisis sentimen untuk meningkatkan deteksi anomali dalam manipulasi pasar saham. Hal ini mencerminkan penerapan yang lebih luas dan beragam, serta menunjukkan kerangka berpikir yang komprehensif untuk memecahkan masalah kompleks.

### Kesimpulan:

- **Jurnal pertama** menggunakan istilah metode karena fokus utamanya pada **alat atau teknik tertentu** (Isolation Forest) yang diterapkan secara praktis untuk masalah pendeteksian anomali dalam data streaming.
- **Jurnal kedua**, meskipun tidak menyebutkan secara langsung "metodologi," mengindikasikan pendekatan yang lebih metodologis karena mencakup **pendekatan komprehensif** yang melibatkan berbagai aspek dan metode dalam mendeteksi anomali pada _time series_, termasuk analisis sentimen, yang melibatkan konsep-konsep lebih luas dibanding hanya satu metode.

# Review 1

**Judul**:  
_Anomaly Detection Approach Based on Isolation Forest Algorithm for Streaming Data using Sliding Window_

**Penulis**:

- Zhiguo Ding (Shanghai University, Zhejiang Normal University)
- Minrui Fei (Shanghai University)

**Abstrak**:  
Pendeteksian perilaku anomali menjadi semakin penting dalam berbagai aplikasi, seperti keamanan komputer dan jaringan sensor. Data streaming yang terus berubah dan memiliki volume besar menjadi tantangan dalam pendeteksian anomali. Dalam penelitian ini, sebuah kerangka deteksi anomali berbasis algoritma _Isolation Forest_ diadaptasi untuk data streaming, yang diberi nama _iForestASD_. Algoritma ini menggunakan konsep _sliding windows_ untuk menangani fenomena _concept drift_ dalam data yang terus berkembang. Uji coba dilakukan pada empat dataset dari UCI Repository, menunjukkan bahwa algoritma ini efektif dalam mendeteksi anomali dalam data streaming.

**Kata kunci**:  
Deteksi Anomali, Data Streaming, Concept Drift, Isolation Forest, Sliding Window

### Pendahuluan:

- Data streaming adalah bentuk data yang mengalir terus menerus dan sering digunakan dalam aplikasi dunia nyata seperti pemantauan keamanan jaringan, manajemen lalu lintas, dan transaksi industri ritel.
- Tantangan utama dalam pendeteksian anomali pada data streaming adalah volume data yang besar, perubahan konsep yang sering, dan kesulitan dalam pelatihan model karena ketidakseimbangan data.
- Algoritma _Isolation Forest_ (iForest) dipilih untuk penelitian ini karena kemampuannya yang efisien dalam mendeteksi anomali pada dataset besar dengan kompleksitas perhitungan yang rendah.

### Kontribusi Utama:

1. Mengusulkan kerangka pendeteksian anomali untuk data streaming.
2. Mengadaptasi algoritma iForest untuk menangani data streaming.
3. Melakukan eksperimen pada empat dataset dunia nyata untuk memvalidasi efektivitas algoritma.

### Kerangka Pendeteksian Anomali:

- Data streaming dibagi menjadi blok data dengan ukuran jendela tetap (_sliding window_).
- Detektor anomali dibangun menggunakan algoritma iForest dan memperbarui model ketika terjadi _concept drift_.
- Ketika _concept drift_ terdeteksi, model dilatih ulang menggunakan data dari jendela terbaru.

### Algoritma iForestASD:

- _iForest_ terdiri dari sejumlah pohon isolasi (_iTree_) yang dibangun melalui pengambilan sampel acak dari dataset. Anomali adalah titik data yang lebih cepat terisolasi dibandingkan dengan data normal.
- Algoritma ini menghitung skor anomali berdasarkan rata-rata kedalaman _iTree_ untuk setiap instance.

### Hasil Eksperimen:

- Dataset yang digunakan dalam eksperimen berasal dari UCI Repository, yaitu Http, Smtp, ForestCover, dan Shuttle.
- Algoritma iForestASD menunjukkan kinerja yang baik dalam mendeteksi anomali pada data streaming, dengan AUC meningkat seiring dengan bertambahnya ukuran jendela sliding.

### Kesimpulan dan Pekerjaan Masa Depan:

- Algoritma iForestASD efektif dalam mendeteksi anomali pada data streaming, namun ada beberapa tantangan seperti penentuan ukuran jendela dan ambang batas deteksi anomali yang perlu diperbaiki.
- Penelitian di masa depan akan fokus pada pengembangan metode untuk mendeteksi _concept drift_ secara otomatis dan meningkatkan kinerja algoritma melalui pembaruan model yang lebih adaptif.

# Review 2

Berikut adalah resume berdasarkan file yang Anda berikan:

---

**Judul**:  
_Time Series Contextual Anomaly Detection for Detecting Stock Market Manipulation_

**Penulis**:

- Seyed Koosha Golmohammadi

**Institusi**:

- Department of Computing Science, University of Alberta

**Tahun**:  
2016

**Abstrak**:  
Pendeteksian anomali dalam _time series_ merupakan masalah penting dalam _data mining_ yang memiliki penerapan di berbagai bidang, termasuk deteksi manipulasi pasar saham. Dalam disertasi ini, penulis mengusulkan metode pendeteksian anomali kontekstual berbasis prediksi (_Contextual Anomaly Detection_, CAD) untuk _time series_ yang tidak bisa dijelaskan melalui model deterministik. Penulis juga mengeksplorasi bagaimana teknik _big data_, seperti analisis sentimen dari Twitter, dapat membantu meningkatkan kinerja deteksi anomali dengan mengurangi positif palsu. Metode ini diterapkan pada data pasar saham untuk mendeteksi manipulasi dengan lebih efektif.

**Kata kunci**:  
Anomaly Detection, Time Series, Stock Market Manipulation, Contextual Anomaly Detection, Big Data, Sentiment Analysis

### Pendahuluan:

- Deteksi anomali merupakan tugas penting dalam banyak bidang, seperti deteksi intrusi pada jaringan komputer, deteksi anomali pada data kesehatan, serta deteksi penipuan di pasar saham.
- Teknik pendeteksian anomali konvensional sering mengabaikan aspek temporal dari data _time series_, sehingga kurang efektif dalam aplikasi yang membutuhkan analisis temporal seperti manipulasi pasar saham.

### Masalah Utama:

- Pendekatan konvensional yang hanya mencari objek berbeda dari normal tanpa memperhatikan konteks temporal tidak efektif dalam mendeteksi anomali di pasar saham.
- Manipulasi pasar saham mempengaruhi kepercayaan publik dan memerlukan deteksi anomali yang lebih baik untuk mencegah kerugian finansial.

### Metodologi:

- Penulis mengusulkan metode CAD yang berbasis prediksi untuk mendeteksi anomali dalam _time series_. CAD memprediksi perilaku normal saham berdasarkan korelasi data historis, dan mengidentifikasi penyimpangan dari perilaku tersebut sebagai anomali.
- Sentimen analisis Twitter digunakan untuk membantu mengurangi jumlah positif palsu dengan mengaitkan data sentimen dari tweet terhadap saham tertentu dengan deteksi anomali yang terjadi di pasar saham.

### Kontribusi Utama:

1. Menyajikan metode deteksi anomali kontekstual yang memanfaatkan korelasi _time series_ untuk mendeteksi anomali di pasar saham.
2. Menggabungkan analisis sentimen dari data Twitter untuk mengeliminasi positif palsu dalam deteksi anomali saham.
3. Studi kasus yang menunjukkan peningkatan kinerja pendeteksian anomali pada data pasar saham dengan CAD dibandingkan dengan metode _kNN_ dan _random walk_.

### Hasil dan Diskusi:

- Eksperimen menunjukkan bahwa metode CAD yang diusulkan meningkatkan _recall_ dari 7% menjadi 33% tanpa mengorbankan presisi.
- Penggunaan analisis sentimen berhasil mengidentifikasi 28% dari positif palsu, sehingga meningkatkan keakuratan deteksi anomali.

### Kesimpulan:

- CAD berbasis prediksi yang diusulkan lebih efektif dalam mendeteksi manipulasi pasar saham dibandingkan dengan metode lain. Penggunaan data besar, seperti analisis sentimen, dapat lebih meningkatkan akurasi dan mengurangi positif palsu.
- Studi lebih lanjut perlu dilakukan untuk mengeksplorasi bagaimana menggabungkan lebih banyak sumber data tidak terstruktur, seperti laporan keuangan dan berita, untuk meningkatkan deteksi anomali.
