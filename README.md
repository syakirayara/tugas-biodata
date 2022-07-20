s3
- jika ingin menghapus file pada s3 dan masih ingin meninggalkan jejak, pertama hapus tampa mengaktifkan version dan ke dua hapus dengan mengaktifkan version.
* fungsi dari versioning adalah untuk roal back (kembali ke versi ke sebelumnya)

cloudFrount 

* berguna untuk menyimpan file file yang sudah pernah di akses dan mendekatkan yang jauh (menyimpan file file yang sering dan pernah kita akses)
- harus membuat s3 terlebih dahulu
- kosongkan origin path
- name nya standar
- untuk acsess gunakan 'yes OAI'
- gunakan acsess identity
- pilih update
-jika berhasil (sertivicate manager untuk https) bisa di tambahkan CNAME

route 53

-buat creat record 
-kalau udh baru ke sertificate manager

sertificate manager

-request
-masukan domain
-gunakan DNS validasi

#modul 1

-s3
-route 53
-lambda
-dynamodb
-lamba + dynamodb
-api gateway
-akses api dari luar

MODUL 3

1. buat ec2 dan install node js
2. buat AMI 
3. load balancing 
4. auto scaling
5. rds
6. ealastichace
7. route 53
-hubungkan api dari luar


