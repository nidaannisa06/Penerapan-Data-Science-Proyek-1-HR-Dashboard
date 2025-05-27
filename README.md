# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding

Jaya Jaya Maju merupakan salah satu perusahaan multinasional yang telah berdiri sejak tahun 2000 dan memiliki lebih dari 1000 karyawan yang tersebar di seluruh penjuru negeri. Namun demikian, perusahaan Jaya Jaya Maju mengalami kesulitan dalam mengelola karyawan yang berimbas pada fenomena tingginya attrition rate karyawan (rasio jumlah karyawan yang keluar dengan total karyawan keseluruhan) hingga lebih dari 10%. Oleh sebab itu, diperlukan identifikasi terkait faktor penyebab tingginya attrition rate dan sebuah business dashboard untuk monitoring faktor penyebab permasalahan.

### Permasalahan Bisnis

Adapun permasalahan bisnis yang dialami oleh Perusahaan Jaya Jaya Maju adalah sebagai berikut:
1. Faktor-faktor apa saja yang paling berkontribusi terhadap keluarnya karyawan dari perusahaan?

2. Apakah machine learning dapat digunakan untuk memprediksi apakah seorang karyawan akan keluar dari perusahaan?
   
### Cakupan Proyek

Proyek ini mencakup seluruh tahapan proses data science, antara lain:
- Mengumpulkan dan mengolah data karyawan Jaya Jaya Maju
- Eksplorasi dan pemahaman data yang diberikan.
- Pra-pemrosesan data dan transformasi fitur.
- Pembuatan dan evaluasi model machine learning (Random Forest Classifier).
- Analisis feature importance dan korelasi.
- Pembuatan visualisasi data interaktif.
- Pengembangan business dashboard menggunakan Looker Studio.
- Memberikan rekomendasi berdasarkan hasil analisis data.

### Persiapan

