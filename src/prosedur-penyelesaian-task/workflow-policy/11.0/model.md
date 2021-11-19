# Model

Pada model, ada beberapa hal yang perlu dilakukan:

<script
  type="text/javascript"
  src="https://cdn.jsdelivr.net/npm/gist-embed@1.0.4/dist/gist-embed.min.js"
></script>

#### 1. Inherit model mixin.policy

CONTOH KODE:

<code data-gist-id="d3543c33d1466d772b04beb562b1ce48" data-gist-highlight-line="5" data-gist-line="9-15"></code>

#### 2. Override method _compute_policy

CONTOH KODE:

<code data-gist-id="d3543c33d1466d772b04beb562b1ce48" data-gist-highlight-line="1-4" data-gist-line="53-56"></code>

#### 3. Menambahkan field policy

> Ketentuan Standar:
> * Penamaan field = **{nama_button}_ok** (*Huruf kecil semua*)
> * Type field = ***Computed Fields*** dengan tipe data ***Boolean***

CONTOH KODE:

<code data-gist-id="d3543c33d1466d772b04beb562b1ce48" data-gist-line="58-86"></code>

#### 4. Menambahkan method **_get_template_id**

Method **_get_template_id** ini berfungsi untuk mencari template yang sesuai dengan kriteria. <br/>
Pengisian **template_id** sangat dibutuhkan untuk menentukan isian dari **field policy** yang sudah dibuat pada langkah sebelumnya.

> Note:
> Trigger dari method ini disesuaikan dengan skenario yang diinginkan, bisa diletakkan ketika **on_change**,**create**, dst

CONTOH KODE:

**Scenario**: Trigger pada saat **on_change**

<code data-gist-id="d3543c33d1466d772b04beb562b1ce48" data-gist-highlight-line="5" data-gist-line="134-140"></code>
