# Lab2Web : Praktikum Dasar CSS

Repositori ini berisi latihan dan tugas yang telah diselesaikan sebagai bagian dari **Lab 2: CSS Dasar** untuk mata kuliah Pemrograman Web di **Universitas Pelita Bangsa**. Praktikum ini mencakup dasar-dasar penggunaan CSS, seperti penerapan CSS internal, eksternal, dan inline, serta penggunaan selector, properti, dan nilai CSS.

## Daftar Isi
1. [Pendahuluan](#pendahuluan)
2. [Langkah-langkah](#langkah-langkah)
   - [Langkah 1: Membuat Dokumen HTML](#langkah-1-membuat-dokumen-html)
   - [Langkah 2: Menambahkan CSS Internal](#langkah-2-menambahkan-css-internal)
   - [Langkah 3: Menambahkan CSS Inline](#langkah-3-menambahkan-css-inline)
   - [Langkah 4: Menambahkan CSS Eksternal](#langkah-4-menambahkan-css-eksternal)
   - [Langkah 5: Menggunakan Selector CSS](#langkah-5-menggunakan-selector-css)
3. [Hasil Eksperimen](#hasil-eksperimen)
4. [Kesimpulan](#kesimpulan)
5. [Tangkapan Layar](#tangkapan-layar)

---

## Pendahuluan

Tujuan dari praktikum ini adalah untuk memperkenalkan dasar-dasar CSS kepada mahasiswa. Dengan latihan ini, mahasiswa akan mempelajari cara menggunakan CSS secara internal, eksternal, dan inline, serta bagaimana memilih elemen HTML yang akan diubah tampilannya menggunakan berbagai jenis selector CSS.

## Langkah-langkah

### Langkah 1: Membuat Dokumen HTML
### Langkah 1: Membuat Dokumen HTML
Langkah pertama adalah membuat struktur dasar HTML seperti berikut:

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
    <div id="intro">
        <h1>Hello World</h1>
        <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah Pemrograman Web.</p>
        <a class="button btn-primary" href="#intro">Informasi selengkapnya</a>
    </div>
</body>
</html>
```
### Langkah 2: Menambahkan CSS Internal
Selanjutnya, tambahkan CSS internal di dalam tag `<head>`:

```html
<style>
    body {
        font-family: 'Open Sans', sans-serif;
    }
    header {
        min-height: 80px;
        border-bottom: 1px solid #77CCEF;
    }
    h1 {
        font-size: 24px;
        color: #0F189F;
        text-align: center;
    }
    h1 i {
        color: #6d6a6b;
    }
</style>
```

### Langkah 3: Menambahkan CSS Inline
CSS inline diterapkan langsung di elemen `<p>`:

```html
<p style="text-align: center; color: #ccd8e4;">Teks ini diatur menggunakan CSS inline.</p>
```

### Langkah 4: Menambahkan CSS Eksternal
Buat file eksternal (`assets/css/style.css`) dan hubungkan ke dokumen HTML:

```html
<link rel="stylesheet" href="assets/css/style.css" type="text/css">
```

Isi dari `assets/css/style.css`:

```css
nav {
    background: #20A759;
    color: #fff;
    padding: 10px;
}

nav a {
    color: #fff;
    text-decoration: none;
    padding: 10px 20px;
}

nav a:hover {
    background: #0B6B3A;
}
```

### Langkah 5: Menggunakan Selector CSS
Gunakan selector CSS seperti ID dan class:

```html
#intro {
    background: #418fb1;
    padding: 10px;
}

.button {
    padding: 15px 20px;
    background: #bebcbd;
    color: #fff;
}

.btn-primary {
    background: #E42A42;
}
```
---
## Screenshot
1. **Tampilan Sebelum CSS Diterapkan:**
   - Tangkapan layar ini menunjukkan tampilan dasar halaman HTML sebelum ada gaya CSS yang diterapkan.
     
![star 1](https://github.com/user-attachments/assets/10fc6b4e-43ab-4425-88c9-c58d42f7fb56)
![star 1 2](https://github.com/user-attachments/assets/ac986bc6-00ca-4f3e-a991-c977b11f2ddd)

2. **Tampilan Dengan CSS Internal dan Inline:**
   - Tangkapan layar ini menunjukkan perubahan tampilan setelah CSS internal dan inline diterapkan, seperti perubahan warna teks dan tata letak.

![star 2](https://github.com/user-attachments/assets/88f5f24a-56a5-4fd5-b4dc-0ed5d8020acf)
![star 2 1](https://github.com/user-attachments/assets/54dcf69d-2a52-4f77-8e3c-62e83b5ec01a)

3. **Tampilan Setelah Menambahkan CSS Eksternal:**
   - Di tangkapan layar ini, file CSS eksternal telah diterapkan, sehingga gaya pada navigasi dan elemen lainnya menjadi lebih terstruktur.

![star 4 1](https://github.com/user-attachments/assets/bc25368a-92c9-44ad-988b-0b178cb30359)
![star 4 2](https://github.com/user-attachments/assets/63e5e39e-9551-4e79-a86d-43949a24ceba)
![star 4 3](https://github.com/user-attachments/assets/69b25c8d-3d78-48d4-80b2-06a252e9d7c6)

4. **Tampilan Final Setelah Semua CSS Diterapkan:**
   - Ini adalah hasil akhir setelah semua jenis CSS (internal, inline, dan eksternal) diterapkan, termasuk penggunaan selector ID, class, dan elemen.

![star 5 2](https://github.com/user-attachments/assets/cb16a50e-b7b5-4215-a41c-afbd22190628)
![star 5 1](https://github.com/user-attachments/assets/a427da9e-6d06-4aa1-8ead-d71198e5d50e)

---
## Hasil Eksperimen
1. **Perbedaan Selector Elemen (`h1 {...}`) vs. Selector ID (`#intro h1 {...}`):**
   - Selector elemen menerapkan gaya ke semua elemen `<h1>`, sedangkan selector ID hanya akan mempengaruhi elemen `<h1>` di dalam elemen dengan ID `#intro`.

2. **Urutan Prioritas CSS Internal, Eksternal, dan Inline:**
   - Jika ketiga jenis CSS ini diterapkan pada elemen yang sama, **inline CSS** memiliki prioritas tertinggi, diikuti **CSS eksternal**, dan terakhir **CSS internal**. Misalnya:

```html
<h1 style="color: red;">Judul ini akan berwarna merah karena CSS inline.</h1>
```

3. **Prioritas Selector ID dan Class:**
   - Selector ID memiliki prioritas lebih tinggi dibandingkan selector class, karena ID lebih spesifik.

```html
<p id="paragraf-1" class="text-paragraf">Gaya teks akan mengikuti selector ID.</p>
```

## Kesimpulan
Praktikum ini memberikan pengalaman dalam menggunakan berbagai metode deklarasi CSS dan menunjukkan bagaimana aturan CSS diterapkan dengan berbagai selector dan urutan prioritasnya.

---