Sumber data: [Data Karyawan Jaya Jaya Maju](https://github.com/dicodingacademy/dicoding_dataset/blob/main/employee/employee_data.csv)

Setup environment:

```python
pip install -r requirements.txt
```

## Business Dashboard

Bisnis dashboard yang dibuat menggunakan Looker Studio dirancang untuk memberikan visibilitas dan insight yang cepat kepaada Manajemen dan Departemen HR tentang faktor-faktor attriotion di Jaya Jaya Maju. Saat ini dashboard dapat diakses melalui [Employee Attrition Dasboard Jaya Jaya Maju](https://lookerstudio.google.com/reporting/5b531828-11a6-45d6-8dc6-421703777b92). Dashboard ini menampilkan Dashboard akan menampilkan fitur-fitur utama berikut:
- Ringkasan Tingkat Attrition: Menampilkan metrik utama seperti attrition rate, jumlah karyawan attrition, dan jumlah karyawan keseluruhan.
- Faktor Pendorong Attrition: Grafik yang menunjukkan fitur yang memengaruhi attrition (berdasarkan features importance model). Pengguna dapat mengeksplorasi bagaimana faktor-faktor seperti OverTime, MonthlyIncome, atau Age berkorelasi dengan attrition.
- Analisis Demografi Karyawan: Visualisasi distribusi karyawan berdasarkan departemen dan peran pekerjaan untuk mengidentifikasi segmen karyawan yang berbeda.
- Perbandingan Kategori dengan Attrition: Visualisasi dengan bar chart yang membandingkan attrition rate di berbagai kategori seperti lembur, usia, overtime dan peran pekerjaan memberikan insight langsung tentang area yang perlu diperhatikan.

![Dashboard _Attrition_Karyawan](https://github.com/user-attachments/assets/4fa5710c-64ac-47df-92ea-aea19ce5c74a)

## Conclusion

Proyek ini telah berhasil mengatasi permasalahan attrition rate di Jaya Jaya Maju dengan implementasi solusi data science yang komprehensif. Analisis data yang dilakukan mengungkapkan bahwa MonthlyIncome, Age, MonthlyRate, dan OverTime_Yes adalah faktor-faktor paling signifikan yang berkontribusi terhadap kecenderungan keluarnya karyawan, memberikan pemahaman jelas mengenai akar penyebab attrition. Konfirmasi ini secara langsung menjawab kebutuhan perusahaan akan identifikasi faktor pendorong utama.

Selanjutnya, proyek ini dengan tegas menunjukkan bahwa machine learning terbukti sangat efektif dalam memprediksi probabilitas attrition karyawan. Model yang dikembangkan memungkinkan identifikasi proaktif terhadap karyawan berisiko tinggi, suatu kapabilitas yang esensial untuk memitigasi biaya rekrutmen dan menjaga produktivitas. Seluruh artefak proyek telah disiapkan untuk integrasi ke business dashboard yang akan datang, mendukung pengambilan keputusan strategis yang berkelanjutan dan berbasis data.

### Rekomendasi Action Items (Optional)

Berikan beberapa rekomendasi yang dapat dilakukan perusahaan guna menyelesaikan permasalahan atau mencapai target mereka.

1. Tinjau dan Optimalisasi Struktur Kompensasi:
   Prioritas: MonthlyIncome dan MonthlyRate adalah faktor penting.
   Aksi: Lakukan studi perbandingan gaji (benchmarking) dengan industri sejenis untuk memastikan bahwa pendapatan bulanan dan tarif yang diberikan kompetitif. Pertimbangkan penyesuaian gaji berkala, bonus, atau program insentif yang terkait dengan kinerja dan loyalitas. Fokus pada segmen karyawan di mana ketidakpuasan gaji menjadi pendorong utama attrition.

2. Kelola Beban Kerja dan Tingkatkan Keseimbangan Hidup-Kerja:
   Prioritas: OverTime_Yes memiliki dampak signifikan.
   Aksi: Kaji ulang kebijakan dan praktik lembur. Dorong budaya kerja yang menghargai keseimbangan hidup-kerja, misalnya dengan membatasi jam lembur yang tidak perlu, menyediakan fleksibilitas jam kerja, atau mempromosikan well-being karyawan. Identifikasi departemen atau tim yang sering lembur dan kaji ulang alokasi sumber daya mereka.

3. Kembangkan Program Retensi Berbasis Demografi dan Pengalaman:
   Prioritas: Age dan TotalWorkingYears adalah faktor penting.
   Aksi: Merancang program retensi yang disesuaikan untuk berbagai kelompok usia dan tingkat pengalaman. Misalnya, untuk karyawan yang lebih senior atau dengan masa kerja lama, fokus pada pengembangan karir, kesempatan mentoring, atau persiapan pensiun yang menarik. Untuk kelompok usia tertentu yang menunjukkan attrition tinggi, pahami kebutuhan dan aspirasi mereka.

4. Perbaiki Lingkungan Kerja dan Kondisi Harian:
   Prioritas: DailyRate dan DistanceFromHome memiliki pengaruh.
   Aksi: Evaluasi elemen-elemen yang memengaruhi pengalaman kerja harian. Untuk DailyRate, pastikan kompensasi harian adil. Untuk DistanceFromHome, pertimbangkan opsi kerja fleksibel (misalnya, hybrid atau remote jika memungkinkan), tunjangan transportasi, atau fasilitas yang dapat mengurangi beban komuter.

5. Perkuat Ikatan Karyawan dan Dukungan Manajerial:
   Prioritas: YearsAtCompany dan NumCompaniesWorked serta potensi dari YearsInCurrentRole dan YearsWithCurrManager.
   Aksi: Lakukan check-in reguler dengan karyawan, terutama mereka yang telah lama berada di perusahaan atau sering berganti perusahaan. Fokus pada pengembangan hubungan yang kuat antara karyawan dan manajer (YearsWithCurrManager) serta peluang promosi dan pengembangan karir yang jelas (YearsSinceLastPromotion, YearsInCurrentRole).

6. Manfaatkan Dashboard untuk Intervensi Proaktif:
   Aksi: Tim HR harus secara aktif menggunakan business dashboard yang telah dibangun untuk memantau indikator attrition secara berkelanjutan dan mengidentifikasi karyawan yang diprediksi berisiko tinggi untuk keluar. Lakukan wawancara retensi, tawarkan solusi yang disesuaikan (misalnya, pelatihan, perubahan peran, atau peningkatan kompensasi) sebelum karyawan memutuskan untuk keluar.
