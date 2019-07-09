## Start Containers using Kubectl
1. Menjalankan minikube
   ![Screenshot_1](https://user-images.githubusercontent.com/43244821/58264468-1f9ef680-7da8-11e9-903b-57170703f56e.jpg)
2. Melihat nodes
   ![Screenshot_2](https://user-images.githubusercontent.com/43244821/58264490-29c0f500-7da8-11e9-89b9-5a85400d0d29.jpg)
3. Melakukan Run Image
   ![Screenshot_3](https://user-images.githubusercontent.com/43244821/58264531-36dde400-7da8-11e9-870f-492895c4acec.jpg)
4. Melihat image yang sudah dideployment
   ![Screenshot_4](https://user-images.githubusercontent.com/43244821/58264549-40ffe280-7da8-11e9-889e-0be214dc53f6.jpg)
5. Melihat describe deployment
   ![Screenshot_5](https://user-images.githubusercontent.com/43244821/58264582-4b21e100-7da8-11e9-83d9-71622ba59b45.jpg)
6. Melakukan kubectl expose
   ![Screenshot_6](https://user-images.githubusercontent.com/43244821/58264606-5543df80-7da8-11e9-81bf-320ef6d3b1c7.jpg)
7. Melakukan testing
   ![Screenshot_7](https://user-images.githubusercontent.com/43244821/58264708-7f959d00-7da8-11e9-8195-32eb64a8dc93.jpg)
8. Melakukan kubectl run dan expose port 8001
   ![Screenshot_8](https://user-images.githubusercontent.com/43244821/58264730-8a503200-7da8-11e9-874b-abc8de6b537d.jpg)
9. Testing akses
   ![Screenshot_9](https://user-images.githubusercontent.com/43244821/58264749-96d48a80-7da8-11e9-992d-d70c21bb886a.jpg)
10.Melihat service yang dijalankan
   ![Screenshot_10](https://user-images.githubusercontent.com/43244821/58264766-a0f68900-7da8-11e9-8b70-d7de0c498775.jpg)
11. Melihat detail
    ![Screenshot_11](https://user-images.githubusercontent.com/43244821/58264780-a94ec400-7da8-11e9-9678-8cddb2b783d7.jpg)
12. Melakukan scale containers, dengan replica = 3
    ![Screenshot_12](https://user-images.githubusercontent.com/43244821/58264817-ba97d080-7da8-11e9-95b1-8eb35341c2fe.jpg)
13. Melihat daftar pods
    ![Screenshot_13](https://user-images.githubusercontent.com/43244821/58264839-c4b9cf00-7da8-11e9-8a20-2ec6e41145e4.jpg)
14. Melihat describe service
    ![Screenshot_14](https://user-images.githubusercontent.com/43244821/58264864-cdaaa080-7da8-11e9-85a7-eab7621f35b9.jpg)
15. Melakukan testing
    ![Screenshot_15](https://user-images.githubusercontent.com/43244821/58264887-d9966280-7da8-11e9-98b8-f746b7eef65e.jpg)

## Deploy Containers Using YAML
1. Membuat file konfigurasi YAML
   ![1](https://user-images.githubusercontent.com/43244821/58264933-f16de680-7da8-11e9-9d2f-9f5b57f97a39.jpg)
2. Membuat deployment
   ![2](https://user-images.githubusercontent.com/43244821/58264953-fb8fe500-7da8-11e9-9169-ed7ad4067757.jpg)
3. Melihat pods yang di deploy
   ![3](https://user-images.githubusercontent.com/43244821/58264969-034f8980-7da9-11e9-8602-f352c2bb8d24.jpg)
4. Melihat describe dari deployment
   ![4](https://user-images.githubusercontent.com/43244821/58265000-0cd8f180-7da9-11e9-87f8-d04d09fd4bd4.jpg)
5. Membuat file service.yaml
   ![5](https://user-images.githubusercontent.com/43244821/58265025-19f5e080-7da9-11e9-87c4-49a5aad532b9.jpg)
6. Membuat service
   ![6](https://user-images.githubusercontent.com/43244821/58265043-224e1b80-7da9-11e9-83ca-3fea13b04d8d.jpg)
7. Melihat daftar service
   ![7](https://user-images.githubusercontent.com/43244821/58265089-3c87f980-7da9-11e9-9653-89dcbced680c.jpg)
8. Melihat deskripsi service
   ![8](https://user-images.githubusercontent.com/43244821/58265466-ee272a80-7da9-11e9-873b-c629808b4961.jpg)
9. Melakukan testing
   ![9](https://user-images.githubusercontent.com/43244821/58265487-fa12ec80-7da9-11e9-9d81-37abae6ba7f0.jpg)
10. Mengganti jumlah replica=4
    ![10](https://user-images.githubusercontent.com/43244821/58265503-026b2780-7daa-11e9-8fcf-9415d62f2b49.jpg)
11. Membuat file konfigurasi
    ![11](https://user-images.githubusercontent.com/43244821/58265516-0ac36280-7daa-11e9-8b41-1e72bdc0441b.jpg)
12. Membuat deployment dengan jumlah replica=4
    ![12](https://user-images.githubusercontent.com/43244821/58265537-144cca80-7daa-11e9-9445-1c31fb062cef.jpg)
13. Melihat jumlah pods
    ![13](https://user-images.githubusercontent.com/43244821/58265612-35adb680-7daa-11e9-8372-bc82d62e41ee.jpg)
14. Melakukan Testing
    ![14](https://user-images.githubusercontent.com/43244821/58265624-3d6d5b00-7daa-11e9-896a-289d7eb4b818.jpg)

