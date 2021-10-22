# Konfirmasi Ketika Klik Tombol

Setiap tombol harus memiliki dialog konfirmasi ketika diklik.

### KETENTUAN STANDAR

* Konfirmasi dibuat hanya untuk tombol-tombol yang mengubah **State/Workflow**
* Untuk tombol-tombol yang membuka **window action** dikecualikan
* Pesan konfirmasi = "**{state}** Data. Are you sure?"

<script
  type="text/javascript"
  src="https://cdn.jsdelivr.net/npm/gist-embed@1.0.4/dist/gist-embed.min.js"
></script>

### CONTOH KODE KONFIRMASI TOMBOL DIGUNAKAN

<code data-gist-id="9bd75e4e7697fbff622cb51f2c0d8e7f" data-gist-highlight-line="6,14,22" data-gist-line="1-24"></code>

### CONTOH KODE KONFIRMASI TOMBOL TIDAK DIGUNAKAN

<code data-gist-id="9bd75e4e7697fbff622cb51f2c0d8e7f" data-gist-line="26-56"></code>
