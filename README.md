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
- Proyek ini dapat dijalankan dengan mudah menggunakan Google Colabolatory (Colab), yang menyediakan *environment* siap pakai dengan sebagian besar dependensi yang sudah **terinstal**.
- Namun jika ingin menjalankan proyek ini secara local di komputer pribadi, disarankan untuk menggunakan virtual environment untuk mengelola dependensi proyek:

**1. Membuat Virtual Environment (opsional, untuk lokal)**:
Buka terminal atau command prompt, lalu navigasikan ke direktori proyek Anda. Jalankan perintah berikut:

```Bash
python -m venv venv
```

**2. Mengaktifkan Virtual Environment (opsional, untuk lokal)** :
- Windows:
```Bash
.\venv\Scripts\activate
```

- macOS / Linux:
```Bash
    source venv/bin/activate
```

**3. Instalasi Dependensi** :
- Baik di Google Colab maupun di environment lokal (setelah mengaktifkan virtual environment), Anda mungkin perlu menginstal beberapa library tambahan yang tidak tersedia secara default. Pastikan Anda berada di direktori proyek dan jalankan perintah berikut:
```Bash
    pip install -r requirements.txt
```
- Catatan: Jika ada library yang perlu diinstal di Colab, Anda bisa menambahkannya di sel kode awal notebook Colab Anda dengan:
```Bash
!pip install nama_library
```
- Catatan: Untuk menjalankan prediction notebook dibutuhkan file yang ada di folder model.

## **Cara Menjalankan Proyek**
**Menggunakan Google Colaboratory (Direkomendasikan)**
1. **Buka Notebook** : Unggah atau buka file notebook .ipynb proyek ini di Google Colab.
2. **Jalankan Semua Sel** : Pastikan Anda menjalankan semua sel kode secara berurutan, dari atas ke bawah. Ini akan memproses data, melatih model (jika ada), dan menyiapkan dashboard.
3. **Akses Dashboard** : Untuk mengakses dashboard di Looker Studio, gunakan tautan yang disediakan di bagian "Business Dashboard" di bawah ini.

## **Menjalankan Secara Lokal (Opsional)**

