# Membuat Branch Baru

#### 1. Masuk ke direktori repository

Pada terminal, jalankan sintaks berikut:

````bash
cd {nama-folder-odoo-8}/odoo/custom/src/{nama-remote-repository}
````
> Note: Abaikan apabila sudah masuk ke dalam direktori repository

#### 2. Membuat Branch Baru

Pada terminal, jalankan sintaks berikut:

````bash
git checkout -b {odoo-version}-T{nomor-task} origin/8.0
````
Contoh:
````bash
git checkout -b 8.0-T003432 origin/8.0
````
