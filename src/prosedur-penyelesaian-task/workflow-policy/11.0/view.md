# View

View yang perlu ditambahkan adalah sbb:

<script
  type="text/javascript"
  src="https://cdn.jsdelivr.net/npm/gist-embed@1.0.4/dist/gist-embed.min.js"
></script>

#### 1. Tambahkan/modifikasi attributes pada setiap button policy.

> Ketentuan Standar:
> * Apabila perlu dilakukan modifikasi, hilangkan attribute **states** pada view.
> * Pengisian Attibutes = "{'invisible':[('{**policy_field**}','=',False)]}"
> * Sesuaikan **policy_field** dengan button yang berkaitan.

CONTOH KODE:

<code data-gist-id="82b13762aa7809e32d62b3dc007b3733" data-gist-highlight-line="6,13,20,27,34,42" data-gist-line="23-65"></code>

#### 2. Pada notebook, tambahkan page polices

CONTOH KODE:

<code data-gist-id="82b13762aa7809e32d62b3dc007b3733" data-gist-line="105-119"></code>
