# 1. Single Page Aplication
SPA adalah aplikasi web yang berisi HTML yang kontennya terus diupdate saat user berinteraksi tanpa harus refresh (Rizqy, 2020). Perbedaannya dengan aplikasi web tradisional : 
- web tradisional : setiap interaksi artinya meminta server untuk mengirimkan suatu halaman baru secara penuh, membuat layar loading dulu.
- SPA : Browser menggunakan JavaScript untuk mengubah tampilan secara instan tanpa memuat ulang halaman.
- Keuntungan :
    - Pengalaman yang lebih baik bagi pengguna karena tidak ada loading-loading
    - Bisa menyimpan data lokal dengan baik untuk penggunaan offline
- Kerugian :
    - Saat pertama kali dibuka, lumayan lambat karena harus meng-load semuanya dulu
    - Pengoptimalan sulit
- sumber : https://www.codepolitan.com/blog/apa-itu-spa-single-page-application/

# 2. Service dalam Backend
Service dalam konteks backend adalah suatu lapisan yang berisi logika bisnis dari aplikasi. Service bertindak sebagai perantara yang memisahkan antara Controller/Route (yang menangani permintaan HTTP) dan Data Access/Repository (yang berhubungan dengan database).
Peran Service dalam Modularitas :
- Dengan memindahkan logika ke service, route hanya fokus pada ke-valid-an input dan pengiriman respon, sehingga service bisa fokus mau diapakan datanya
- dapat menggunakan logika yang sama untuk dipanggil kembali
- bisa melakukan unit testing tanpa harus menjalankan server
sumber : https://www-coursera-org.translate.goog/articles/back-end-developer?_x_tr_sl=en&_x_tr_tl=id&_x_tr_hl=id&_x_tr_pto=sge 

