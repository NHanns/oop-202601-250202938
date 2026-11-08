# Catatan Minggu 01: Paradigma Pemrograman dan Setup

## Yang saya kerjakan

Pada minggu pertama, saya menyiapkan lingkungan pemrograman Java menggunakan JDK 21, Maven, Git, dan Visual Studio Code. Saya mengerjakan tiga contoh program dengan paradigma prosedural, OOP, dan fungsional. Ketiga program dibuat agar menghasilkan sapaan yang memuat nama, NIM, dan nama sistem Aset-Pinjam. Setelah selesai, saya menjalankan pengujian menggunakan script `uji.ps1` dan seluruh pengujian berhasil.

## Keputusan desain

Saya menggunakan bentuk sapaan yang sama pada ketiga program, yaitu "Hello Aset-Pinjam, saya [nama] ([NIM])", agar perbedaan ketiga paradigma dapat dilihat dari cara penulisan programnya.

- **Prosedural:** Menggunakan metode statis `sapa()` untuk menghasilkan sapaan.
- **OOP:** Menggunakan field `private` untuk menyimpan nama dan NIM, kemudian menghasilkan sapaan melalui metode `sapa()`.
- **Fungsional:** Menggunakan lambda yang dikembalikan oleh metode `pembuatSapaan()` untuk menghasilkan sapaan berdasarkan nama yang diberikan.

## Kendala

Awalnya saya perlu memahami struktur folder project dan menemukan file Java yang harus dikerjakan. Saya juga perlu memahami perbedaan cara kerja ketiga paradigma pemrograman. Kendala tersebut saya atasi dengan memeriksa struktur project, membaca instruksi pada setiap file, dan mencoba menjalankan pengujian. Setelah perbaikan selesai, seluruh 5 pengujian Minggu 1 berhasil dijalankan tanpa kegagalan.

## Penggunaan AI

- Alat yang dipakai: ChatGPT.
- Bagian yang dibantu AI: `HelloProsedural.java`, `HelloOOP.java`, `HelloFungsional.java`, serta arahan pengisian catatan Minggu 1.
- Prompt utama:
  1. Membantu mengerjakan bagian TODO pada ketiga file Java Minggu 1.
  2. Menjelaskan cara menemukan dan mengedit file pada struktur project di VS Code.
  3. Membantu menjalankan dan memahami hasil pengujian menggunakan `uji.ps1`.
- Yang saya ubah atau tolak dari saran AI, dan alasannya: Saya menyesuaikan nama dan NIM yang digunakan agar sesuai dengan identitas saya. Tidak ada saran kode utama yang saya tolak.
- Satu hal yang saya pahami lebih baik sekarang: Saya memahami bahwa paradigma prosedural menggunakan fungsi atau metode, OOP menggabungkan data dan perilaku dalam class, sedangkan paradigma fungsional dapat menggunakan lambda dan fungsi sebagai nilai.