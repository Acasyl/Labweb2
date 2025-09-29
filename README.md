## Nama :Syalsha Putri ichwani
## NIM  :312410209

1. pertama gambar terlihat kosong.
<img width="1918" height="1024" alt="Cuplikan layar 2025-09-29 143141" src="https://github.com/user-attachments/assets/3de90156-3f90-4a9e-9472-6baac89e35bf" />

 2.langkah Kemudian tambahkan deklarasi inline CSS pada tag <p> seperti berikut.
`<p style="text-align: center; color: #ccd8e4;">`
 Simpan kembali dan refresh kembali browser untuk melihat perubahannya.
 
<img width="1903" height="692" alt="Cuplikan layar 2025-09-29 133754" src="https://github.com/user-attachments/assets/e91a4cf0-7d9d-428e-86a2-1ca852eca4ec" />

3. Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.
`nav {
background: #20A759;
color:#fff;
padding: 10px;
}
nav a {
color: #fff;
text-decoration: none;
padding:10px 20px;
}
nav .active,
nav a:hover {
background: #0B6B3A;
}`
Kemudian tambahkan tag `<link>` untuk merujuk file css yang sudah dibuat pada bagian `<head>`
`<head>`
<!-- menyisipkan css eksternal -->
`<link rel="stylesheet" href="style_eksternal.css" type="text/css">`
`</head>`

Selanjutnya refresh kembali browser untuk melihat perubahannya. 
<img width="1911" height="1025" alt="Cuplikan layar 2025-09-29 141043" src="https://github.com/user-attachments/assets/b3078a66-2968-461d-8a82-5a5e1d42ea82" />


Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
style_eksternal.css, tambahkan kode berikut.

`/* ID Selector */
#intro {
background: #418fb1;
border: 1px solid #099249;
min-height: 100px;
padding: 10px;
}
#intro h1 {
text-align: left;
border: 0;
color: #fff;
}
/* Class Selector */
.button {
padding: 15px 20px;
background: #bebcbd;
color: #fff;
display: inline-block;
margin: 10px;
text-decoration: none;
}
.btn-primary {
background: #E42A42;
}`

Kemudian simpan kembali dan refresh browser untuk melihat perubahannya.

<img width="1913" height="565" alt="Cuplikan layar 2025-09-29 143753" src="https://github.com/user-attachments/assets/b47d60e3-5667-40bf-ac33-a6e8924faece" />














# Soal-Soal
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
penjelasannya!

jawabannya:
CSS pada elemnt h1 ini merujuk langsung ke element h1 dalam file, sehingga semua tag h1 akan mengikuti intruksi css dari h1, sedangkan #intro h1 akan merujuk ke semua element h1 yang berada dalam div #intro

3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
penjelasan dan contohnya!

 jawabannya :
Inline CSS didahulukan karena tingkat prioritas (specificity), bukan karena waktu browser merender HTML lebih dulu. Browser tetap menggabungkan semua aturan CSS (eksternal, internal, inline) lalu memilih yang paling kuat sesuai CSS Cascade

4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )

Jawabannya:
Selector dari ID lebih kuat dibandingkan selector dari class, oleh karna itu deklarasi css menggunakan id akan lebih didahulukan dibanding menggunakan class`
