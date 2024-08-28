# TokoShop Telegram bot ppob dan topup game
Toko shop, awalnya merupakan program untuk jualan yang di pesan oleh berbagai orang. Per pesanan di hargai 250rb - 350rb, pengembangan proyek terganggu di karenakan biaya yang di bayarkan kurang. Walaupun sudah banyak yang berkontribusi membayar jasa untuk project ini, tapi pengembanganya terus masih belum usai. Sejak Era QR payment Elma ID.

Fitur awal hanya di khususkan untuk menjual akun Premium, E-Book Novel, Lisensi Software, Documents, Arsip, Video Footage, Art, dan karya digital lain. Dengan mengungsung konsep sistem cerdas yaitu cek pembayaran otomatis. Karena cuma buat jual produk digital, pryek nampak kurang menarik, dan gak semua orang punya produk digital mereka.

Update pembaruhan akhirnya di tambah dengan fitur PPOB ( Payment Online Bank ), fitur ini meramaikan jumlah produk yang dapat di jual dari bot telegram toko shop. Ukuran program juga makin besar, awlanya saya mau melisensikan untuk di jual secara source program. Tapi ketika melihat versi sebelumnya, di mana saya pernah jual source program dan di jual ulang oleh orang lain, jadi untuk menjual source di batalkan.

Bot ini mempunyai konfigurasi yang rumit, jadi gak semua orang bisa menjalankan program. Salah setting bisa gak work alias gak jalan program nya. Butuh integrasi ke layanan payment gateway, digiflazz, linkqu atau server pulsa lain. Juga butuh akses ke server VPS untuk dapat installasi mandiri. Jadi bot ini saya jadikan sebagai SaaS, gak perlu repot setup server dan konfigurasi sana sini.

Dan saya udah mengupdate banyak fitur dan bug dari bot ini. Beberapa perbaikan akan saya sebutkan di sini secara satu persatu, dan inilah yang membuat proyek ini jadi bernilai lebih. Versi update sudah di 6.1, saya masih kesulitan untuk mendistribusikan kode ke banyak program yang udah berjalan, karena kalau server di off kan semua jadi terganggu.

Beberapa perbaikan tidak saya tulis tanggalnya karena wkatu kerja juga gak nyatet. Release sekarang :

1. Perbaikan fitur, Owner bot bisa menambahkan margin keuntungan sendiri per SKU produk selain  menggunakan pendekatan harga otomatis by kategori.
2. Perbaikan fitur TOKO : Katalog di hilangkan di ganti kategori, penambahan parameter harga beli, dan penggunaan fitur stock per sku.
3. Penambahan list daftar server id ( khusus produk netzku pulsa ), tujuanya agar penggguna yang membeli produk topup game bisa memilih server secara langsung.
4. Perbaikan desain halaman dashboard panel, agar menampilkan angka yang penting contoh saldo digiflazz, saldo netzku, dan omzet selama 12 bulan tarkhir.
5. Perbaikan halaman management user untuk mencegah kebingungan, jika owner bot mengurangi atau menambah saldo user maka akan dapat notif di telegram.
6. Perbaikan halaman riwayat transaksi, kalau sebelumnya di pisah kini jadi satu dashboard tunggal bisa memilih  filter by Digiflazz/Netzku Pulsa/Produk Toko
7. Penambahan payment gateway eksternal yang dapat digunakan langsung selain tripay yaitu TOKOPAY.
8. Halaman deposit member sebelumnya berisi invoice, kini sudah menampilkan jumlah dana yang tersedia di akun member untuk mencegaah pencurian dana. Dan catatan jumlah yang di belanjakan member/volume trx 12 bulan terakhir.
10. Halaman riwayat saldo netzku di edit, ini untuk memungkinkan pengguna agar bisa menggunakan saldo netzku untuk membeli suplier pulsa ke 2.
11. Program afffiliate untuk produk ini di turunkan jadi 5% dan harga produk dari awalnya 35rb di turunkan jadi 25 ribu ( hanya instalasi saja )
12. Perubahan pada nama perintah sebelumnya kelolah toko jadi Managements
13. Penambahan fitur untuk download rekapan dari bot, hanya untuk download rekapan bulan ini via perintah Rekapan
14. Update perbaikan ID, sebelumnya ada celah bug jika SSID bot kalian kesebar orang lain bahkan bisa masuk ke dashboard dengan akun mereka. Walau gak bisa transaksi tetep aja bisa lihat riwayat dashborad botmu.
15. Perbaikan inkonsistensi history saldo, riwayat saldo di catat secara penuh karena sebelumnya hanya di catat apabila transaksi berhasil. Tapi akibat delay proses yang lama membuat urutan data gak konsisten.
16. Sekarang transaksi reffund akan ada catatan historycal saldo nya untuk lebih waspada terhadap pengurangan dan catatan yang gak konsisten.
