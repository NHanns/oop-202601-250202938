# Minggu 4: Polymorphism

## Ringkasan
Pada minggu keempat, saya mempelajari konsep polymorphism dalam Java melalui method overriding dan overloading. Implementasi dilakukan pada class Aset beserta subclass-nya dan class KatalogAset.

## Pekerjaan yang Dilakukan

1. **Overriding pada class Ruang**
   - Mengimplementasikan method `hitungDenda(int)`.
   - Denda dihitung berdasarkan jumlah hari keterlambatan dikalikan tarif dasar.

2. **Overriding pada class Laptop**
   - Mengimplementasikan method `hitungDenda(int)`.
   - Menggunakan pengali denda 2 kali tarif dasar.

3. **Overriding pada class AlatLab**
   - Mengimplementasikan method `hitungDenda(int)`.
   - Menggunakan pengali denda 4 kali tarif dasar.

4. **Overloading pada class KatalogAset**
   - Membuat method `cari(String kata)` untuk mencari aset berdasarkan nama tanpa membedakan huruf besar dan kecil.
   - Membuat method `cari(String kata, JenisAset jenis)` untuk mencari aset berdasarkan nama dan jenis aset tertentu.

## Aturan Denda
Tarif dasar denda dibaca dari `Varian.aktif().dendaPerHari`.

- Ruang: 1 kali tarif dasar.
- Laptop: 2 kali tarif dasar.
- AlatLab: 4 kali tarif dasar.
- Keterlambatan 0 hari menghasilkan denda 0.
- Jumlah hari negatif menghasilkan `IllegalArgumentException`.

## Pengujian
Pengujian dilakukan menggunakan perintah:

`.\scripts\uji.ps1 -Minggu 4`

Hasil pengujian:
- Week 1: 5 tes berhasil.
- Week 2: 6 tes berhasil.
- Week 3: 8 tes berhasil.
- Week 4: 8 tes berhasil.
- Total: 27 tes.
- Failures: 0.
- Errors: 0.
- Skipped: 0.

Hasil akhir: **BUILD SUCCESS**.

## Penggunaan AI
Saya menggunakan ChatGPT sebagai alat bantu untuk memahami konsep polymorphism, membantu implementasi method overriding pada subclass Ruang, Laptop, dan AlatLab, serta membuat dua method overloading pada KatalogAset. Saya juga menggunakan ChatGPT untuk membantu memeriksa hasil pengujian dan memahami aturan implementasi.

## Kesimpulan
Melalui tugas minggu keempat, saya memahami penggunaan overriding untuk memberikan perilaku berbeda pada subclass dan overloading untuk menyediakan beberapa method dengan nama sama tetapi parameter berbeda. Seluruh 27 pengujian berhasil dijalankan tanpa kegagalan.