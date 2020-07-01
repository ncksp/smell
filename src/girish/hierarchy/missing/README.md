# Missing

Smell ini mirip sama kayak Switch Statement. hanya ada hal spesifik yaitu ada behavior yang bisa ditaro di parent karna kesalahan dalam design

### Masalah
Terdapat method/member yang sama antara class satu dengan yang lain. Tetapi tidak dibuatkan parent / abstract class 

### Solusi
Buat abstract class untuk menampung kedua method/member yang sama tersebut **(jika memiliki behavior yang sama)**