# Praktikum 2 - Pemrograman Web

```
Fitrah Rizki Ardiansyah
311910465
TI.19.A.2
```
# LANGKAH 1
## Membuat dokumen HTML dengan nama file lab2_css_dasar.html. Setelah itu buat struktur dasar HTML dan masukan coding nya.
```
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
![image](https://user-images.githubusercontent.com/56240954/115667675-5012b500-a370-11eb-88dd-7a171724ae9f.png)

# LANGKAH 2
## Mendeklarasikan CSS Internal dibagian ```<head>```.
```
<head>
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
![image](https://user-images.githubusercontent.com/56240954/115667831-7d5f6300-a370-11eb-8e24-72602e5851e1.png)

# LANGKAH 3
## Menambahkan deklarasi Inline CSS pada tag ```<p>``` dibawah H1.
  ```
  <p style="text-align: center; color: #ccd8e4;">
  ```
  ![image](https://user-images.githubusercontent.com/56240954/115668306-273eef80-a371-11eb-8966-1b2642f8cbf4.png)
  
# LANGKAH 4
## Buat file baru dengan nama style_eksternal.css kemudian buat deklarasi CSS
```
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
![image](https://user-images.githubusercontent.com/56240954/115668587-7ab13d80-a371-11eb-9bca-ab4f42b91e34.png)

# LANGKAH 5
## Tambahkan tag ```<link>``` untuk merujuk file css yang sudah dibuat pada bagian ```<head>``` pada ```lab2_css_dasar.html```

<head>
    <!-- menyisipkan css eksternal -->
    <link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
![image](https://user-images.githubusercontent.com/56240954/115668764-b3511700-a371-11eb-8b31-a588133d1010.png)

# LANGKAH 6
## Tambahkan CSS Selector menggunakan ID dan Class Selector. Pada file ```style_eksternal.css```
```
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
![image](https://user-images.githubusercontent.com/56240954/115668963-f1e6d180-a371-11eb-9fbd-153ec6c3a415.png)

# TUGAS
# 1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
Saya bereksperimen menambahkan background dan mengubah warna pada button
TUGAS 1 CSS
![image](https://user-images.githubusercontent.com/56240954/115669408-6d488300-a372-11eb-9ff3-ea9fb7d076db.png)
![image](https://user-images.githubusercontent.com/56240954/115669550-923cf600-a372-11eb-9637-bde4c61f0bd8.png)

# 2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!
Pendeklarasian CSS elemen h1 mengubah tampilan seluruh elemen yang memiliki tag h1, jika #intro h1 hanya mengubah tampilan elemen h1 yang memiliki id #intro.
# 3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
jika mendeklarasikan CSS pada elemen yang sama namun isi deklarasi nya berbeda, maka semua deklarasi CSS tersebut akan ditampilkan.
![image](https://user-images.githubusercontent.com/56240954/115670016-260ec200-a373-11eb-8465-347f74b54d8c.png)

    
   


