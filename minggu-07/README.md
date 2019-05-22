# Bagian 1 -- Docker Compose

##  Step 1 - Defining First Container
1. Docker compose didibuat dalam bentuk file docker-compose.yaml. Pertama, isi file tersebut untuk kontainer yang akan dijalankan
Kemudian menghubungkan 2 container dengan menggunakan links dan berjalan di port 3000:8000. 
![3](https://user-images.githubusercontent.com/43244821/56709472-aaf67f00-674b-11e9-85b8-3397d58f248a.JPG)

2. Kemudian docker-compose untuk menjalankan file tersebut.

![4](https://user-images.githubusercontent.com/43244821/56709580-38d26a00-674c-11e9-8ec2-53a23122664b.JPG)
![5](https://user-images.githubusercontent.com/43244821/56709586-42f46880-674c-11e9-9ede-46b1772d148c.JPG)

3. Melihat daftar container yang berjalan

![6](https://user-images.githubusercontent.com/43244821/56709604-60c1cd80-674c-11e9-89ac-5abd45536be6.JPG)

4. Melihat logs

![7](https://user-images.githubusercontent.com/43244821/56709616-70411680-674c-11e9-8c8d-db39e0e0eba7.JPG)

5.Docker scale

![9](https://user-images.githubusercontent.com/43244821/56709659-9a92d400-674c-11e9-8d9c-7250670b4962.JPG)
![10](https://user-images.githubusercontent.com/43244821/56709670-a54d6900-674c-11e9-9cd0-0d67bb0b77dd.JPG)

6. Menghentikan docker compose

![11](https://user-images.githubusercontent.com/43244821/56709688-be561a00-674c-11e9-8dfd-816a8920cd3b.JPG)

7. Menghapus Docker Compose

![12](https://user-images.githubusercontent.com/43244821/56709698-ce6df980-674c-11e9-9bd2-e25e80b48009.JPG)

# Bagian 2-- Docker Swarm

1. Melihat perintah docker swarm

![1](https://user-images.githubusercontent.com/43244821/56709766-3d4b5280-674d-11e9-9b17-d37ccb536537.JPG)

2. Docker swarm init

![2](https://user-images.githubusercontent.com/43244821/56709784-52c07c80-674d-11e9-92c6-1414b6b5a7a6.JPG)

3. Melakukan join di Terminal Host 2

![3](https://user-images.githubusercontent.com/43244821/56709811-75eb2c00-674d-11e9-8d27-f17f24ca9612.JPG)

4. Menggunakan alamat Ip

![4-terminal2](https://user-images.githubusercontent.com/43244821/56709837-91563700-674d-11e9-9724-a5a0134275eb.JPG)

5. Melihat daftar node

![5](https://user-images.githubusercontent.com/43244821/56709850-a3d07080-674d-11e9-8fc9-7c8620efa879.JPG)

6. Membuat docker network

![6](https://user-images.githubusercontent.com/43244821/56709866-b6e34080-674d-11e9-89d8-a8b3eaa21570.JPG)

7. Membuat replickasi dengan docker service

![7](https://user-images.githubusercontent.com/43244821/56709895-db3f1d00-674d-11e9-96b8-5b5d493c734e.JPG)

8. Melihat daftar docker service

![8](https://user-images.githubusercontent.com/43244821/56709904-eabe6600-674d-11e9-8d03-f395157adb2f.JPG)

9. Melihat daftar kontainer

![9](https://user-images.githubusercontent.com/43244821/56709923-01fd5380-674e-11e9-9db9-4b06dcf21653.JPG)

10. Melihat daftar container di terminal host 2

![10](https://user-images.githubusercontent.com/43244821/56709973-38d36980-674e-11e9-8a77-c12ef2086eb7.JPG)

11. Melihat proses

![11](https://user-images.githubusercontent.com/43244821/56710004-5e607300-674e-11e9-9f79-3267a4c2a7aa.JPG)

12. Melihat docker service

![12](https://user-images.githubusercontent.com/43244821/56710033-720bd980-674e-11e9-9d02-bd4b297e7018.JPG)

13. Docker inspect

![13](https://user-images.githubusercontent.com/43244821/56710065-9962a680-674e-11e9-8650-3e725ce01fbf.JPG)

14. Melihat node

![14](https://user-images.githubusercontent.com/43244821/56710100-b303ee00-674e-11e9-9f94-9525170cc94a.JPG)
![15](https://user-images.githubusercontent.com/43244821/56710121-cd3dcc00-674e-11e9-89a9-f4e81c50e955.JPG)

15. Melihat proses

![16](https://user-images.githubusercontent.com/43244821/56710150-ed6d8b00-674e-11e9-8763-f049ecd8aa30.JPG)

16. Docker scale

![17](https://user-images.githubusercontent.com/43244821/56710168-0118f180-674f-11e9-9183-92e216a62c8e.JPG)

17. Melihat daftar container

![18](https://user-images.githubusercontent.com/43244821/56710193-1aba3900-674f-11e9-9166-df03a682e9a8.JPG)
