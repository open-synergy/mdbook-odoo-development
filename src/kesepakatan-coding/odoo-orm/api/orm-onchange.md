# Onchange

API Onchange digunakan untuk memberikan nilai kepada field(***Tujuan***) ketika ada field(***Sumber***) yang diubah.

### METHOD

```
@api.onchange(
    {nama_field_sumber:str},
    ...
)
def {nama_method}(self):
```

### KETENTUAN STANDAR

* Nama method diawali dengan **onchange_{nama_field_tujuan}**.
* Onchange dibuat per 1 field.
* Tidak perlu menggunakan looping recordset, karena **self** pada onchange sudah merujuk record pada form itu sendiri.

<script
  type="text/javascript"
  src="https://cdn.jsdelivr.net/npm/gist-embed@1.0.4/dist/gist-embed.min.js"
></script>

### CONTOH KODE

* **Deskripsi:** Data partner dan user akan terisi sesuai dengan nilai partner dan user pada type
* **Field Sumber:** type_id
* **Field Tujuan:** partner_id, user_id <br/>

<code data-gist-id="f54c6631f28b84a2b94a2fa143890c82"></code>
