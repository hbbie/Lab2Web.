# Lab2Web.
Tugas Pertemuan 3
# Nama      : Dhani Naufal Habibie
# Kelas     : TI.24.A4
# NIM       : 312410300

# Langkah 1
Membuat dokumen HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CSS Dasar</title>
</head>
<body>
<header>
<h1>CSS Internal dan <i>Inline CSS</i></h1>
</header>
<nav>
<a href="lab2_css_dasar.html">CSS Dasar</a>
<a href="lab2_css_eksternal.html">CSS Eksternal</a>
<a href="lab1_tag_dasar.html">HTML Dasar</a>
</nav>
<!-- CSS ID Selector -->
<div id="intro">
<h1>Hello World</h1>
<p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
dan CSS.</p>
<!-- CSS Class Selector -->
<a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
</div>
</body>
</html>
```
<img width="1845" height="661" alt="image" src="https://github.com/user-attachments/assets/f868ae86-6bda-46b4-a762-3a546e6e11be" />

# Langkah 2

Mendeklarasikan CSS Internal

Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen.
``` html
<title>CSS Dasar</title>
<style>
body {
font-family:'Open Sans', sans-serif;
}
header {
min-height: 80px;
border-bottom:1px solid #77CCEF;
}
h1 {
font-size: 24px;
color: #0F189F;
text-align: center;
padding: 20px 10px;
}
h1 i {
color:#6d6a6b;
}
</style>
</head>
```

<img width="1919" height="954" alt="image" src="https://github.com/user-attachments/assets/de84fb6b-0be4-4892-82cc-5c6e0c61abee" />

# Langkah 3
Kemudian tambahkan deklarasi inline CSS pada tag <p> seperti berikut.
``` html
<p style="text-align: center; color: #ccd8e4;">
```
simpan lalu refresh
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/2490121e-1d27-45ed-b2d2-740d5191740e" />

# Langkah 4
Membuat CSS Eksternal

Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.
``` html
nav {
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
}
```
Kemudian tambahkan tag <link> untuk merujuk file css yang sudah dibuat pada bagian <head>

``` html
<head>
<!-- menyisipkan css eksternal -->
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>

```
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/dc36de54-4b61-4970-a41f-e96a86338d1b" />

# Langkah 5
Menambahkan CSS Selector

Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
style_eksternal.css, tambahkan kode berikut.

``` html
/* ID Selector */
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
}
```
<img width="1918" height="992" alt="image" src="https://github.com/user-attachments/assets/68d4a1cb-a9b6-4774-8c3a-4c30d071fdf1" />






