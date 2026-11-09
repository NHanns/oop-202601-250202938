# Catatan Minggu 02: Struktur OOP : Class, Object, Encapsulation

## Yang saya kerjakan

Pada minggu 2, saya melengkapi class `Aset.java` dengan menerapkan konsep encapsulation. Saya membuat field `kode`, `nama`, `status`, dan `kondisi` menjadi private. Saya juga melengkapi konstruktor, getter, setter, serta validasi agar data aset tidak menerima nilai yang tidak sesuai ketentuan.

## Keputusan desain

- Field `kode` dan `nama` tidak boleh bernilai null atau kosong.
- Status awal aset adalah `TERSEDIA`.
- Kondisi awal aset adalah `BAIK`.
- Field `kode` tidak memiliki setter agar kode aset tidak dapat diubah setelah objek dibuat.
- Setter status dan kondisi menolak nilai null.
- Validasi menggunakan `trim().isEmpty()` untuk memeriksa teks kosong, tetapi nilai asli tetap disimpan tanpa menghapus spasi atau mengubah huruf menjadi kapital.

## Kendala

Kendala yang saya temui adalah memahami validasi pada konstruktor dan setter serta memastikan setiap field memiliki akses yang sesuai. Saya mengatasinya dengan memeriksa kembali aturan pada dokumen Minggu 2 dan menjalankan pengujian menggunakan Maven.

## Penggunaan AI

- **Alat yang dipakai:** ChatGPT.
- **Bagian yang dibantu AI:** Implementasi field, konstruktor, getter, setter, dan validasi pada class `Aset.java`.
- **Prompt utama:** Membantu melengkapi class `Aset.java` sesuai aturan pada dokumen Minggu 2, termasuk validasi kode, nama, status, dan kondisi.
- **Yang saya ubah atau tolak dari saran AI, dan alasannya:** Saya menggunakan validasi `trim().isEmpty()` tanpa mengubah nilai asli yang disimpan karena tidak ingin melakukan normalisasi data.
- **Satu hal yang saya pahami lebih baik sekarang:** Encapsulation digunakan untuk membatasi akses langsung ke field dan mengatur perubahan data melalui method yang telah diberi validasi.