# TCP/IP (Transmission Control Protocol/Internet Protocol)
---

#### :bulb: Apa Itu TCP/IP?
TCP/IP adalah standar komunikasi data yang digunakan oleh komunitas internet dalam proses tukar-menukar data dari satu komputer ke komputer lain di dalam jaringan Internet. Protokol ini tidaklah dapat berdiri sendiri, karena memang protokol ini berupa kumpulan protokol (protocol suite). Protokol ini juga merupakan protokol yang paling banyak digunakan saat ini. Data tersebut diimplementasikan dalam bentuk perangkat lunak (software) di sistem operasi. Istilah yang diberikan kepada perangkat lunak ini adalah TCP/IP stack.

![TCP/IP Stack](/assets/tcp.png)

Protokol TCP/IP dikembangkan pada akhir dekade 1970-an hingga awal 1980-an sebagai sebuah protokol standar untuk menghubungkan komputer-komputer dan jaringan untuk membentuk sebuah jaringan yang luas (WAN). Protokol ini menggunakan skema pengalamatan yang sederhana yang disebut sebagai alamat IP (IP Address) yang mengizinkan hingga beberapa ratus juta komputer untuk dapat saling berhubungan satu sama lainnya di Internet. Protokol ini juga bersifat routable yang berarti protokol ini cocok untuk menghubungkan sistem-sistem berbeda (seperti Microsoft Windows dan keluarga UNIX) untuk membentuk jaringan yang heterogen.

#### :memo: Keunggulan TCP/IP
- Tersedia secara bebas dan dikembangkan independen terhadap komputer atau sistem operasi apapun, sehingga ideal untuk menyatukan berbagai macam hardware dan software.
- Independen dari physical network hardware yang menjadikan TCP/IP dapat mengintegrasikan berbagai macam network.
- Skema addressing yang umum sehingga device yang menggunakan TCP/IP dapat menghubungi alamat device lain di seluruh network.
- High level protocol standard yang dapat melayani user secara luas.

#### :memo: Macam-Macam Layer pada TCP/IP
**1. Link Layer**
Link Layer merupakan gabungan antara Data Link dan Physical layer. Protokol pada layer ini menyediakan media bagi system untuk mengirimkan data ke device lain yang terhubung secara langsung.

**2. Internet Layer**
Diatas Network Access Layer adalah Internet Layer. Internet Protocol adalah jantung dari TCP/IP dan protokol paling penting pada Internet Layer. Seluruh protokol, diatas dan dibawah Internet layer, menggunakan Internet Protokol untuk mengirimkan data. Semua data TCP/IP mengalir melalui IP, baik incoming maupun outgoing, dengan mengabaikan tujuan terakhirnya.

**3. Transport Layer**
Dua protokol utama pada layer ini adalah Transmission Control Protocol (TCP) dan User Datagram Protocol (UDP). TCP menyediakan layanan pengiriman data handal dengan end-to-end deteksi dan koreksi kesalahan. UDP menyediakan layanan pengiriman datagram tanpa koneksi (connectionless) dan low-overhead. Kedua protokol ini mengirmkan data diantara Application Layer dan Internet Layer.

**4. Application Layer**
Pada sisi paling atas dari arsitektur protokol TCP/IP adalah Application Layer. Layer ini termasuk seluruh proses yang menggunakan transport layer untuk mengirimkan data. Banyak sekali application protocol yang digunakan saat ini. Beberapa diantaranya adalah :
- FTP, File Transfer Protocol, digunakan untuk file transfer.
- SMTP, Simple Mail Transfer Protocol, dugunakan untuk mengirimkan electronic mail.
- DNS, Domain Name Service, untuk memetakan IP Address ke dalam nama tertentu.
- NFS, Network File System, untuk sharing file terhadap berbagai host dalam jaringan.
- HTTP, Hyper Text Transfer Protokol, protokol untuk web browsing.
- Dan lain-lain.