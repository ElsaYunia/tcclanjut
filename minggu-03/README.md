# PART 1 : Deploying Your First Docker Container
Pada praktikum part 1, membahas tentang bagaimana melakukan deploy sebuah docker container. 

## Step 1 - Menjalankan Kontainer
1. Mengidentifikasi Docker Image dengan menjalankan Redis. Mencari image dengan perintah "docker search redis"
   ![1](https://user-images.githubusercontent.com/43244821/54689049-5dd22c80-4b51-11e9-8e80-cc8a123536b7.JPG)

2. Menjalankan image redis dengan menggunakan docker run
   ![2](https://user-images.githubusercontent.com/43244821/54689150-8ce89e00-4b51-11e9-8b7e-6eb4feb79a8d.JPG)
   
## Step 2 - Melihat Container yang dijalankan
1. Melihat kontainer yang dijalankan dengan menggunakan "docker ps"
   ![3](https://user-images.githubusercontent.com/43244821/54689307-d933de00-4b51-11e9-8025-79335300c911.JPG)
   
## Step 3 - Mengakses Redis
1. Mengakses Redis dengan menggunakan port 6379 
   ![4](https://user-images.githubusercontent.com/43244821/54689449-231cc400-4b52-11e9-8fc9-6ea6dfb05358.JPG)

## Step 4 - Mengakses Redis
1. Konfigurasi port dan testing
   ![5](https://user-images.githubusercontent.com/43244821/54757238-65aad300-4c1c-11e9-9683-a53d1ecb0edc.JPG)
   
2. Ketika port sudah berhasil, kita harus mengatur port yang dipakai
   ![6](https://user-images.githubusercontent.com/43244821/54757741-70b23300-4c1d-11e9-9611-081b9e705aa5.JPG)

3. Kemudian lihat lagi daftar kontainer
   ![7](https://user-images.githubusercontent.com/43244821/54757795-89224d80-4c1d-11e9-927c-18db1bb0a5b6.JPG)

## Step 5 - Persisting Data
Beberapa data yang dibutuhkan tersimpan didalam Docker Host tidak didalam kontainer. Jadi, harus tersimpan didalam               /opt/docker/data/redis.
Untuk menyimpannya, dengan perintah :
![8](https://user-images.githubusercontent.com/43244821/54757858-a6efb280-4c1d-11e9-837b-f80cd2370971.JPG)

## Step 6 - Menjalankan Kontainer
1. Menjalankan Ubuntu Kontainer
   ![9](https://user-images.githubusercontent.com/43244821/54757953-d30b3380-4c1d-11e9-99d7-2f1c65631b37.JPG)
   
2. Menjalankan bash shell Ubuntu
   ![10](https://user-images.githubusercontent.com/43244821/54758008-f0d89880-4c1d-11e9-8531-e93e32d6b2b3.JPG)
   
# PART 2 : Deploy Static HTML Website as Container
Pada part 2, mmembuat dockerfile untuk melakukan deploy web sebagai kontainer

## Step 1 - Membuat Dockerfile
1. Membuat dockerfile untuk membuat image
   ![1](https://user-images.githubusercontent.com/43244821/54758313-8411ce00-4c1e-11e9-84e1-87bc7d5f4694.JPG)
   
## Step 2 - Build Image
1. Dockerfile dibuat menggunakan Docker CLI. Hasil dari dockerfile, akan menjadi Docker Image dan dapat dijalankan sebagai aplikasi.        Format untuk build :
   ![2](https://user-images.githubusercontent.com/43244821/54759555-e7046480-4c20-11e9-9be8-0b7d03ebaecf.JPG)
   
2. Melihat daftar images
   ![3](https://user-images.githubusercontent.com/43244821/54759746-4d898280-4c21-11e9-88d6-b0168b835d82.JPG)
   
## Step 3 - Run
1. Menjalankan image dengan port 80
   ![4](https://user-images.githubusercontent.com/43244821/54760933-ac4ffb80-4c23-11e9-98c2-33f818f64b06.JPG)

2. Via curl docker
   ![5](https://user-images.githubusercontent.com/43244821/54760957-bc67db00-4c23-11e9-89e8-7dd5477230eb.JPG)
   
3. Test menggunakan web browser
   ![6](https://user-images.githubusercontent.com/43244821/54761005-d73a4f80-4c23-11e9-9901-31fbf6394373.JPG)

# PART 3 : Building Container Images
1. Membuat dockerfile
   ![4](https://user-images.githubusercontent.com/43244821/54762230-41ec8a80-4c26-11e9-8e63-ef0b249d81ce.JPG)

2. Build Container
   ![5](https://user-images.githubusercontent.com/43244821/54762295-6b0d1b00-4c26-11e9-82f0-923f1621a983.JPG)
   
3. Melihat daftar images
   ![6](https://user-images.githubusercontent.com/43244821/54762344-837d3580-4c26-11e9-99bc-24144524cf6b.JPG)
   
4. Menjalankan image 
   ![7](https://user-images.githubusercontent.com/43244821/54762390-9e4faa00-4c26-11e9-832d-98b3555c9cc5.JPG)

5. Mengakses image
   ![8](https://user-images.githubusercontent.com/43244821/54762437-b7f0f180-4c26-11e9-83d8-cba4053fdfe7.JPG)

6. Melihat daftar images
   ![9](https://user-images.githubusercontent.com/43244821/54762495-d6ef8380-4c26-11e9-80bd-b23e62ecc98b.JPG)

   


   
