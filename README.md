

# PROJECT-2-LATIHAN-
# LANGKAH 1 
# Membuat Direktori untuk 3 Departemen MARKETING,ENGINEERING,HR
Definisi gambar
https://drive.google.com/file/d/1gGkJ_udy1NnmEAujefrjJUWcnuaTfCpy/view?usp=drivesdk
```
mkdir Marketing Enginering HR
```
# MEMBUAT SUBFOLDER DI MASING-MASING DIREKTORI
Definisi gambar
https://drive.google.com/file/d/1aXM81VNuzi35oNWK0vhTBMFv8itbI-pt/view?usp=drivesdk
```
divamakalalag@divamakalalag-virtualbox:$ cd Marketing
divamakalalag@divamakalalag-virtualbox:$ mkdir Documents Archives
divamakalalag@divamakalalag-virtualbox:$ cd Documeumen
divamakalalag@divakakalalag-virtualbox-Documents:$ touch Marketing.docx
divamakalalag@divamakalalag-virtualbox-Documents:$ cd ..
divamakalalag-virtualbox:$cd Archives
divamakalalag-virtualbox-Archives:$ touch TargetPasar_file.pdf
divamakalalag-virtualbox-Archives:$cd ..
```
*`Penjelasan`.
* `mkdir` → membuat folder baru.
* `touch` → membuat file baru.
* `cd` → masuk ke folder.
* `cd ..` → keluar ke folder sebelumnya.
# LANGKAH 2 MEMINDAHKAN FILE YANG SALAH TEMPAT KE FIREKTORI YANG BENAR
Definisi gambar
https://drive.google.com/file/d/1GtDOaYN2agAC-w_C7J12u-D_62aMABib/view?usp=drivesdk
```
mv images/file11.jpg Marketing/Documents
```
```
mv images/file12.jpg Engineering/Documents
```
```
mv images/file13.jpg HR/Documents
```
# MEMBUAT BACKUP DI FOLDER ARCHIVES
Definisi gambar
https://drive.google.com/file/d/1X-YemVfgfPnK6u7y88dygGDf90Pt7Cst/view?usp=drivesdk.
```
cp -r Marketing/Dokuments/Marketing.docx Marketing/Archives
```
```
cp -r Engineering/Documents/Engineering.docx Engineering/Archives
```
```
cp -r HR/Documents/HR.docx HR/Archives
```
# LANGKAH 3 SET PERMISION/MEMBATASI HAK AKSES DI SETIAP FOLDER
Defenisi gambar
https://drive.google.com/file/d/1oQ1PoDdJhERrq4TtiwMxu6FAr8M6zlXw/view?usp=drivesdk
```
sudo groupadd Marketing
```
```
sudo groupadd Enginering
```
```
sudo groupadd HR 
```
# MENGUBAH KEPEMILIKAN FOLDER DAN SEMUA ISI DI DALAMNYA
Definisi gambar
https://drive.google.com/file/d/1BlRZtkOGeNyHHA6UAMJoe5ha04LLlV2i/view?usp=drivesdk
```
sudo chgrp -r Marketing Marketing
```
```
sudo chgrp -r Engineering Engineering
```
```
sudo chgrp -r HR HR
```
# MENGATUR IZIN PERMISION FOLDER
Definis gambar
https://drive.google.com/file/d/19BhLSdDypQsdeA2NhuTQwpGvDYWSJgga/view?usp=drivesdk
```
sudo chmod 770 Marketing
```
```
sudo chmod 770 Engineering
```
```
sudo chmod 770 HR
```

*`Penjelasan`.
* `sudo groupadd` → menambahkan grup.
* `sudo chgrp` → mengubah kepemilikan grup.
* `sudo chmod 770` → mengatur izin akses
* `7` → buat owner.
* `7` → buat group.
* `0` → buat outher.

# LATIHAN 4 MENAMPILKAN FILE PDF -7 HATI YANG LALU
definisi gambar
https://drive.google.com/file/d/1DpwXZKaeOPC2RseHDqgFrAp-eTrI6Ng3/view?usp=drivesdk
```
find . -type f -iname "*.pdf" -mtime -7
```
*`Penjelasan`.
* `find` → mencari file/folder sesuai nama,tipe,ukuran,dll
