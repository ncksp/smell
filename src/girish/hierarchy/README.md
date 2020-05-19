# Hierarchy

- Hierarchy Intro | [Link Video](https://www.youtube.com/watch?v=FvLtPJzya5o&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)
- [Missing Hierarchy](missing) | [Link Video](https://www.youtube.com/watch?v=Z0gVvdARFWw&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)
- [Unnecessary Hierarchy](unnecessary) | [Link Video](https://www.youtube.com/watch?v=hfNd8QPcWDk&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)
- [Unfactored Hierarchy](unfactored) | [Link Video](https://www.youtube.com/watch?v=IJFO8YlSosc&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)
- [Wide Hierarchy](wide) | [Link Video](https://www.youtube.com/watch?v=7pyZYGDz54w&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)
- [Speculative Hierarchy](speculative) | [Link Video](https://www.youtube.com/watch?v=WaI-tpREgd8&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)

Dalam OOP ada 2 jenis hierarchy
1. Type hierarchy  -> is-a
2. Object hierarchy -> part-of (has-a / part-of)
    ```
    Bedanya antara has-a dan part-of adalah
    - has-a itu aggregate
    - part-of itu composisition

    contoh composition:
        
        class A{
            B b;
        }

    Ketika A dihapus maka B akan otomatis kehapus, sebaliknya jika aggregate A dihapus maka B tidak akan dihapus
    ```

Teknik untuk mencapat hierarchy yang baik

1. Apply meaningful classification (Missing, Unnecessary)
    -> cari hal yang sama antara children, ketika ada yang sama maka ditaro ke parent (implementasi harus beda)

2. Apply meaningful generalization (Unfactored, Wide, Speculative, Deep)
    -> sama kayak meaning classification

3. Ensure substitutability (Rebellious, Broken)
    -> pakai teknik Liskov Segregation Principle, mirip smell Request Bequest martin fowler

4. Avoid redundant paths (Multipath)
    -> salah extend
    ```
    misalkan ada class D extend C dst
    A <---
    |    |
    B    |
    |    |
    C    |
    |    |
    D >---

    lalu tiba2 D juga melakukan extends ke A, berlaku juga untuk implements
    ```
5. Ensure proper ordering (Cyclic)
    -> pastikan order nya benar, tidak melanggar Dependencies Invarian Principle
---

Repository ini hanyalah rangkuman dari buku Suryanarayana et al. dengan sedikit tambahan informasi lain. Diharapkan mahasiswa juga membaca sumber aslinya pada bab 6 halaman 123 - 192.