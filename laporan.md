# **Projek Pertama - Klasifikasi Penyakit Jantung**


---
Author : `David Mario Yohanes Samosir`

# CRISP - DM
## 1. Data Understanding
- Memprediksi apakah seseorang terjangkit penyakit jantung berdasarkan beberapa atribut kesehatan

## 2. Data Preparation
- Dataset: [Heart_disease](https://www.kaggle.com/datasets/dharanireddy/heart-disease)

- Fitur yang digunakan:
    1. age - Usia dalam tahun
    2. sex - (1 = male; 0 = female)
    3. cp - chest pain type
      - 0: Typical angina: nyeri dada terkait mengurangi suplai darah ke jantung
      - 1: Atypical angina: nyeri dada tidak berhubungan dengan jantung
      - 2: Non-anginal pain: biasanya kejang esofagus (tidak berhubungan dengan jantung)
      - 3: Asymptomatic: nyeri dada tidak menunjukkan tanda-tanda penyakit
    4. trestbps - mengistirahatkan tekanan darah (dalam mm Hg saat masuk ke rumah sakit)
      - di atas 130-140 biasanya memprihatinkan
    5. chol - serum cholestoral dalam mg/dl
      - serum = LDL + HDL + .2 * triglycerides
      - di atas 200 yang memprihatinkan
    6. fbs - (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
      - '>126' mg/dL signals diabetes
    7. restecg - resting electrocardiographic results
      - 0: Tidak ada yang perlu diperhatikan
      - 1: ST-T Wave abnormality
        - dapat berkisar dari gejala ringan hingga masalah parah
        - sinyal detak jantung yang tidak normal
      - 2: Possible or definite left ventricular hypertrophy
        - Ruang pompa utama jantung yang diperbesar
    8. thalach - denyut jantung maksimum tercapai
    9. exang - latihan diinduksi angina (1 = yes; 0 = no)
    10. oldpeak - Depresi ST yang disebabkan oleh olahraga relatif terhadap istirahat
      - melihat stres jantung saat berolahraga
      - jantung yang tidak sehat akan lebih stres
    11. slope - kemiringan segmen ST latihan puncak
      - 0: Upsloping: detak jantung yang lebih baik dengan olahraga (tidak biasa)
      - 1: Flatsloping: perubahan minimal (jantung sehat yang khas)
      - 2: Downslopins: tanda-tanda jantung yang tidak sehat
    12. ca - jumlah pembuluh darah utama (0-3) diwarnai oleh flourosopy
      - pembuluh berwarna berarti dokter dapat melihat darah yang melewatinya
      - semakin banyak gerakan darah semakin baik (tidak ada gumpalan)
    13. thal - hasil stres thalium
      - 1,3: normal
      - 6: fixed defect: dulu cacat tapi sekarang baik-baik saja
      - 7: reversable defect: tidak ada gerakan darah yang tepat saat berolahraga
    14. target - memiliki penyakit atau tidak (1=yes, 0=no) (= atribut yang diprediksi)

## 3. Data Wrangling
Langkah-langkah:

- Muat dataset dan pahami struktur data.
- Identifikasi dan tangani missing values jika ada.
- Lakukan encoding untuk variabel kategorikal jika diperlukan.
- Lakukan normalisasi atau standarisasi data untuk mempersiapkan fitur-fitur numerik.

## 4. Model Training
Langkah-langkah:

- Bagi dataset menjadi training set dan testing set.
- Pilih beberapa model klasifikasi yaitu Regression, Random Forest, atau SVM.
- Latih model menggunakan training set.

## 5. Model Testing
Langkah-langkah:

- Gunakan model yang telah dilatih untuk membuat prediksi menggunakan testing set.

## 6. Model Evaluation
Langkah-langkah:

- Evaluasi model menggunakan berbagai metrik seperti accuracy, precision, recall, dan F1-score.
- Analisis confusion matrix untuk memahami performa model lebih lanjut.
