**Nama  :** Jordan Frisay Himawan <br>
**NRP   :** 3122600007 <br>
**Kelas :** 2 D4 IT A <br>

`Tugas ini merupakan tugas mata kuliah Konsep Jaringan yang dibimbing oleh Bpk. Dr. Ferry Astika Saputra, ST, M.Sc`

# TCP 3-Way Handshake Process

#### :bulb: Apa Itu Three-Way Handshake?
Sebuah proses yang digunakan oleh protokol TCP/IP untuk membuat sebuah koneksi antara server dan client, Disebut Three-Way karena proses ini memang terdiri dari 3 langkah.3 langkah proses tersebut membutuhkan server dan client untuk bertukar synchronization dan acknowledgement sebelum proses komunikasi dengan data asli dimulai.

![7 OSI Layer](./assets/establish.png)

Three-Way Handshake dirancang sedemikian rupa untuk membantu menginisiasi, negosiasi, dan memisahkan koneksi TCP pada waktu yang sama. 

#### :memo: Pesan Pada Three-Way Handshake
| **Pesan**             | **Deskripsi**                                       |
|-----------------------|-----------------------------------------------------|
| SYN (Synchronize)     | Digunakan untuk menginisiasi dan establish koneksi. |
| ACK (Acknowledgement) | Membantu konfirmasi SYN pada server atau client.    |
| SYN-ACK               | Membuat SYN dan melakukan ACK pada segment.         |
| FIN                   | Untuk mengakhiri koneksi.                            |

#### :memo: Proses Three-Way
- Pada step pertama, client melakukan establishment koneksi dengan server. Dengan cara mengirimkan segment berisi SYN.
- Pada step kedua, server merespon request client dengan mengirimkan segment berisi SYN-ACK set. ACK berarti server telah menerima request dari client, dan SYN menandakan digit sequence yang akan dikirimkan pada segment berikutnya.
- Pada step ketiga, setelah client acknowledge terhadap respon dari server maka client dan server membuat koneksi yang stabil dan memulai proses transfer data asli.

Proses diatas merupakan langkah-langkah yang terjadi pada proses establishment, selanjutnya adalah proses data transfer dan connection termination.

Pada dasarnya step yang terjadi sama, hanya saja pada proses data transfer akan terdapat data asli pada segment yang dikirimkan. Sedangkan pada proses termination client dan server menggunakan FIN-ACK.