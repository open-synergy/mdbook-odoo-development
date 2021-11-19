# Model

Pada model, ada beberapa hal yang perlu dilakukan:

<script
  type="text/javascript"
  src="https://cdn.jsdelivr.net/npm/gist-embed@1.0.4/dist/gist-embed.min.js"
></script>

#### 1. Inherit model mixin.sequence

CONTOH KODE:

<code data-gist-id="1db60e9542024fbf3b26480ae11df29e" data-gist-highlight-line="4" data-gist-line="9-15"></code>

#### 2. Menambahkan method **_create_sequence**

Method **_create_sequence** ini berfungsi untuk meng-*generate* sequence sesuai dengan template yang dibuat. <br/>

> Note:
> Trigger dari method ini disesuaikan dengan skenario yang diinginkan, bisa diletakkan ketika **action**,**create**, dst

CONTOH KODE:

**Scenario**: Trigger pada saat **create**

<code data-gist-id="1db60e9542024fbf3b26480ae11df29e" data-gist-highlight-line="5,8" data-gist-line="174-184"></code>
