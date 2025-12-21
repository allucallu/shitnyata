# PANDUAN PASANG IKLAN (SHITNYATA)

Dokumen ini berisi cara memasang iklan (Google AdSense, Adsterra, dll) di template ini tanpa harus pusing coding.

Sudah disiapkan 2 "Slot Khusus" untuk Anda.

---

## 1. Iklan Otomatis / Pop-Up / Script Utama
Biasanya penyedia iklan (AdSense/Adsterra) meminta Anda menaruh kode `<script>` di dalam bagian `<head>` situs.

*   **File yang diedit:** `_includes/ads-head.html`
*   **Caranya:**
    1.  Buka file `_includes/ads-head.html`.
    2.  Hapus semua teks panduan di dalamnya (opsional).
    3.  **Paste** script iklan Anda di situ.
    4.  Save.

*Contoh isi file nanti:*
```html
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXX" crossorigin="anonymous"></script>
```

---

## 2. Iklan Banner di Sidebar (Kotak Kanan)
Untuk mengganti iklan palsu "Jual Ginjal" dengan iklan banner asli (ukuran 300x250 biasanya).

*   **File yang diedit:** `_includes/ads-sidebar.html`
*   **Caranya:**
    1.  Buka file `_includes/ads-sidebar.html`.
    2.  **Hapus** seluruh kode `div class="fake-ad-widget" ...` (blok iklan palsu).
    3.  **Paste** kode banner HTML dari penyedia iklan di situ.
    4.  Save.

---

## 3. Iklan di Dalam Artikel (Manual)
Jika Anda ingin menyisipkan iklan di tengah-tengah tulisan (misal setelah paragraf 1).

*   **File yang diedit:** File postingan Anda (misal: `_posts/2025-12-20-judul.md`)
*   **Caranya:**
    Cukup paste kode iklan langsung di antara paragraf tulisan Anda.

    *Contoh:*
    ```markdown
    Paragraf pertama tulisan anda bla bla bla.

    <!-- Paste Kode Iklan Disini -->
    <div id="iklan-tengah">...</div>

    Paragraf kedua lanjut bla bla bla.
    ```

---

## CATATAN PENTING
*   **Waktu Tayang**: Setelah dipasang, kadang iklan butuh waktu 1-24 jam untuk muncul (terutama AdSense baru).
*   **Localhost**: Iklan biasanya **TIDAK MUNCUL** saat Anda preview di komputer sendiri (`localhost`). Upload dulu ke GitHub/Cloudflare baru cek di HP/Browser lain.
