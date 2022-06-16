# Tugas6_SBD

Nama    : Didi Kumaedi

NIM   : 312010002

Kelas   : TI.20.D.1

Matkul    : Sistem Basis Data

- Masuk ke databse nama_nim

![image](https://user-images.githubusercontent.com/101849655/174044666-566a3d8e-0ea4-42df-9b83-05b9f51b1f12.png)

- Lakukan proses backup dan recovery dengan sql dari database tugas seblumnya !
Backup

![Screenshot (78)](https://user-images.githubusercontent.com/101849655/174047167-c55fa85d-bdc2-4973-8079-d920a74cc5fd.png)

jika proses backup berhasil maka akan muncul file backuppada direktori C:\xampp\mysql\data\nama database

![image](https://user-images.githubusercontent.com/101849655/174047421-56046f1e-9eee-4e3c-9b5d-3e0c32290c32.png)

Recovery

Data yang telah di-backup dapat dikembalikan kapan saja bila diperlukan. Sintaks SQL yang digunakan adalah LOAD DATA INFILE. Perintah yang dijalankan adalah

LOAD DATA INFILE ‘Nama_backup_file’ INTO TABLE nama_table ;

![Screenshot (79)](https://user-images.githubusercontent.com/101849655/174047830-9bc4afbf-2add-49eb-82fb-e16a75e3a467.png)

![Screenshot (80)](https://user-images.githubusercontent.com/101849655/174048001-f5181bbd-309c-4f44-814b-06001accdf01.png)

![Screenshot (82)](https://user-images.githubusercontent.com/101849655/174048193-2f978eb9-009b-44af-80f3-4c1aecfc3cac.png)

- Lakukan proses backup dan recovery dengan sqldump dari database tugas seblumnya !

![Screenshot (84)](https://user-images.githubusercontent.com/101849655/174048457-7c4b9f14-e5d2-474b-b5d4-7aeb54666eda.png)


Tulisakan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam !
crontab –e

00**7myqldump -u root -p didi_kumaedi_312010002>didi_kumaedi_312010002_backup.sql
