# capstoneproject3
## Hotel Booking Demand

**Context**  
Sebuah hotel merekrut Data Scientist yang mempunyai kemampuan dibidang Machine Learning untuk memprediksi apakah seorang customer akan membatalkan booking-an hotel atau tidak. Customer melakukan booking di hotel mereka, akan tetapi hotel sering mengalami kerugian karena customer yang membatalkan pemesanan.
Target :
- 0 : Tidak akan cancel
- 1 : Cancel

**Problem Statement :**

Bagaimana kita dapat memprediksi dan meminimalkan pembatalan oleh customer sehingga dapat mengurangi kerugian dari customer membatalkan kamar.

**Goals :**

Maka berdasarkan permasalahan tersebut, pihak hotel ingin memiliki kemampuan untuk memprediksi kemungkinan calon customer akan melakukan cancel booking pada hotel tersebut atau tidak, sehingga dapat memfokuskan pemberian kamar pada calon customer yang tidak akan men-cancel booking-an kamar mereka.

**Analytic Approach :**

Langkah pertama dalam penyelesaian permasalahan ini adalah melakukan analisis data untuk mengidentifikasi pola-pola yang memisahkan antara pengunjung yang berhasil menginap di hotel dengan yang customer yang memutuskan untuk membatalkan menginap. Setelahnya, kita akan mengembangkan sebuah model klasifikasi yang dapat memberikan prediksi terhadap karakteristik pengunjung, membantu hotel dalam mengantisipasi apakah pengunjung tersebut kemungkinan besar akan menginap atau membatalkan booking-an.

**Metric Evaluation**

1. True Positif: Kita memprediksi customer akan me-cancel dan sebenarnya customer tersebut benar me-cancel
2. False Positif: Kita memprediksi customer akan me-cancel tapi ternyata customer tersebut tidak me-cancel
3. True Negatif: Kita memprediksi customer tidak akan membatalkan booking dan sebenarnya customer benar tidak membatalkan booking
4. False Negatif: Kita memprediksi customer tidak akan membatalkan booking tapi ternyata customer membatalkan booking 

Pada model ini kita akan memprioritaskan untuk meminimalisir customer yang aktualnya cancel namun diprediksi tidak cancel (False Negative), maka dari itu kita akan memaksimalkan score recall pada model.
