# PANDUAN INTEGRASI SHOPEE AFFILIATE (SHITNYATA)

Fitur ini memungkinkan Anda menampilkan "Kartu Rekomendasi Produk" di akhir artikel secara otomatis.

---

## Cara Penggunaan

Setiap kali Anda membuat artikel baru (file `.md` di folder `_posts`), Anda cukup menambahkan data produk di bagian **Front Matter** (bagian paling atas yang diapit garis `---`).

### Format Kode

Copy-paste kode berikut ke bagian atas artikel Anda:

```yaml
---
layout: post
title: "Judul Artikel Anda"
date: 2025-12-22 10:00:00 +0700
categories: [Kategori]
affiliate:
  product_name: "Tulis Nama Produk Di Sini"
  image_url: "Paste Link Gambar Produk (Shopee/Google)"
  product_link: "Paste Link Affiliate Shopee Anda"
---
```

### Penjelasan Field

1.  **`product_name`**:
    *   Nama produk yang akan muncul sebagai judul kartu.
    *   *Contoh:* "Buku Filosofi Teras"

2.  **`image_url`**:
    *   Link langsung ke gambar produk.
    *   *Cara mudah:* Klik kanan gambar di Shopee -> "Copy Image Address".
    *   *Contoh:* `https://cf.shopee.co.id/file/....`

3.  **`product_link`**:
    *   Link affiliate khusus punya Anda (bisa link custom atau universal link).
    *   *Contoh:* `https://shopee.co.id/universal-link/...`

---

## Pertanyaan Umum (FAQ)

**Q: Bagaimana jika saya tidak mengisi data affiliate?**
A: Tidak masalah. Fitur ini bersifat opsional. Jika Anda tidak menulis bagian `affiliate:` sama sekali, kartu produk tidak akan muncul dan halaman artikel tetap terlihat rapi.

**Q: Apakah bisa untuk Tokopedia/Lazada?**
A: Bisa! Meskipun saya menamakannya "Racun Shopee", secara teknis ini hanya link tombol. Anda bisa memasukkan link Tokopedia/TikTok Shop di `product_link`, dan card akan tetap berfungsi mengarahkan ke sana.