Jika telah melakukan langkah-langkah Setup Environment di atas untuk menjalankan proyek secara lokal:
1. Pastikan Virtual Environment Aktif: Di terminal atau command prompt, pastikan Anda telah mengaktifkan virtual environment.
2. Jalankan Skrip Utama: Navigasikan ke direktori utama proyek Anda. Kemudian, jalankan file Python utama proyek Anda. Jika file utama Anda adalah main.py, app.py, atau dashboard.py (sesuaikan dengan nama file Anda):
```Bash
    python nama_file_utama_anda.py
```
3. Akses Dashboard: Setelah skrip berhasil dijalankan, jika dashboard Anda di-hosting secara lokal, alamat akses biasanya akan ditampilkan di terminal (misalnya, http://127.0.0.1:8050/ atau http://localhost:5000/). Namun, untuk dashboard Looker Studio, Anda cukup mengakses tautan  yang di [Employee Attrition Dasboard Jaya Jaya Maju](https://lookerstudio.google.com/reporting/5b531828-11a6-45d6-8dc6-421703777b92) berikan di bagian "Business Dashboard".

## Business Dashboard

*Business dashboard* yang dibuat menggunakan Looker Studio dirancang untuk memberikan visibilitas dan *insight* yang cepat kepaada Manajemen dan Departemen HR tentang faktor-faktor attriotion di Jaya Jaya Maju. Saat ini dashboard dapat diakses melalui [Employee Attrition Dasboard Jaya Jaya Maju](https://lookerstudio.google.com/reporting/5b531828-11a6-45d6-8dc6-421703777b92). Dashboard ini menampilkan Dashboard akan menampilkan fitur-fitur utama berikut:
- Ringkasan Tingkat Attrition: Menampilkan metrik utama seperti attrition rate, jumlah karyawan attrition, dan jumlah karyawan keseluruhan.
- Faktor Pendorong Attrition: Grafik yang menunjukkan fitur yang memengaruhi attrition (berdasarkan features importance model). Pengguna dapat mengeksplorasi bagaimana faktor-faktor seperti OverTime, MonthlyIncome, atau Age berkorelasi dengan attrition.
- Analisis Demografi Karyawan: Visualisasi distribusi karyawan berdasarkan departemen dan peran pekerjaan untuk mengidentifikasi segmen karyawan yang berbeda.
- Perbandingan Kategori dengan Attrition: Visualisasi dengan bar chart yang membandingkan attrition rate di berbagai kategori seperti lembur, usia, overtime dan peran pekerjaan memberikan insight langsung tentang area yang perlu diperhatikan.

![Dashboard _Attrition_Karyawan](https://github.com/user-attachments/assets/4fa5710c-64ac-47df-92ea-aea19ce5c74a)

## Conclusion

Proyek ini telah berhasil mengatasi permasalahan attrition rate di Jaya Jaya Maju dengan implementasi solusi data science yang komprehensif. Analisis data yang dilakukan mengungkapkan bahwa **karyawan yang cenderung mengalami attrition memiliki karakteristik umum sebagai berikut**:

- **Pendapatan dan Tingkat Gaji Rendah**: Karyawan dengan MonthlyIncome dan MonthlyRate yang lebih rendah memiliki kecenderungan lebih tinggi untuk keluar. Ini menunjukkan bahwa kompensasi menjadi faktor pendorong signifikan.
- **Usia Lebih Muda**: Karyawan dengan Age yang lebih muda (terutama di rentang awal karir) menunjukkan tingkat attrition yang lebih tinggi, kemungkinan karena mencari peluang pertumbuhan atau pengalaman baru.
- **Sering Lembur** (OverTime_Yes): Karyawan yang sering bekerja lembur memiliki probabilitas attrition yang jauh lebih tinggi, mengindikasikan masalah keseimbangan hidup-kerja yang serius.
- **Masa Kerja Pendek di Perusahaan/Peran**: Faktor seperti YearsAtCompany, YearsInCurrentRole, YearsWithCurrManager, dan NumCompaniesWorked juga berperan, menunjukkan bahwa kurangnya stabilitas, kesempatan promosi, atau hubungan manajerial yang buruk dapat memicu keluarnya karyawan.

- Konfirmasi ini secara langsung menjawab kebutuhan perusahaan akan identifikasi faktor pendorong utama dan karakteristik karyawan berisiko.

- Selanjutnya, proyek ini menunjukkan bahwa machine learning terbukti sangat efektif dalam memprediksi probabilitas attrition karyawan. Model yang dikembangkan memungkinkan identifikasi proaktif terhadap karyawan berisiko tinggi, suatu kapabilitas yang esensial untuk memitigasi biaya rekrutmen dan menjaga produktivitas. Seluruh artefak proyek telah disiapkan untuk integrasi ke business dashboard yang akan datang, mendukung pengambilan keputusan strategis yang berkelanjutan dan berbasis data.

### Rekomendasi Action Items (Optional)

Berikan beberapa rekomendasi yang dapat dilakukan perusahaan guna menyelesaikan permasalahan atau mencapai target mereka.

1. Tinjau dan Optimalisasi Struktur Kompensasi
- Prioritas: MonthlyIncome dan MonthlyRate adalah faktor penting.
- Aksi: Lakukan studi perbandingan gaji (benchmarking) dengan industri sejenis untuk memastikan bahwa pendapatan bulanan dan tarif yang diberikan kompetitif. Pertimbangkan penyesuaian gaji berkala, bonus, atau program insentif yang terkait dengan kinerja dan loyalitas. Fokus pada segmen karyawan di mana ketidakpuasan gaji menjadi pendorong utama attrition.

2. Kelola Beban Kerja dan Tingkatkan Keseimbangan Hidup-Kerja:
- Prioritas: OverTime_Yes memiliki dampak signifikan.
- Aksi: Kaji ulang kebijakan dan praktik lembur. Dorong budaya kerja yang menghargai keseimbangan hidup-kerja, misalnya dengan membatasi jam lembur yang tidak perlu, menyediakan fleksibilitas jam kerja, atau mempromosikan well-being karyawan. Identifikasi departemen atau tim yang sering lembur dan kaji ulang alokasi sumber daya mereka.

3. Kembangkan Program Retensi Berbasis Demografi dan Pengalaman:
- Prioritas: Age dan TotalWorkingYears adalah faktor penting.
- Aksi: Merancang program retensi yang disesuaikan untuk berbagai kelompok usia dan tingkat pengalaman. Misalnya, untuk karyawan yang lebih senior atau dengan masa kerja lama, fokus pada pengembangan karir, kesempatan mentoring, atau persiapan pensiun yang menarik. Untuk kelompok usia tertentu yang menunjukkan attrition tinggi, pahami kebutuhan dan aspirasi mereka.

4. Perbaiki Lingkungan Kerja dan Kondisi Harian:
- Prioritas: DailyRate dan DistanceFromHome memiliki pengaruh.
- Aksi: Evaluasi elemen-elemen yang memengaruhi pengalaman kerja harian. Untuk DailyRate, pastikan kompensasi harian adil. Untuk DistanceFromHome, pertimbangkan opsi kerja fleksibel (misalnya, hybrid atau remote jika memungkinkan), tunjangan transportasi, atau fasilitas yang dapat mengurangi beban komuter.

5. Perkuat Ikatan Karyawan dan Dukungan Manajerial:
- Prioritas: YearsAtCompany dan NumCompaniesWorked serta potensi dari YearsInCurrentRole dan YearsWithCurrManager.
- Aksi: Lakukan check-in reguler dengan karyawan, terutama mereka yang telah lama berada di perusahaan atau sering berganti perusahaan. Fokus pada pengembangan hubungan yang kuat antara karyawan dan manajer (YearsWithCurrManager) serta peluang promosi dan pengembangan karir yang jelas (YearsSinceLastPromotion, YearsInCurrentRole).

6. Manfaatkan Dashboard untuk Intervensi Proaktif:
- Aksi: Tim HR harus secara aktif menggunakan business dashboard yang telah dibangun untuk memantau indikator attrition secara berkelanjutan dan mengidentifikasi karyawan yang diprediksi berisiko tinggi untuk keluar. Lakukan wawancara retensi, tawarkan solusi yang disesuaikan (misalnya, pelatihan, perubahan peran, atau peningkatan kompensasi) sebelum karyawan memutuskan untuk keluar.
