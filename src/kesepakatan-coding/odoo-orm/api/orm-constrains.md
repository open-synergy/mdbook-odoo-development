# Constrains

API Constrains biasa digunakan untuk mencegah user menginput data yang salah sebelum disimpan ke dalam database.

### METHOD

```
@api.multi
@api.constrains(
    {nama_field:str},
    ...
)
def {nama_method}(self):
```

### KETENTUAN STANDAR

* Nama method diawali dengan **_check**.
* Perlu menggunakan looping recordset

<script
  type="text/javascript"
  src="https://cdn.jsdelivr.net/npm/gist-embed@1.0.4/dist/gist-embed.min.js"
></script>

### CONTOH KODE

* **Deskripsi:** Tanggal mulai tidak boleh lebih besar dari tanggal selesai
* **Field:** date_start, date_end

<code data-gist-id="b3d6176a3e7fb91891d868722c22aedd"></code>
