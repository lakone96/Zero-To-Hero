# selector { property : value;}

# 1. Cara menulis CSS Eksternal

---

- CSS yang ditulis dalam file terpisah (.css)
- Sebenarnya ada 3 cara menulis CSS yaitu `Inline`, `Internal`, dan `Eksternal`
- Namun yang lebih disarankan yaitu `Eksternal`
- Dihubungkan ke HTML dengan tag `<link>` yang disimpan sebelum tag tutup `</body>`
- -**`<link rel="stylesheet" href="style.css">`**- `style.css` adalah nama file css pada umumnya

- Keuntungan CSS Eksternal:

- Dapat digunakan di banyak halaman
- Kode lebih terorganisir
- Loading lebih cepat (browser cache)

# 2. Selektor CSS

selector { property : value;}

- Selector adalah elemen html yang akan dipilih atau diubah style nya(`<header>`,`<main>`,dll)
- selector bisa menggunakan elemen html, class, atau id agar lebih spesifik

## 3. Jenis-Jenis Selektor Dasar

**Selector berdasarkan `element`, `class`, dan `id`**

```css
/* Memilih berdasarkan elemen <p> */
p {
  font-size: 16px;
}

/* Memilih semua elemen berdasarkan class="warning" */
.warning {
  color: red;
  font-weight: bold;
}

/* Memilih elemen dengan id="header" */
#header {
  background-color: lightblue;
  padding: 20px;
}
```

### 4. Properti Teks dan Valuenya

**`color` - Warna Teks**

```css
p {
  color: red; /* Nama warna */
  color: #ff0000; /* HEX color */
  color: rgb(255, 0, 0); /* RGB color */
  color: rgba(255, 0, 0, 0.5); /* RGB dengan transparansi */
}
```

**`font-size` - Ukuran Font**

```css
p {
  font-size: 16px; /* Pixels (tetap) */
  font-size: 1em; /* Relatif terhadap font parent */
  font-size: 1.5rem; /* Relatif terhadap root element */
  font-size: 100%; /* Persentase */
  font-size: large; /* Kata kunci (small, medium, large) */
}
```

**`font-weight` - Ketebalan Font**

```css
p {
  font-weight: normal; /* Normal (400) */
  font-weight: bold; /* Tebal (700) */
  font-weight: lighter; /* Lebih tipis */
  font-weight: bolder; /* Lebih tebal */
  font-weight: 600; /* Numeric (100-900) */
}
```

**`font-style` - Gaya Font**

```css
p {
  font-style: normal; /* Normal */
  font-style: italic; /* Miring (cursive) */
  font-style: oblique; /* Miring (slant) */
}
```

**`text-align` - Perataan Teks**

```css
p {
  text-align: left; /* Rata kiri (default) */
  text-align: right; /* Rata kanan */
  text-align: center; /* Rata tengah */
  text-align: justify; /* Rata kiri-kanan */
}
```
