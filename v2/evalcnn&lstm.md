Untuk artikel **"Handwritten Text Recognition using Deep Learning"** yang ditulis oleh Batuhan Balci, Dan Saadati, dan Dan Shiferaw, berikut adalah beberapa *metrics* yang umumnya digunakan dalam penelitian mengenai pengenalan teks tulisan tangan menggunakan pembelajaran mendalam (*deep learning*). Meskipun saya tidak memiliki akses langsung ke isi artikel tersebut, beberapa metrik yang biasa digunakan dalam topik ini adalah sebagai berikut:

### 1. **Accuracy (Akurasi)**
   - **Deskripsi:** Metrik ini mengukur persentase prediksi yang benar dari total prediksi yang dilakukan oleh model. Untuk HTR, akurasi biasanya dihitung berdasarkan jumlah karakter atau kata yang benar dibandingkan dengan jumlah total karakter atau kata yang ada dalam dataset pengujian.
   
   - **Formula:**  
    ![image](https://github.com/user-attachments/assets/5a630b81-eeef-4ee5-959e-326445186c23)


### 2. **Character Error Rate (CER)**
   - **Deskripsi:** CER adalah metrik yang mengukur kesalahan pada tingkat karakter. Ini menghitung persentase kesalahan karakter antara prediksi model dan teks yang benar. CER sering digunakan dalam pengenalan teks tulisan tangan karena lebih sensitif terhadap kesalahan karakter individual.
   
   - **Formula:**  
    ![image](https://github.com/user-attachments/assets/11eeef55-837a-4a40-8f96-f31185becac8)

     Di mana "Salah Karakter" adalah jumlah karakter yang salah dalam prediksi dan "Total Karakter yang Benar" adalah jumlah karakter dalam teks yang benar.

### 3. **Word Error Rate (WER)**
   - **Deskripsi:** WER adalah metrik yang menghitung persentase kesalahan pada tingkat kata. WER dihitung dengan mengukur perbedaan antara teks yang diprediksi dan teks yang benar dengan mempertimbangkan insersi, penghapusan, dan substitusi kata.
   
   - **Formula:**  
    ![image](https://github.com/user-attachments/assets/5d27cfe2-ced8-4faf-8d44-0951db38357f)

### 4. **Precision, Recall, dan F1-Score**
   - **Deskripsi:** Precision, recall, dan F1-score sering digunakan untuk mengukur kinerja dalam pengenalan teks berdasarkan kesalahan spesifik, meskipun lebih umum digunakan dalam masalah klasifikasi. Precision mengukur proporsi prediksi yang benar dari semua prediksi yang dilakukan, sedangkan recall mengukur seberapa banyak prediksi yang benar berhasil ditemukan. F1-score adalah rata-rata harmonis dari precision dan recall.
   
  ![image](https://github.com/user-attachments/assets/1ad1c030-05e7-423d-9f3b-d2e376a981ea)


### 5. **Levenshtein Distance (Edit Distance)**
   - **Deskripsi:** Levenshtein distance, atau edit distance, mengukur perbedaan antara dua string (misalnya teks yang diprediksi dan teks yang benar) berdasarkan jumlah operasi edit yang diperlukan untuk mengubah satu string menjadi string lainnya. Ini bisa menjadi karakteristik yang berguna untuk menghitung kesalahan dalam teks tulisan tangan.

### 6. **Normalized Edit Distance**
   - **Deskripsi:** Versi ternormalisasi dari Levenshtein distance yang membagi edit distance dengan panjang teks, memungkinkan perbandingan antara teks dengan panjang yang berbeda.

### 7. **Top-k Accuracy**
   - **Deskripsi:** Top-k accuracy mengukur apakah kata atau karakter yang benar ada dalam k prediksi teratas yang dihasilkan oleh model. Ini memberi gambaran tentang seberapa sering model memprediksi hasil yang benar dalam beberapa opsi teratas.

   ![image](https://github.com/user-attachments/assets/d338f4e6-abc4-462e-8b5d-6c3f87b0403b)


---

Metrik-metrik di atas sangat relevan untuk menilai kinerja model dalam pengenalan teks tulisan tangan, terutama yang menggunakan metode *deep learning*. Untuk artikel tersebut, metrik yang lebih spesifik mungkin akan disebutkan dalam bagian eksperimen atau hasil dari artikel.
