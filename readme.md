![](docs/run1server3client.png)

Di sini, klien melakukan koneksi ke server melalui WebSocket di Rust. Jika salah satu klien mengirim pesan ke server, server akan membalas pesan
tersebut kepada semua koneksi WebSocket yang terhubung.

![](docs/perubahan-pada-server.png)
Saya mengubah port dari 2000 ke 8080 pada server
![](docs/perubahan-pada-client.png)
Saya turut mengubah port dari 2000 ke 8080 pada client
![](docs/setelahgantiport.png)
Program tetap berjalan dengan baik karena server dan client memiliki protokol TCP yang sama
dan terkoneksi pada address yang sama dengan port yang sama.
![](docs/kode-tambahkan-asal.png)
![](docs/kode-tambahkan-ip.png)
![](docs/tambahkan-ip.png)
Selanjutnya saya menambahkan ip asal client pada pesan
yang dikirimkan oleh server.
