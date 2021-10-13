# Fetch dan Rebase Remote Repository

#### 1. Masuk ke direktori repository

Pada terminal, jalankan sintaks berikut:

````bash
cd {nama-folder-odoo-8}/odoo/custom/src/{nama-remote-repository}
````

#### 2. Checkout branch {odoo-version}

Pada terminal, jalankan sintaks berikut:

````bash
git checkout {odoo-version}
````
> Note: Abaikan apabila branch {odoo-version} sudah tercheckout

#### 3. Fetch remote repository

Pada terminal, jalankan sintaks berikut:

````bash
git fetch origin
````

#### 4. Rebase remote repository

Pada terminal, jalankan sintaks berikut:

````bash
git rebase origin/{odoo-version}
````
