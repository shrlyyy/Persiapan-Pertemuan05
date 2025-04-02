## 1. Apa itu Multithreading?
Multithreading adalah model eksekusi program yang memungkinkan suatu proses memiliki beberapa thread yang berjalan secara independen tetapi berbagi sumber daya yang sama dalam proses tersebut. Dengan multithreading, tugas dapat dieksekusi secara pararel, meningkatkan efisiensi dan kinerja, terutama pada sistem dengan banyak inti prosesor.
<br>

## 2. Apa perbedaan antara Thread dan Runnable?
| *Aspek* | *Thread* | *Runnable* |
| ----- | ----- | ----- |
| Cara menggunakan | Mewarisi (extends) kelas Thread | Mengimplementasikan (implements) antarmuka Runnable |
| Tujuan | Digunakan jika ingin membuat Thread dengan kemampuan tambahan selain run() | Digunakan jika hanya perlu mengganti metode run() tanpa memodifikasi metode lain dalam Thread |
| Hubungan | Thread sendiri mengimplementasikan Runnable | Runnable adalah cara untuk membuat kelas dapat dieksekusi oleh thread tanpa mewarisi Thread |
| Struktur Kode | Harus meng-override metode run() dalam kelas Thread | Harus mengimplementasikan metode run() dari antarmuka Runnable |
| Cara Menjalankan | Membuat objek dari kelas Thread, lalu memanggil start() | Membuat objek Thread dengan Runnable sebagai parameter, lalu memanggil start() |
| Fleksibilitas | Kurang fleksibel karena langsung mewarisi Thread | Lebih fleksibel karena hanya menggunakan antarmuka |
| Keterbatasan | Tidak bisa mewarisi kelas lain karena Java tidak mendukung multiple inheritance | Bisa tetap mewarisi kelas lain karena hanya mengimplementasikan antarmuka |

## 3. Thread.sleep() digunakan untuk?
Thread.sleep() digunakan untuk menjeda eksekusi thread saat ini selama waktu tertentu (dalam milidetik) tanpa menghentikan keseluruhan program.<br>
Fungsi ini memiliki beberapa kegunaan, seperti membuat jeda dalam eksekusi thread (misalnya, dalam animasi atau proses loading), mengontrol alur program agar tidak berjalan terlalu cepat, serta mensimulasikan delay atau waktu tunggu dalam proses asinkron.
