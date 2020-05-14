# Broken

Smell ini mirip sama smell nya martin fowler yaitu [Data Class](https://sourcemaking.com/refactoring/smells/data-class) dan [Feature Envy](https://sourcemaking.com/refactoring/smells/feature-envy)

### Masalah utama:

1. Belum biasa ngoding OOP, terbiasa Procedural
2. Baru masuk ke project besar. Lalu ga sempet baca semua kegunaan fungsi yang udah ada, developer malah buat class lagi

### Solusi:

Hapus hubungan Has-A terharap data class tersebut, lalu pindahin members dari data class tersebut

### When to ignore:
- Code auto generate
- Data Transfer Object 
    - Ini penampung dari banyaknya gabungan class lain. Biasanya cuma berisi setter, getter, parser (ex : json to array)


