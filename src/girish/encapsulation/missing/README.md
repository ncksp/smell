# Missing 
Smell ini mirip sama punya fowler, Switch Statement dan Parallel Inheritance Hierarchies
Smell ini ada 2 kondisi :
### 
1. Client tau kalo service nya punya banyak variasi jadi client harus tau ini fitur baru atau ini fitur lama tapi harus diubah
2. Setiap mau nambah fitur baru kita harus bikin class baru juga 

### Cara Mendeteksi
**OCP (Open Close Principle)** class harus open for extension dan close for modification