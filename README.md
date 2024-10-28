# Init
![](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/init.jpeg?raw=true)
Pada bagian init, dipanggil beberapa method berupa `InitEnvironment`, `InitMaulidzar`, dan `InitObstacle`, di mana masing-masingnya memiliki kegunaan masing-masing. Namun sebelum ke penjelasan dari tiap method, terdapat beberapa logika yang juga dipanggil langsung di method init ini, yaitu mapping untuk menangani input dari user, berupa tombol space dan esc.


### - InitEnvironment()
![](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/init_environment.jpeg?raw=true)
Pada method ini, berisi tentang logika yang berkaitan tentang inisiasi environment dari game, yaitu parallax scrolling pada background untuk game.

### - InitMaulidzar()
![](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/init_maulidzar.jpeg?raw=true)
Lalu pada method ini, akan dilakukan inisiasi untuk karakter yang akan digunakan di game.

### - InitObstacle()
![](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/init_obstacle.jpeg?raw=true)
Pada method ini, digunakan untuk menginisiasi obstacle yang akan di gunakan dalam game, yang mana pada game ini adalah berupa kaktus.

# Draw

![](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/draw.jpeg?raw=true)setelah dilakukan inisiasi terhadap semua kebutuhan dalam game, maka selanjutnya adalah melakukan rendering terhadap semua yang sudah kita inisiasi sebelumnya.

### - RenderEnvironment()
![enter image description here](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/render_environment.jpeg?raw=true)
pada method ini, akan dilakukan rendering terhadap semua sprites yang digunakan sebagai parallax scrolling.

### - RenderMaulidzar()
![enter image description here](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/render_maulidzar.jpeg?raw=true)
Hanya berisi seperti di atas, karena karakter kita hanya satu.

### - RenderObstacle()
![enter image description here](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/render_obstacle.jpeg?raw=true)
Pada method ini, hanya dilakuka render pada spritesObstacle, karena obstacle yang kita miliki hanya berupa satu macam saja.

# Update
![enter image description here](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/update.jpeg?raw=true)
Bagian terakhir adalah tentang update, di mana di sini akan dihandle logika tentang bagaimana game akan berjalan dan apabila kalah. 

### - CalculateScore()
![enter image description here](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/calculate_score.jpeg?raw=true)
Di sini juga dipanggil method `CalculateScore()`, yang gunanya adalah menghitung score, sehingga setiap kali iterasi gameloop, akan ditambahkan poin.

### - CollisionDetection()
![enter image description here](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/collision_detector.jpeg?raw=true)
Pada method ini digunakan untuk mendeteksi apakah karakter mengenai kaktus atau tidak. 

# Physic
![enter image description here](https://github.com/fahmigutawan/fahmigutawan.github.io/blob/main/assets/jump_physic.jpeg?raw=true)
Secara fisik, maka ada beberapa logika yang harus ditangani, termasuk bagaimana logika dari melompat dapat diterapkan pada game ini. Untuk itu, maka digunakan method `JumpPhysic()` untuk mendeteksi dalam setiap iterasi, bahwa jika menekan tombol tertentu maka akan terjadi lompatan pada karakter yang dimainkan.
