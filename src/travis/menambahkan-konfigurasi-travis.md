# Menambahkan Konfigurasi Travis Di Repo

#### 1. Masuk ke dalam direktori repositori dengan menggunakan terminal

#### 2. Copy file *.travis.yml* dari repo OCA/maintener-quality-tools.

Jalankan sintaks berikut di terminal

````bash
wget https://raw.githubusercontent.com/OCA/maintainer-quality-tools/master/sample_files/.travis.yml .
````

#### 3. Add, commit, dan push .travis.yml

````bash
git add -A .travis.yml \
&& git commit -m "Add travis.yml" \
&& git push origin 12.0:12.0
````

Kode di atas mengasumsikan:

1. Tidak ada branch protection rule yang aktif pada pengaturan branch di github.com
2. Branch yang akan diberikan konfigurasi travis adalah branch 12.0

Silahkan lakukan penyesuaian yang diperlukan.
