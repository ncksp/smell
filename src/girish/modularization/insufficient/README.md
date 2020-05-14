# Insufficient
Smell ini punya 2 masalah yaitu:
1. Bloated interface -> Smell ini mirip sama punya martin fowler yaitu [Large Class](https://sourcemaking.com/refactoring/smells/large-class)
2. Bloated Implementation -> abstraksi yang punya banyak method yang diimplementasikan atau punya satu atau lebih method dengan Excessive Implementation Complexity


## Excessive Implementation Complexity

Berbeda sama Complexity biasanya (Time / Space) yang biasanya ngitung performa, kalau ini menghitung **Code Complexity**

Ada beberapa cara mengukurnya salah satunya adalah [Cyclomatic Complexity](https://en.wikipedia.org/wiki/Cyclomatic_complexity), rumus pertama yaitu rumus nya McCabe

Ada beberapa rumus :

```
Rumus Dasar :
    M = E - N + 2P

Funsi Rekursif :
    M = E - N + P

1 Subroutine/Method:
    M = E - N + 2

E = Jumlah garis / egde tiap graph
N = Jumlah node graph
P = Connected component 
```