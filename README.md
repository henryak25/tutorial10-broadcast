# Experiment README
## Experiment 2.1: Original code, and how it run
![Alt text](run.png)
Untuk menjalankan server dan tiga client, maka buka terminal dan jalankan perintah cargo run --bin server untuk memulai server. Server lalu akan mendengarkan connection pada port 2000. Setelah server berjalan, buka tiga terminal lain untuk client dan jalankan perintah cargo run --bin client di masing-masing terminal untuk menjalankan tiga instance client secara paralel.<br><br>

Pada screenshot di atas, terlihat bahwa server berhasil menerima koneksi dari tiga client (127.0.0.1 dengan port berbeda), lalu masing-masing client mengirim pesan seperti "client 1 here", "client 2 here", dan "client 3 here". Pesan-pesan ini kemudian diteruskan kembali oleh server ke seluruh client yang sedang terhubung, yang ditandai dengan munculnya output seperti from server client 2 here di client lainnya.