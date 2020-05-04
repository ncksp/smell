# Deficient

smell ini terjadi kalo akses modifier kebutuhannya itu private tapi dibuat public atau sebaliknya

### Penyebab
1. **Easier testability**: Buat ngetest unit testing biar gampang jadi di set semua ke public tapi lupa kalo bakalan jadiin smell.
    #### Solusi
        - Kalo mau ngetest diusahain jangan ngetest langsung method private, sekiranya mau dipake masukin aja ke method public
        - Atau pake fungsi reflection dari unit testing nya
2. **Procedural thinking in object oriented context**:  Pemahaman tentang oop nya kurang jadi masih terbiasa code procedural

3. **Quick Fix Solutions**:  Developer dikejer deadline jadi buru buru asal selesai aja