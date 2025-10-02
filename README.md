# Lab2web
<p>Nama : Muflih Salda Maulana</p>
<P>Nim  : 312410527</P>
<p>Kelas: TI.24.A5 </p>

1. Membuat Dokumen HTML

Buat file baru lab2_css_dasar.html dengan struktur dasar HTML.

<img width="936" height="433" alt="coding praktikum2 1" src="https://github.com/user-attachments/assets/1486339c-8366-4b20-aaab-298900b330c5" />


📸 Screenshot hasil tampilan awal

<img width="1348" height="413" alt="praktimu 2 web 1" src="https://github.com/user-attachments/assets/6be50272-b9db-4202-8c24-d07d8e002e96" />


2. Menambahkan Internal CSS

Tambahkan CSS pada bagian <head>:

<img width="1005" height="436" alt="coding praktikum2  2" src="https://github.com/user-attachments/assets/93e19f3f-624c-43c0-ba8f-539b9a5f216b" />


📸 Screenshot setelah menggunakan Internal CSS

<img width="1365" height="582" alt="praktikum2 web 2" src="https://github.com/user-attachments/assets/ec2f32b8-ef98-4740-a4ce-00dd0754fba2" />


3. Menambahkan Inline CSS

Tambahkan pada elemen <p>:

<img width="683" height="371" alt="image" src="https://github.com/user-attachments/assets/176475ba-46c6-471c-a5bf-bea45915aca3" />



📸 Screenshot hasil Inline CSS

<img width="681" height="478" alt="image" src="https://github.com/user-attachments/assets/ff18cc93-61cc-4bb0-a6ef-25fcfcbd1fd7" />



4. Membuat Eksternal CSS

Buat file baru style_eksternal.css:

<img width="403" height="264" alt="coding css eksternal 3 " src="https://github.com/user-attachments/assets/04d722a4-ed1f-476e-839d-a0e28387b50e" />


Tambahkan pada file HTML:

<img width="645" height="57" alt="menyisipkan css eksternal 3" src="https://github.com/user-attachments/assets/a86d78f4-f7f7-4e4c-a821-1ffa10f9b8a5" />



📸 Screenshot hasil setelah menggunakan eksternal CSS

<img width="1365" height="552" alt="image" src="https://github.com/user-attachments/assets/3446e3bc-dfa7-4180-b52d-b04e0296a0fa" />




5. Menambahkan CSS Selector

Edit style_eksternal.css:

<img width="414" height="329" alt="menambahkan id selector 4" src="https://github.com/user-attachments/assets/0f0cd778-e2b0-4f2c-b08c-9f3ce6e4c86e" />


📸 Screenshot hasil ID & Class Selector

<img width="1360" height="555" alt="image" src="https://github.com/user-attachments/assets/a7978fe4-ca5c-42c7-a749-43a2bf8b82cb" />

# Pertanyaan

1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.

2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
penjelasannya!

4. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
penjelasan dan contohnya!

6. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )



# **Jawaban Pertanyaan**

## **1. Eksperimen dengan CSS**

Kode awal:

```css
h1 {
    color: blue;
}
```

Hasil eksperimen dengan menambahkan properti:

```css
 h1 {
    color: rgb(209, 34, 11);                  /* Warna teks */
    font-size: 32px;              /* Ukuran huruf */
    text-align: center;           /* Rata tengah */
    background-color: #fa8d08;    /* Latar belakang */
    padding: 15px;                /* Jarak dalam */
    border-radius: 50px;           /* Sudut melengkung */
    box-shadow: 10px 10px 30px rgb(22, 7, 7); /* Bayangan */
}
```

Teks `<h1>` tampil lebih menarik dengan ukuran besar, background oren, dan efek bayangan.

<img width="1360" height="555" alt="image" src="https://github.com/user-attachments/assets/057c5b3d-c95c-4a31-8976-7bb3d190da7b" />


## **2. Perbedaan `h1 {...}` dengan `#intro h1 {...}`**

* **`h1 {...}`** → berlaku untuk semua elemen `<h1>` di halaman.
* **`#intro h1 {...}`** → berlaku hanya untuk `<h1>` di dalam elemen dengan `id="intro"`.

**Contoh:**

```html
<div id="intro">
    <h1>Judul di Intro</h1>
</div>
<h1>Judul Biasa</h1>
```

```css
h1 {
    color: blue;   /* Semua h1 biru */
}
#intro h1 {
    color: yellow;    /* Tapi h1 di dalam #intro jadi kuning */
}
```

Hasil: judul biasa = biru, judul dalam intro = kuning.

<img width="673" height="102" alt="image" src="https://github.com/user-attachments/assets/1010c8c5-12bf-41aa-b344-8e51a47dc33b" />


## **3. Prioritas CSS (Inline, Internal, Eksternal)**

Urutan prioritas CSS jika konflik:

1. **Inline CSS** → tertinggi
2. **Internal CSS (`<style>`)**
3. **Eksternal CSS (`style.css`)** → terendah

**Contoh:**

<head>
    <!-- CSS Eksternal -->
    <link rel="stylesheet" href="style.css">

    <!-- CSS Internal -->
    <style>
        p {
            text-align: justify;
            color: red;
            font-size: 18px;
        }
    </style>
</head>
<body>
    <header>
        <h1>CSS Internal dan <i> inline CSS</i></h1>
    </header>
    <nav>
        <a href="lab2_css_dasar.html">CSS Dasar</a>
        <a href="lab2_css_eksternal.html">CSS Eksternal</a>
        <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>

    <!-- Inline CSS -->
    <p style="text-align: center; color: #ccd8e4;">
        Ini adalah teks tambahan dengan style inline
    </p>
</body>


Misalkan di style.css (eksternal) ada aturan:

p {
  color: blue;
  text-align: left

**Hasil yang muncul di browser:**

Eksternal (style.css) → p { color: blue; text-align: left; }

Internal (style di <head>) → p { color: red; text-align: justify; }

Inline (style langsung di tag <p>) → style="text-align: center; color: #ccd8e4;"

**Karena inline CSS lebih spesifik, maka yang ditampilkan adalah:**

text-align: center; (inline menang melawan justify dan left)

color: #ccd8e4; (inline menang melawan red dan blue)

font-size: 18px; (hanya ada di internal, jadi tetap berlaku)
## **4. ID vs Class (Spesifisitas CSS)**

### Urutan kekuatan CSS (specificity):

1. **Inline CSS** → paling kuat
2. **ID Selector** (`#id`)
3. **Class Selector** (`.class`)
4. **Tag Selector** (`p, h1, div`)

---

### Contoh:

```html
<p id="paragraf-1" class="text-paragraf" style="color: green;">
    Ini adalah paragraf percobaan
</p>
```

CSS:

```css
/* Class */
.text-paragraf {
    color: blue;
}

/* ID */
#paragraf-1 {
    color: red;
}
```

Hasil yang muncul di browser: **warna hijau**

* Karena **inline style** (style="color: green;") mengalahkan ID dan class.

Kalau **tanpa inline style**:

* Warna **merah** (karena ID `#paragraf-1` lebih kuat daripada class `.text-paragraf`).

**Inline > ID > Class > Tag**
* Jadi yang dipakai tergantung siapa yang lebih kuat.


 Kesimpulan

CSS memiliki tiga cara penulisan: inline, internal, eksternal.

Selector digunakan untuk mengatur elemen secara spesifik (elemen, class, id).

Prioritas CSS: Inline > ID > Class > Elemen > Eksternal.

Dengan CSS, tampilan web menjadi lebih menarik, terstruktur, dan konsisten.
