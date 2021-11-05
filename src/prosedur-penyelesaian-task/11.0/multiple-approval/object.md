# Object

Pada object, ada beberapa hal yang perlu dilakukan:

<script
  type="text/javascript"
  src="https://cdn.jsdelivr.net/npm/gist-embed@1.0.4/dist/gist-embed.min.js"
></script>

#### 1. Inherit object mixin.multiple_approval

CONTOH KODE:

<code data-gist-id="1aa3d12f80697c9d468fab692a82783b" data-gist-highlight-line="5" data-gist-line="8-14"></code>

#### 2. Sesuaikan variable \_approval\_

Default variable yang tersedia:

* _approval_state_field = "state" <br/>
Isi variable **\_approval\_state\_field** dengan nama field **state**

* _approval_state = "confirm" <br/>
Isi variable **\_approval\_state** dengan value statenya (cth: draft,confirm,dst) <br/>
***Variable ini menentukan ketika di state mana approval akan dilakukan.***

* _approval_from_state = "draft" <br/>
Isi variable **\_approval\_from\_state** dengan value statenya (cth: draft,confirm,dst) <br/>
***Variable ini menentukan state sebelum approval dilakukan.***

* _approval_to_state = "confirm" <br/>
Isi variable **\_approval\_to\_state** dengan value statenya (cth: draft,confirm,dst) <br/>
***Variable ini menentukan state setelah approval dilakukan.***

* _approval_cancel_state = "cancel" <br/>
Isi variable **\_approval\_cancel\_state** dengan value statenya (cth: draft,confirm,dst) <br/>
***Variable ini menentukan state yang digunakan untuk cancel.***

* _approval_reject_state = "reject" <br/>
Isi variable **\_approval\_reject\_state** dengan value statenya (cth: draft,confirm,dst) <br/>
***Variable ini menentukan state yang digunakan untuk reject.***


CONTOH KODE:

<code data-gist-id="1aa3d12f80697c9d468fab692a82783b" data-gist-highlight-line="8-10" data-gist-line="8-17"></code>

#### 3. Override method approval

Tambahkan method **action_request_approval()**, pada method action sesuai dengan isi dari variable **\_approval\_state** <br/>

CONTOH KODE:

Isi dari variable **\_approval\_state** = "confirm" <br/>
Maka kita perlu menambahkan method **action_request_approval()** pada method action dari state **confirm**

<code data-gist-id="1aa3d12f80697c9d468fab692a82783b" data-gist-highlight-line="4" data-gist-line="53-56"></code>

#### 4. Override method **action_approve_approval**

Override method **action_approve_approval** dan tambahkan method action sesuai dengan isi dari variable **\_approval\_to\_state** <br/>

CONTOH KODE:

Isi dari variable **\_approval\_to\_state** = "open" <br/>
Maka kita perlu menambahkan method **action_open()** pada method **action_approve_approval**

<code data-gist-id="1aa3d12f80697c9d468fab692a82783b" data-gist-highlight-line="6" data-gist-line="74-79"></code>
