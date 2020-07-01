# Unfactored

Smell ini mirip Duplicate Code milik Martin Fowler

Ada beberapa kemungkinan :

1. Duplikasi terjadi di class turunannya

    Penyelesaian : buat abstract class di parent
2. Duplikasi terjadi di class parent dan children

    Penyelesaian : hapus duplikat di children
3. Interface yang duplicate -> signature (implementasi beda)
    
    Penyelesaian : cukup buat abstarct method aja di parent
4. Implementasi sama
    
    Penyelesaian : langsung buat method konkrit di parent nya
5. Gabungan antara interface duplikat dan implementasi sama
    
    Penyelesaian : pindahin langsung ke parent
