# Lab2web
1. Membuat Dokumen HTML

Buat file baru lab2_css_dasar.html dengan struktur dasar HTML.

<img width="936" height="433" alt="coding praktikum2 1" src="https://github.com/user-attachments/assets/1486339c-8366-4b20-aaab-298900b330c5" />


📸 Screenshot hasil tampilan awal

<img width="1348" height="413" alt="praktimu 2 web 1" src="https://github.com/user-attachments/assets/6be50272-b9db-4202-8c24-d07d8e002e96" />


2. Menambahkan Internal CSS

Tambahkan CSS pada bagian <head>:



📸 Screenshot setelah menggunakan Internal CSS



3. Menambahkan Inline CSS

Tambahkan pada elemen <p>:

<p style="text-align: center; color: #ccd8e4;">
    Ini adalah contoh paragraf dengan Inline CSS
</p>


📸 Screenshot hasil Inline CSS


<img width="1365" height="582" alt="praktikum2 web 2" src="https://github.com/user-attachments/assets/7e10b57f-2284-4041-8ca8-cfc23274fde9" />


4. Membuat Eksternal CSS

Buat file baru style_eksternal.css:

<img width="403" height="264" alt="coding css eksternal 3 " src="https://github.com/user-attachments/assets/04d722a4-ed1f-476e-839d-a0e28387b50e" />


Tambahkan pada file HTML:

<img width="645" height="57" alt="menyisipkan css eksternal 3" src="https://github.com/user-attachments/assets/a86d78f4-f7f7-4e4c-a821-1ffa10f9b8a5" />



📸 Screenshot hasil setelah menggunakan eksternal CSS

<img width="1365" height="537" alt="praktikum2 web 4" src="https://github.com/user-attachments/assets/1b8c85a1-54b4-4412-9cce-3200c6bab44a" />


5. Menambahkan CSS Selector

Edit style_eksternal.css:

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


📸 Screenshot hasil ID & Class Selector

❓ Pertanyaan

Apa perbedaan h1 {..} dengan #intro h1 {..}?

h1 {..} → berlaku untuk semua elemen <h1>.

#intro h1 {..} → hanya berlaku untuk <h1> yang ada di dalam elemen dengan id="intro".

Jika ada internal, eksternal, dan inline CSS pada elemen yang sama, mana yang ditampilkan?

Browser akan mengutamakan Inline CSS → Internal CSS → Eksternal CSS (berdasarkan urutan prioritas CSS).

Jika satu elemen memiliki ID dan Class, deklarasi mana yang ditampilkan?

ID Selector lebih spesifik dibanding Class, sehingga ID lebih diutamakan.

Contoh:

<p id="paragraf-1" class="text-paragraf">Contoh teks</p>

📌 Kesimpulan

CSS memiliki tiga cara penulisan: inline, internal, eksternal.

Selector digunakan untuk mengatur elemen secara spesifik (elemen, class, id).

Prioritas CSS: Inline > ID > Class > Elemen > Eksternal.

Dengan CSS, tampilan web menjadi lebih menarik, terstruktur, dan konsisten.
