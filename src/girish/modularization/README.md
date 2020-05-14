# Modularization

- Modularization Intro | [Link Video](https://www.youtube.com/watch?v=Q5Y42rdZza4&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)
- [Broken Modularization](broken) | [Link Video](https://www.youtube.com/watch?v=0aeIbhESMco&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)
- [Insufficient Modularization](insufficient) | [Link Video](https://www.youtube.com/watch?v=eRAoks2udlk&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)
- [Cyclically-dependent Modularization](cyclic) | [Link Video](https://www.youtube.com/watch?v=Xm5T75YZB0I&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)
- [Hub-like Modularization](hub) | [Link Video](https://www.youtube.com/watch?v=ImUM8T-1fy4&list=PLG_Cu5FmqSk2KHT6lXngRvcOmOzuk4_ju)

---

```
Modularization adalah gimana caranya buat 1 class abstaction dengan coupling dan cohesion yang sebaik mungkin

Akan susah dibaca jika code tidak dibuat localization dan decomposition
```
---

Modularization berlaku disemua paradigma bahasa pemgrograman, tapi karna **OOP maka modularization yang dimaksud adalah level class**.

Ada 4 teknik untuk mencapai goal
1. Localize related data and method ->
    ``Dimana data dan method dijadiin 1 (punya tanggung jawab yang sama``
2. Decompose abstraction to manageable size ->
    ``Mecah abstraction yang gede menjadi kecil tapi jangan jadi terlalu kecil dan jangan terlalu kecil``  
3. Create acyclic dependencies ->
    `` Jangan buat class terlalu cyclic (hubungannya muter A->B->D->E->C->A)``
4. Limit dependencies
   ``Rendah terhadap fan-in dan fan-out`` 

        - Fan In
            Banyak yang make method dikelas itu. Tapi bisa jadi nilai tambah karna class itu misalkan class helper atau emang banyak dipake. Itu ga masalah
        - Fan Out 
            Terlalu banyak make method dikelas lain


Ada 4 Smell dari kategori ini yang tiap-tiap smell nya merusak dari 4 teknik tersebut

1. Broken -> Localize
2. Insufficient -> Decompose abstraction
3. Cyclic -> Create acyclic
4. Hub-like -> Limit dependencies

---
---


Repository ini hanyalah rangkuman dari buku Suryanarayana et al. dengan sedikit tambahan informasi lain. Diharapkan mahasiswa juga membaca sumber aslinya pada bab 5 halaman 93 - 122.