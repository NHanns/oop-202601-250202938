# Catatan Minggu 03: Inheritance (Pewarisan)

## Yang saya kerjakan

Pada minggu 3, saya menerapkan konsep inheritance pada class aset. Saya melengkapi tiga subclass, yaitu `Ruang`, `Laptop`, dan `AlatLab` yang mewarisi class `Aset`. Saya juga menambahkan field, konstruktor, getter, validasi, dan override method `getJenis()` pada masing-masing subclass.

## Keputusan desain

- Semua field tambahan dibuat private untuk menerapkan encapsulation.
- Konstruktor setiap subclass memanggil `super(kode, nama)` untuk menggunakan validasi dari class induk `Aset`.
- Kapasitas ruang harus lebih dari 0.
- Spesifikasi dan nomor inventaris laptop tidak boleh null atau kosong.
- Laboratorium tidak boleh null atau kosong dan tingkat risiko tidak boleh null.
- Method `getJenis()` dioverride sesuai jenis aset masing-masing.

## Kendala

Kendala yang saya temui adalah memahami hubungan antara class induk dan subclass serta penggunaan `super()` dan `@Override`. Saya mengatasinya dengan mempelajari struktur class dan menjalankan pengujian khusus Minggu 3.

## Penggunaan AI

- **Alat yang dipakai:** ChatGPT.
- **Bagian yang dibantu AI:** Implementasi class `Ruang.java`, `Laptop.java`, dan `AlatLab.java`.
- **Prompt utama:** Membantu melengkapi ketiga subclass sesuai aturan pada dokumen Minggu 3.
- **Yang saya ubah atau tolak dari saran AI, dan alasannya:** Saya mengikuti validasi menggunakan `trim().isEmpty()` tanpa mengubah nilai asli yang disimpan agar konsisten dengan implementasi Minggu 2.
- **Satu hal yang saya pahami lebih baik sekarang:** Inheritance memungkinkan subclass mewarisi atribut dan perilaku dari class induk, sedangkan overriding memungkinkan subclass menyediakan implementasi method sendiri.