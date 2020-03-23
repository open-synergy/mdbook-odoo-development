# Mempersiapkan Development Environment

### 1. Buka terminal
### 2. Clone repositori doodba scafolding

Sintaks untuk ssh:

```bash
git clone -b <versi-odoo> git@github.com:open-synergy/doodba-scaffolding.git <nama-folder-development>
```

Sintaks untuk https:

```bash
git clone -b <versi-odoo> https://github.com/open-synergy/doodba-scaffolding.git <nama-folder-development>
```

Keterangan:

* *versi-odoo*: versi Odoo yang akan didevelop. Contoh: 8.0, 9.0
* *nama-folder-development*: nama folder yang akan menampung hasil clone. Bebas.

### 3. Masuk ke dalam folder *nama-folder-development*

Sintaks:

```bash
cd <nama-folder>
```

### 4. Perbesar disk size untuk inotify

Sintaks:

```bash
echo 16384 | sudo tee /proc/sys/fs/inotify/max_user_watches
```

### 5. chmod folder odoo/auto

Sintaks:

```bash
chmod -R ug+rwX odoo/auto
```

### 6. Sesuaikan environment variable *UID* dan *GID*

Sintaks:

```bash
export UID GID="$(id -g $USER)" UMASK="$(umask)"
```

### 7. Pull dan build docker image yang akan digunakan

Sintaks:

```bash
sudo docker-compose -f devel.yaml build --pull
```

### 8. Jalankan git-aggregator untuk melakukan clone odoo, ocb, dan OpenUpgrade codebase

Sintaks:

```bash
sudo docker-compose -f setup-devel.yaml run --rm odoo
```
