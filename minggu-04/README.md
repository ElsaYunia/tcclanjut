# Komunikasi 2 Container
Untuk menghubungkan antara 2 kontainer yang berbeda, maka diperlukan media. Ada 2 cara untuk menghubungkannya.

## 1. Menggunakan Network
1. Menjalankan container. pada contoh ini, menggunakan image dari Redis-server
![1](https://user-images.githubusercontent.com/43244821/55660875-b2a0c300-5832-11e9-88de-747a25b7e3ed.jpg)

2. Membuat Link
Link digunakan untuk menyesuaikan environment variabel. Pada contoh ini, kontainer redis akan di link kan dengan container dari alpine.
Hasilnya, akan memberikan informasi ports dan ip address
![2](https://user-images.githubusercontent.com/43244821/55660941-14f9c380-5833-11e9-8aeb-9c78dbba5f3f.jpg)

3. Docker akan melakukan update hosts file dari container 
![3](https://user-images.githubusercontent.com/43244821/55660982-496d7f80-5833-11e9-9a28-feed38cb5275.jpg)

4. Link sudah dibuat. Sekarang ping pada container alpine dengan melakukan link ke container redis seperti berikut
![4](https://user-images.githubusercontent.com/43244821/55661006-7752c400-5833-11e9-8db7-b947d86a536e.jpg)

5. Connect dengan aplikasi
Disini menggunakan aplikasi node.js yang akan dikoneksikan menggunakan hostname redis
![5](https://user-images.githubusercontent.com/43244821/55661089-019b2800-5834-11e9-9f7f-03d6f13454a3.jpg)

6. Test Koneksi
![6](https://user-images.githubusercontent.com/43244821/55661106-1081da80-5834-11e9-8c22-7c9367baa3ee.jpg)

7. Menggunakan Redis CLI
![7](https://user-images.githubusercontent.com/43244821/55661124-28f1f500-5834-11e9-8611-7925d3cf7636.jpg)


## 2. Menggunakan Link

