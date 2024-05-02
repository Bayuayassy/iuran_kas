# Laporan Keuangan Kas RT

 **Nama Kelompok** : 
 
 - Bayu Maulana Ayassy   (312210166)
 
 - Yoga Pratama          (312210042)
 
 - Cahyo Hidayatullah    (312210079)

 **Disini kami ingin menyelesaikan tugas dari mata kuliah pemrograman mobile 2 tentang** :
 ![Cuplikan layar 2024-04-18 233934](https://github.com/Bayuayassy/iuran_kas/assets/115678251/3722a93e-8a37-417a-9060-2eacacc6c34f)

**Deskripsi:**

Aplikasi Android ini dibuat untuk mempermudah pengelolaan keuangan Kas RT dengan menampilkan laporan keuangan yang terstruktur dan mudah dipahami. Laporan keuangan ini diperoleh dengan parsing data JSON dari Google Spreadsheets melalui API Spreadsheets.

**Teknologi:**

* Android Studio
* Kotlin
* API Spreadsheets
* Google Spreadsheets

**Struktur Proyek:**

* **model:** Berisi kelas-kelas model data, seperti `DataItem.kt` dan `ResponseUser.kt`.
* **network:** Berisi konfigurasi API dan service, seperti `ApiConfig.kt` dan `ApiService.kt`.
* **res:** Berisi kode utama aplikasi Android, konfigurasi build, dan resources (seperti gambar, string, dan layout).
* **layout:** Berisi file-file layout XML yang digunakan untuk mendesain tampilan aplikasi.

**Penjelasan Kode:**

* File `MainActivity.kt` merupakan file utama yang berisi kode untuk menampilkan data dari JSON dan menampilkannya di layout.
* File `DataItem.kt` dan `ResponseUser.kt` merupakan kelas model data yang digunakan untuk memetakan data JSON ke objek Kotlin.
* File `ApiConfig.kt` berisi konfigurasi API, seperti URL endpoint dan API key.
* File `ApiService.kt` berisi interface API yang mendefinisikan method-method untuk melakukan request dan menerima response dari API.

**Langkah Penggunaan:**

1. Buat spreadsheet di Google Spreadsheets dengan kolom-kolom yang sesuai dengan data yang ingin ditampilkan (foto, nama, alamat, iuran, dll.).
2. Dapatkan link spreadsheet dari Google Spreadsheets.
3. Masukkan link spreadsheet di file `ApiConfig.kt`.
4. Tambahkan dependencies berikut di file `build.gradle` pada module `app`:

```
dependencies {
  ...
    implementation("androidx.recyclerview:recyclerview:1.3.2")
    implementation("com.github.bumptech.glide:glide:4.11.0")
    implementation("com.loopj.android:android-async-http:1.4.9")

    implementation("com.google.code.gson:gson:2.8.9")

    implementation("com.squareup.retrofit2:retrofit:2.6.4")
    implementation("com.squareup.retrofit2:converter-gson:2.6.4")

    implementation("com.squareup.okhttp3:logging-interceptor:3.8.0")
    debugImplementation("com.github.chuckerteam.chucker:library:3.3.0")
}
```

5. Build dan jalankan aplikasi di Android Studio.

**Catatan:**

* Pastikan data di spreadsheet sudah terstruktur dengan benar.
* Untuk menambahkan foto warga, upload foto ke Google Drive dan masukkan link fotonya di kolom spreadsheet.

**Link:**

* Youtube: 
* Laporan PDF: https://drive.google.com/file/d/1-OVRWNiJjLFpq-4QWZV01_RO1oTBOI69/view?usp=sharing 

**Referensi:**

* API Spreadsheets: [https://www.apispreadsheets.com/](https://www.apispreadsheets.com/)
* Membuat Aplikasi Android dengan Kotlin: [https://developer.android.com/courses/kotlin-bootcamp/overview](https://developer.android.com/courses/kotlin-bootcamp/overview)

**Terima kasih!**

Kami harap penjelasan ini bermanfaat dan membantu kalian memahami cara kerja aplikasi ini.



