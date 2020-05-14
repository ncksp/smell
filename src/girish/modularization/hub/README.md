# Hub-Like

Smell ini terjadi kalo ada abstraction yang punya dependencies nya kebanyakan yang masuk / keluar (fan in / fan out)

### Penyebab:

1. Abstraction terlalu banyak tugas melanggar SRP 
2. Masukin semua helper kedalam 1 class

### Solusi:

1. Apakah banyak tugas ? jika iya di extract class
2. Apa ada member (field /  method) yang salah tempat, lakuin extract method