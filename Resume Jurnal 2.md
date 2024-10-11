Nama : Muhammad Fairus Ramadhani  
NPM : 21081010090  
Kelas : Riset Informatik C

# 1. Pendahuluan

Dalam dunia keamanan komputer, serangan terhadap jaringan seperti DoS, DDoS, worm, dan spyware terus berkembang, sementara teknik deteksi juga semakin canggih. Makalah ini fokus pada pengembangan kerangka kerja pembelajaran mesin untuk deteksi anomali jaringan. Tujuannya adalah untuk mendeteksi serangan yang baru muncul dengan menggabungkan algoritma genetika (GA) untuk pemilihan fitur dan Support Vector Machine (SVM) untuk klasifikasi paket jaringan. Makalah ini membahas kelemahan dari sistem deteksi intrusi berbasis tanda tangan (NIDS) dan mengusulkan pendekatan baru yang lebih efektif dan otonom dalam deteksi anomali jaringan.

# 2. Metode

Kerangka kerja yang diusulkan dalam makalah ini menggunakan SVM yang dimodifikasi dan algoritma genetika (GA) sebagai langkah awal untuk seleksi fitur. Komponen utama dari framework ini adalah:

Seleksi fitur menggunakan GA: Memilih field paket yang relevan untuk analisis lebih lanjut.
Preprocessing data: Paket yang difilter kemudian diproses untuk mempersiapkan input ke dalam framework SVM.
Pembelajaran menggunakan SVM: Dua metode digunakan—SVM soft margin (supervised learning) dan one-class SVM (unsupervised learning). Pendekatan SVM yang diperbarui ini memanfaatkan keunggulan dari kedua metode untuk meningkatkan kinerja dalam deteksi anomali.
Pengujian dan pembandingan: Framework diuji secara eksperimen dan dibandingkan dengan sistem deteksi intrusi nyata seperti Snort dan Bro.

# 3. Pembahasan

Framework yang diusulkan menggunakan GA untuk memilih field yang paling relevan dari paket TCP/IP, yang kemudian digunakan untuk meningkatkan akurasi dan efisiensi deteksi. Proses preprocessing data bertujuan untuk mempersiapkan data paket yang difilter agar sesuai dengan input pembelajaran SVM. Dengan menggunakan dua pendekatan SVM, framework ini memungkinkan deteksi anomali yang lebih baik dengan kombinasi pembelajaran terawasi dan tidak terawasi. Hasil eksperimen menunjukkan bahwa framework yang diusulkan mengungguli sistem deteksi intrusi berbasis tanda tangan seperti Snort dalam hal kemampuan mendeteksi serangan baru. Selain itu, penggunaan GA untuk seleksi fitur mengurangi waktu pemrosesan sekaligus meningkatkan tingkat deteksi.

# 4. Kesimpulan

Pendekatan yang diusulkan dalam makalah ini menggunakan kombinasi SVM terawasi dan tidak terawasi untuk memberikan solusi yang efektif dalam mendeteksi serangan baru di jaringan. Dengan menggunakan algoritma genetika untuk seleksi fitur, kerangka ini memberikan deteksi yang lebih baik dengan tingkat false-positive yang rendah dibandingkan dengan sistem berbasis tanda tangan. Framework ini telah terbukti unggul dalam eksperimen menggunakan dataset DARPA dan juga menunjukkan kinerja yang menjanjikan ketika dibandingkan dengan sistem deteksi intrusi nyata seperti Snort. Penelitian lebih lanjut diperlukan untuk membuat profil data normal yang lebih baik agar framework ini lebih efektif dalam lingkungan dunia nyata.
