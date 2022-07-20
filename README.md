membuat node.js
sudo git clone https://github.com/sam-meech-ward-bcit/lotr
masukin ke etc/systemd/system/lotr.service

[Unit]
Description=My Node Server
After=multi-user.target

[Service]
ExecStart=/usr/bin/node /home/ec2-user/lotr/server.js
Restart=always
RestartSec=10
StandardOutput=syslog
StandardError=syslog
SyslogIdentifier=my-node-server
User=ec2-user
EnvironmentFile=/home/ec2-user/lotr/app.env

[Install]
WantedBy=multi-user.target

-sudo system start lotr.service
-sudo system status lotr.service 
- suo cat var/log/syslog




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
-hubungkan api dari luar


MODUL 3

1. buat rds
1. buat ec2 dan install node js
2. buat AMI 
3. load balancing 
4. auto scaling
6. ealastichace
7. route 53

PORT yang di butuhkan 
 
 1.SSH(buat di terminal)
 2.https
 3.http
 4.port 8080 (buat node.js)
 5.MYSQL 
 6.6379 (buat elastichace)



