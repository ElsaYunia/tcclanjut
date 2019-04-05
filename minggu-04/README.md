# Komunikasi 2 Container
Untuk menghubungkan antara 2 kontainer yang berbeda, maka diperlukan media. Ada 2 cara untuk menghubungkannya.

## 1. Menggunakan Links
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


## 2. Menggunakan Network
1. Membuat Network

![Screenshot_1](https://user-images.githubusercontent.com/43244821/55661586-ccdca000-5836-11e9-8914-f0d1728dcf66.jpg)

2. Connect dengan network.  
Ketika meluncurkan kontainer baru, menggunakan --net attribute

![Screenshot_2](https://user-images.githubusercontent.com/43244821/55661591-d6660800-5836-11e9-9305-478482bc5db8.jpg)

3.  Docker tidak lagi menetapkan environment variables dan melakukan perubahan pada hosts file dari kontainerThe first thing you'll notice is that Docker no longer assigns environment variables or updates the hosts file of containers. 

![Screenshot_3](https://user-images.githubusercontent.com/43244821/55661597-debe4300-5836-11e9-99a1-64c8f35d4afa.jpg)

4. Disini kita akan mendapatkan info backend network

![Screenshot_4](https://user-images.githubusercontent.com/43244821/55661601-e7167e00-5836-11e9-8398-830444c33ec9.jpg)

5. Kontainer akan berkomunikasi dengan Embedded DNS Server di docker. DNS server menetapkan semua kontainer berkomunikasi via IP 127.0.0.11 di file resolv.conf

![Screenshot_5](https://user-images.githubusercontent.com/43244821/55661613-ef6eb900-5836-11e9-9e5f-82e32ec82696.jpg)

6. Ketika kontainer akan mengakses kontainer lain, dns sserver akan menggunakan IP address dari kontainer.

![Screenshot_6](https://user-images.githubusercontent.com/43244821/55661620-f7c6f400-5836-11e9-9c5e-d5cef566b29e.jpg)

7. Membuat front-end network

![Screenshot_7](https://user-images.githubusercontent.com/43244821/55661633-01505c00-5837-11e9-9a97-5214249cdb37.jpg)

8. Connect kontainer dengan network

![Screenshot_8](https://user-images.githubusercontent.com/43244821/55661636-0a412d80-5837-11e9-91c5-d0972cbf700b.jpg)

9. Ketika membuka web server, akan otomatis berkomunikasi dengan Redis.kemudian melakukan pull dari image katacoda/redis-node-docker

![Screenshot_9](https://user-images.githubusercontent.com/43244821/55661641-15945900-5837-11e9-8681-ea26c0ef2281.jpg)

10. Melakukan test

![Screenshot_10](https://user-images.githubusercontent.com/43244821/55661647-2218b180-5837-11e9-8f1d-8b313dac625e.jpg)

11. Konek container dengan alias

![Screenshot_11](https://user-images.githubusercontent.com/43244821/55661654-2e047380-5837-11e9-9c1d-1a49c102085f.jpg)

12. Test ping

![Screenshot_12](https://user-images.githubusercontent.com/43244821/55661661-3bb9f900-5837-11e9-9a34-b7f40370a723.jpg)

13. Melihat daftar network

![Screenshot_13](https://user-images.githubusercontent.com/43244821/55661666-44aaca80-5837-11e9-9c02-816a0e6f33ad.jpg)

14. Melihat inspect

![Screenshot_14](https://user-images.githubusercontent.com/43244821/55661673-4eccc900-5837-11e9-86b1-e38be0deffd9.jpg)

15. Mematikan koneksi kontainer

![Screenshot_15](https://user-images.githubusercontent.com/43244821/55661676-57bd9a80-5837-11e9-86ca-9d36d1b947e0.jpg)
