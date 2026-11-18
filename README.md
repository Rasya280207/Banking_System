Penjelasan Konsep OOP pada Kode di Atas:
Encapsulation (__saldo dan __pin): Saldo dan PIN diawali dengan dua garis bawah (__), artinya variabel tersebut bersifat privat dan tidak bisa diubah sembarangan dari luar class (misalnya akun1.__saldo = 99999999 akan menghasilkan error). Harus melalui method resmi seperti setor(), tarik(), atau get_saldo().

Inheritance (AkunTabungan & AkunBisnis mewarisi AkunBank): Class anak menggunakan kembali sifat-sifat umum dari class induk (AkunBank) tanpa harus menulis ulang kode untuk fungsi setor atau tarik.

Polymorphism (cek_info): Baik AkunTabungan maupun AkunBisnis memiliki fungsi bernama sama (cek_info), namun perilakunya berbeda dan disesuaikan dengan jenis akun masing-masing.

Abstraction (ABC & @abstractmethod): Mencegah pembuatan objek langsung dari class AkunBank secara sembarangan, serta mewajibkan setiap jenis akun baru untuk memiliki fungsi cek_info().