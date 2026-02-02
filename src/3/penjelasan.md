# a. Artifical Potential Field (APF)
APF adalah metode navigasi yang dimiliki sebuah robot di mana metode yang digunakan adalah menjadikan target seperti gaya tarik, dan obstacle sebagai gaya tolak. Semakin jauh benda dari target, semakin besar gaya tariknya, dan semakin dekat benda dengan obstacle, semakin besar gaya dorongnya. Bisa dibayangkan dengan sebuah bola (robot) yang bergerak disuatu bidang. Dalam bidang tersebut ada lembah (target) dan ada gunung (obstacle). Bola akan bergerak menuju lembah dan tidak akan memanjat gunung, melainkan menghindarinya. 
- Gambar diagram
![Gambar Diagram](../../assets/Artificial%20Potential%20Field.jpeg)
- sumber : https://www.google.com/url?sa=i&source=web&rct=j&url=https://ejournal.sultanpublisher.com/index.php/ijec/article/download/117/55&ved=2ahUKEwjh8ZyW3rqSAxXJUGwGHZfAE70QqYcPegQIAhAD&opi=89978449&cd&psig=AOvVaw1dA1DvO_lrYoXK0LCfzN6p&ust=1770119241832000

# b. Uniform Cost Search (UCS), Greedy Best First Search (GBFS), dan A* Search
1. Uniform Cost Search (UCS)
- Algoritma yang mengecek semua jalan dan menentukan jalan mana yang costnya paling murah
- Cara kerja: Cari jalan dengan biaya bensin paling sedikit dari start
- Kelebihan : Pasti ketemu jalan yang termurah 
- Kekurangan : dicobain semua, jadinya lama 
- Situasi : Jika biaya jalur bervariasi dan tidak tersedia informasi tambahan tentang setiap jalurnya

2. Greedy Best First Search (GBFS)
- hanya peduli pada seberapa dekat posisi saat ini dengan tujuan berdasarkan perkiraan
- cara kerja : tarik garik lurus ke tujuan, pokoknya cari jalan yang paling lurus
- Kelebihan : Paling efisien dan menjamin solusi optimal selama fungsi heuristik yang digunakan bersifat admissible (tidak pernah melebih-lebihkan biaya)
- Kekurangan: Mengonsumsi banyak memori karena harus menyimpan semua node yang diekspansi dalam daftar
Situasi Cocok: Ketika kecepatan adalah yang utama tanpa memerdulikan kualitas jalur

3. A* Search
- Menggunakan keunggulan dari UCS dan GBFS. 
- Cara kerja : Dengan cara melihat biaya perjalanan, tetapi juga melihat jarak terdekat
- Keunggulan : cepat dan murah
- Kekurangan: Butuh banyak "catatan" di memori untuk menghitung kombinasi tersebut
- Situasi : Standar utama untuk navigasi real-time, seperti pada sistem GPS

Sumber : https://ursinus-cs477-f2023.github.io/CoursePage/ClassExercises/Week3_PrioritySearch/#:~:text=Today%20we%20discussed%20a%20set,the%20goal%20to%20the%20solution

