# Kumpulan Soal Latihan Jaringan Komputer (Bab 1 & 2)

Kumpulan soal pilihan ganda berdasarkan materi *Computer Networking: A Top-Down Approach 9th Ed.* (Kurose & Ross).<br>
Klik pada bagian **Jawaban & Penjelasan** untuk melihat kunci dan alasannya berdasarkan slide PPT.

---

## 1. Instantaneous vs Average Throughput
Apa yang membedakan *instantaneous throughput* dari *average throughput*?

a. Instantaneous throughput diukur pada suatu saat tertentu, sedangkan average throughput diukur selama interval yang lebih panjang<br>
b. Average throughput mengabaikan transfer data<br>
c. Average throughput hanya berlaku pada TCP<br>
d. Tidak ada perbedaan<br>
e. Instantaneous throughput hanya berlaku pada optical fiber<br>
f. Instantaneous throughput selalu lebih tinggi

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Instantaneous throughput diukur pada suatu saat tertentu, sedangkan average throughput diukur selama interval yang lebih panjang.<br>
*Penjelasan: Slide 1-56 mendefinisikan instantaneous throughput sebagai laju (rate) pada titik waktu tertentu, sedangkan average throughput adalah laju rata-rata selama periode waktu yang lebih panjang.*
</details>

---

## 2. Transport Layer ke Network Layer
Apa yang secara umum terjadi ketika transport-layer segment diberikan ke network layer?

a. Segment langsung menjadi sinyal listrik<br>
b. Aplikasi dijalankan di router<br>
c. Packet menjadi circuit<br>
d. Network layer menambahkan header miliknya untuk membentuk datagram<br>
e. Semua header dihapus<br>
f. Network layer menghapus semua informasi transport

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** Network layer menambahkan header miliknya untuk membentuk datagram.<br>
*Penjelasan: Slide 1-73 menunjukkan proses enkapsulasi di mana network layer membungkus transport-layer segment dengan network-layer header (Hn) untuk membuat datagram.*
</details>

---

## 3. Perangkat Layer IP
Sebuah perangkat memeriksa informasi layer IP dan meneruskan traffic menuju tujuan. Menurut model layer dalam bab ini, perangkat tersebut kemungkinan besar apa?

a. Proses pengguna<br>
b. Router<br>
c. Editor teks<br>
d. Link-layer switch murni<br>
e. Hanya repeater fisik<br>
f. Hanya server aplikasi

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: b.** Router.<br>
*Penjelasan: Slide 1-27 dan 1-71 menjelaskan bahwa router beroperasi pada network layer (layer IP) untuk melakukan fungsi forwarding dan routing datagram.*
</details>

---

## 4. End-to-End Transmission Delay (Store-and-Forward)
Satu packet melewati dua link store-and-forward, masing-masing berkecepatan R, dan propagation delay diabaikan. Berapa end-to-end transmission delay?

a. 2L/R<br>
b. L/2R<br>
c. L/R<br>
d. R/2L<br>
e. 2R/L<br>
f. 3L/R

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** 2L/R.<br>
*Penjelasan: Slide 1-30 menjelaskan konsep store-and-forward di mana seluruh packet harus tiba di router sebelum diteruskan. Untuk 2 link, delay-nya adalah (L/R) + (L/R) = 2L/R.*
</details>

---

## 5. Circuit Switching Resources
Mengapa circuit switching dapat membuang resources?

a. Reserved capacity dapat menganggur ketika pengguna tidak mengirimkan data<br>
b. Aplikasi tidak dapat mengirim data secara terus-menerus<br>
c. Link tidak dapat membawa banyak pengguna<br>
d. Circuit selalu menggunakan wireless media<br>
e. Router membuang seluruh traffic<br>
f. Setiap packet harus diduplikasi

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Reserved capacity dapat menganggur ketika pengguna tidak mengirimkan data.<br>
*Penjelasan: Slide 1-33 dan 1-36 mencatat bahwa pada circuit switching, sumber daya didedikasikan (no sharing). Jika pengguna tidak aktif (bursty data), capacity yang di-reserve akan terbuang sia-sia.*
</details>

---

## 6. Total Delay (3 Links)
Sebuah end-to-end path memiliki tiga link. Setiap link memberikan transmission delay 4 ms dan propagation delay 6 ms. Abaikan processing dan queueing. Berapa total delay?

a. 18 ms<br>
b. 10 ms<br>
c. 24 ms<br>
d. 30 ms<br>
e. 36 ms<br>
f. 60 ms

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** 30 ms.<br>
*Penjelasan: Berdasarkan rumus delay pada Slide 1-48, total delay per link = transmission + propagation = 4ms + 6ms = 10ms. Untuk 3 link: 3 × 10ms = 30ms.*
</details>

---

## 7. Packet Switching vs Circuit Switching
Mengapa packet switching menarik untuk komunikasi komputer dibanding circuit switching tradisional?

a. Traffic komputer sering berganti antara periode aktif dan tidak aktif, sehingga capacity yang reserved secara permanen menjadi tidak efisien<br>
b. Packet switching menghilangkan propagation delay<br>
c. Packet switching tidak memerlukan protocol<br>
d. Circuit switching tidak memiliki link fisik<br>
e. Komputer tidak dapat mentransmisikan melalui circuit<br>
f. Komputer tidak dapat menggunakan saluran telepon

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Traffic komputer sering berganti antara periode aktif dan tidak aktif, sehingga capacity yang reserved secara permanen menjadi tidak efisien.<br>
*Penjelasan: Slide 1-36 menyatakan packet switching sangat cocok untuk data yang "bursty" (kadang aktif, kadang tidak), memungkinkan resource sharing, dan lebih sederhana tanpa call setup.*
</details>

---

## 8. Bottleneck Rate
Sebuah path memiliki link dengan capacity 100, 50, 10, dan 80 Mbps. Berapa bottleneck rate?

a. 10 Mbps<br>
b. 80 Mbps<br>
c. 50 Mbps<br>
d. 60 Mbps<br>
e. 100 Mbps<br>
f. 240 Mbps

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** 10 Mbps.<br>
*Penjelasan: Slide 1-57 mendefinisikan bottleneck link sebagai link pada end-end path yang membatasi (constrains) throughput keseluruhan, yaitu link dengan kapasitas terendah (10 Mbps).*
</details>

---

## 9. Aplikasi Suara dan Switching
Sebuah aplikasi suara membutuhkan capacity yang dapat diprediksi sepanjang call meskipun sesekali hanya mengirim sedikit data. Konsep switching mana yang paling langsung menyediakan perilaku ini?

a. Best-effort packet switching<br>
b. IP spoofing<br>
c. Packet sniffing<br>
d. Circuit switching<br>
e. Enkapsulasi<br>
f. Resolusi DNS

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** Circuit switching.<br>
*Penjelasan: Slide 1-33 menjelaskan circuit switching menyediakan dedicated resources yang menjamin performa (circuit-like guaranteed performance), sangat cocok untuk aplikasi yang butuh prediktabilitas seperti suara.*
</details>

---

## 10. FTP Control Out-of-Band
Mengapa FTP control disebut out-of-band?

a. Command berjalan melalui DNS<br>
b. Control hanya dibawa dalam packet header<br>
c. FTP tidak menggunakan TCP connection<br>
d. Control information ditempatkan di dalam setiap file<br>
e. Data tidak pernah melintasi network<br>
f. Control information menggunakan connection yang terpisah dari file data connection

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Control information menggunakan connection yang terpisah dari file data connection.<br>
*Penjelasan: Slide 2-64 dan konsep FTP di Bab 2 menjelaskan bahwa FTP menggunakan koneksi TCP yang terpisah untuk control (port 21) dan data (port 20), yang disebut out-of-band.*
</details>

---

## 11. DNS dan E-mail Delivery
Bagaimana DNS membantu e-mail delivery?

a. DNS menggantikan SMTP<br>
b. DNS menyimpan setiap e-mail body<br>
c. DNS membuat HTTP cookie<br>
d. DNS menjamin message encryption<br>
e. DNS memetakan mail-server alias atau domain ke canonical mail server menggunakan MX information<br>
f. DNS membuka IMAP folder

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** DNS memetakan mail-server alias atau domain ke canonical mail server menggunakan MX information.<br>
*Penjelasan: Slide 2-79 menunjukkan bahwa DNS record tipe MX (Mail Exchange) memetakan nama domain ke hostname dari SMTP mail server yang bertanggung jawab.*
</details>

---

## 12. CNAME Record
Relationship apa yang dinyatakan oleh CNAME record?

a. URL ke cookie<br>
b. Domain ke mail server-nya<br>
c. Port ke process<br>
d. Hostname ke IPv4 address saja<br>
e. Alias hostname ke canonical hostname<br>
f. Domain ke authoritative server-nya

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** Alias hostname ke canonical hostname.<br>
*Penjelasan: Slide 2-79 mendefinisikan record CNAME sebagai pemetaan dari nama alias ke nama aslinya (canonical name), misalnya www.ibm.com ke servereast.backup2.ibm.com.*
</details>

---

## 13. Serangan DDoS
Ribuan host yang telah dikompromikan secara bersamaan membanjiri sebuah Web server dengan traffic. Jenis serangan apa yang terjadi?

a. DDoS<br>
b. Resolusi DNS<br>
c. Konvergensi routing<br>
d. Circuit multiplexing<br>
e. Packet switching<br>
f. Enkapsulasi

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** DDoS.<br>
*Penjelasan: Slide 1-64 menjelaskan Denial of Service (DoS/DDoS) di mana penyerang menggunakan banyak host yang dikompromikan (botnet) untuk membanjiri target dengan traffic palsu.*
</details>

---

## 14. SMTP Direct TCP Transfer
Mengapa SMTP menggunakan direct TCP transfer antara sending mail server dan receiving mail server?

a. DNS membawa message body<br>
b. FTP membuka satu data connection per line<br>
c. Browser melakukan pull setiap mail object hanya dengan HTTP<br>
d. Sending server membentuk TCP connection dan melakukan push message ke receiving server<br>
e. UDP menjamin ordered delivery<br>
f. Recipient harus online

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** Sending server membentuk TCP connection dan melakukan push message ke receiving server.<br>
*Penjelasan: Slide 2-64 membandingkan HTTP dan SMTP, di mana HTTP adalah "client pull", sedangkan SMTP adalah "client push" (sending server pushes message ke receiving server via TCP).*
</details>

---

## 15. Throughput Shared Link
Sepuluh simultaneous connections berbagi secara adil sebuah link backbone 100 Mbps. Jika backbone tersebut adalah bottleneck, kira-kira berapa throughput yang tersedia untuk setiap koneksi?

a. 1 Mbps<br>
b. 5 Mbps<br>
c. 100 Mbps<br>
d. 10 Mbps<br>
e. 50 Mbps<br>
f. 20 Mbps

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** 10 Mbps.<br>
*Penjelasan: Slide 1-58 menunjukkan bahwa jika R adalah bottleneck link yang dibagi secara adil (fairly) ke 10 koneksi, maka throughput per-koneksi adalah R/10 = 100/10 = 10 Mbps.*
</details>

---

## 16. Ukuran Packet dan Transmission Delay
Ukuran packet menjadi dua kali lipat sementara link rate tetap. Apa yang terjadi pada transmission delay?

a. Menjadi dua kali lipat<br>
b. Menjadi nol<br>
c. Menjadi setengah<br>
d. Tetap<br>
e. Menjadi empat kali lipat<br>
f. Hanya bergantung pada jarak

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Menjadi dua kali lipat.<br>
*Penjelasan: Slide 1-49 mendefinisikan transmission delay sebagai d_trans = L/R. Jika L (ukuran packet) dikali dua, maka d_trans juga menjadi dua kali lipat.*
</details>

---

## 17. Circular Identifier Space (P2P/DHT)
Mengapa peer dan key diberi identifier dalam circular identifier space yang sama?

a. Agar TCP menjadi unreliable<br>
b. Agar deterministic rule dapat menetapkan setiap key kepada responsible peer<br>
c. Agar setiap key disimpan pada setiap peer<br>
d. Agar HTTP tidak memerlukan URL<br>
e. Agar peer upload rate menjadi sama<br>
f. Agar DNS dapat membawa file data

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: b.** Agar deterministic rule dapat menetapkan setiap key kepada responsible peer.<br>
*Penjelasan: Pada arsitektur P2P DHT (Distributed Hash Table), circular ID space memungkinkan routing determinatik di mana setiap key di-hash dan diarahkan ke peer dengan ID yang paling dekat/bertanggung jawab.*
</details>

---

## 18. Link-Layer Switch
Sebuah perangkat meneruskan frame menggunakan informasi link layer tetapi tidak memproses informasi forwarding pada layer IP. Perangkat apakah itu?

a. Link-layer switch<br>
b. Proses transport<br>
c. Router<br>
d. Web server<br>
e. Pasti circuit switch<br>
f. Aplikasi DNS

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Link-layer switch.<br>
*Penjelasan: Slide 1-71 menunjukkan bahwa link layer bertugas mentransfer datagram antar elemen jaringan yang bertetangga (neighboring), yang diimplementasikan oleh switch (bukan router yang bekerja di network layer).*
</details>

---

## 19. UDP sendto() Destination Address
Mengapa UDP sendto() harus menyertakan destination address?

a. TCP menghapus UDP address<br>
b. UDP tidak memiliki pre-established connection yang mengikat socket kepada satu peer<br>
c. Destination disimpan dalam HTTP cookie<br>
d. UDP secara otomatis menggunakan DNS root<br>
e. UDP adalah file-transfer protocol<br>
f. Server tidak dapat memiliki port

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: b.** UDP tidak memiliki pre-established connection yang mengikat socket kepada satu peer.<br>
*Penjelasan: Slide 2-102 menjelaskan bahwa UDP adalah connectionless (tidak ada handshaking), sehingga sender harus secara eksplisit melampirkan IP address dan port tujuan ke setiap packet.*
</details>

---

## 20. Data Center Besar
Mengapa data center besar lazim digunakan oleh layanan client-server berskala besar?

a. Data center mengubah desain menjadi pure P2P<br>
b. Data center membuat setiap client selalu aktif<br>
c. Satu server host mungkin tidak mampu menangani service demand<br>
d. Data center menghilangkan kebutuhan akan transport protocol<br>
e. Data center menghilangkan IP addressing<br>
f. Data center menjamin zero delay

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: c.** Satu server host mungkin tidak mampu menangani service demand.<br>
*Penjelasan: Slide 2-6 menyebutkan bahwa pada arsitektur client-server, server sering kali ditempatkan di data centers untuk keperluan scaling (menangani demand yang besar).*
</details>

---

## 21. Passive Packet Sniffing
Mengapa passive packet sniffing dapat sulit dideteksi?

a. Sniffer dapat mengamati packet tanpa mengirim packet sendiri<br>
b. Sniffer menonaktifkan link fisik<br>
c. Sniffer mengenkripsi setiap packet<br>
d. Sniffer selalu mengubah alamat sumber<br>
e. Sniffer meningkatkan propagation speed<br>
f. Sniffer memerlukan reservation circuit

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Sniffer dapat mengamati packet tanpa mengirim packet sendiri.<br>
*Penjelasan: Slide 1-62 menjelaskan packet sniffing pada media broadcast/wireless di mana promiscuous interface hanya membaca/merekam packet yang lewat tanpa perlu mengirim packet apa pun.*
</details>

---

## 22. Recursive vs Iterative DNS Query
Apa perbedaan utama antara recursive dan iterative DNS query?

a. Recursive query melewati DNS server<br>
b. Keduanya hanya berbeda dalam kapitalisasi<br>
c. Recursive query hanya menggunakan TCP; iterative query menggunakan HTTP<br>
d. Iterative query tidak memuat hostname<br>
e. Recursive server memperoleh final answer untuk requester; iterative server mengembalikan referral terbaik yang dimilikinya<br>
f. Iterative query langsung menjamin authoritative answer

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** Recursive server memperoleh final answer untuk requester; iterative server mengembalikan referral terbaik yang dimilikinya.<br>
*Penjelasan: Slide 2-76 (Iterated) menunjukkan server membalas "I don't know, but ask this server", sedangkan Slide 2-77 (Recursive) menunjukkan beban resolusi diletakkan penuh pada server yang dihubungi.*
</details>

---

## 23. Packet Loss dan Buffer Router
Mengapa packet loss terjadi ketika buffer router penuh?

a. Link fisik menghilang<br>
b. Packet merambat terlalu lambat<br>
c. Router kehabisan alamat IP<br>
d. Sender mengganti protocol<br>
e. Packet otomatis mengubah tujuan<br>
f. Packet baru tidak memiliki ruang storage yang tersedia dan dapat dibuang

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Packet baru tidak memiliki ruang storage yang tersedia dan dapat dibuang.<br>
*Penjelasan: Slide 1-55 menjelaskan bahwa queue (buffer) memiliki kapasitas terbatas. Packet yang tiba saat buffer penuh akan di-drop (lost).*
</details>

---

## 24. Fungsi DSLAM
Apa fungsi DSLAM?

a. Menggantikan semua router<br>
b. Hanya menyediakan layanan suara<br>
c. Menjalankan Web application pengguna<br>
d. Mengubah IP menjadi Ethernet secara permanen<br>
e. Mengagregasikan banyak DSL subscriber connections di central office<br>
f. Mengalokasikan nama DNS

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** Mengagregasikan banyak DSL subscriber connections di central office.<br>
*Penjelasan: Slide 1-16 menunjukkan DSLAM (Digital Subscriber Line Access Multiplexer) berada di central office untuk menggabungkan banyak koneksi DSL ke network ISP.*
</details>

---

## 25. Network Peering
Mengapa dua network mungkin melakukan peering secara langsung?

a. Untuk menonaktifkan packet switching<br>
b. Untuk menghilangkan semua router<br>
c. Untuk menghapus IP addressing<br>
d. Untuk membuat satu proses aplikasi<br>
e. Untuk sengaja memperlambat traffic<br>
f. Untuk bertukar traffic tanpa selalu melewati transit provider upstream

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Untuk bertukar traffic tanpa selalu melewati transit provider upstream.<br>
*Penjelasan: Slide 1-42 menjelaskan Internet Exchange Point (IXP) dan peering link yang memungkinkan ISP bertukar traffic secara langsung, menghindari biaya transit ke ISP tier atas.*
</details>

---

## 26. Non-Persistent HTTP RTT
Mengapa non-persistent HTTP biasanya memerlukan kira-kira dua RTT sebelum sebuah object selesai tiba, tidak termasuk transmission time?

a. Satu RTT digunakan untuk membentuk TCP connection dan satu RTT lain membawa HTTP request serta initial response<br>
b. Server melakukan dua cache validation<br>
c. Satu RTT membuka FTP control dan satu lagi membuka FTP data<br>
d. Kedua RTT digunakan untuk DNS lookup<br>
e. HTTP mengirim dua request yang identik<br>
f. TCP menggunakan satu RTT per byte

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Satu RTT digunakan untuk membentuk TCP connection dan satu RTT lain membawa HTTP request serta initial response.<br>
*Penjelasan: Slide 2-24 merinci response time non-persistent HTTP: 1 RTT untuk inisiasi TCP handshake, dan 1 RTT untuk HTTP request & response awal.*
</details>

---

## 27. Distributed Hierarchy DNS
Mengapa DNS diimplementasikan sebagai distributed hierarchy, bukan satu central server?

a. Untuk menggantikan transport protocol<br>
b. Untuk memindahkan application data melalui DNS<br>
c. Untuk mewajibkan setiap host mengetahui setiap IP address<br>
d. Untuk menjamin zero query delay<br>
e. Untuk menghilangkan seluruh caching<br>
f. Untuk meningkatkan scalability, fault tolerance, traffic distribution, dan proximity

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Untuk meningkatkan scalability, fault tolerance, traffic distribution, dan proximity.<br>
*Penjelasan: Slide 2-69 menjelaskan bahwa DNS terpusat tidak akan scalable (single point of failure, traffic volume raksasa, dan jarak yang jauh), sehingga harus didesentralisasi.*
</details>

---

## 28. Peran API Internet
Apa peran API Internet bagi sebuah aplikasi?

a. Menentukan bagaimana program meminta layanan komunikasi dari network infrastructure<br>
b. Memasang tabel peroutean di setiap router<br>
c. Menentukan propagation speed<br>
d. Memilih panjang gelombang optik<br>
e. Mencegah semua packet loss<br>
f. Menentukan panjang kabel

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Menentukan bagaimana program meminta layanan komunikasi dari network infrastructure.<br>
*Penjelasan: Slide 1-6 dan 2-9 mendefinisikan API (seperti Socket) sebagai "hooks" atau antarmuka yang memungkinkan aplikasi meminta layanan transport dari infrastruktur Internet.*
</details>

---

## 29. Transmission Delay Calculation
Packet 6 Mbit dikirim melalui link 3 Mbps. Berapa lama sender membutuhkan waktu untuk menempatkan seluruh packet ke link?

a. 18 s<br>
b. 6 s<br>
c. 0,5 s<br>
d. 2 s<br>
e. 1 s<br>
f. 3 s

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** 2 s.<br>
*Penjelasan: Berdasarkan rumus Slide 1-21 & 1-49, Transmission Delay = L/R = 6 Mbit / 3 Mbps = 2 detik.*
</details>

---

## 30. Web Object
Apa yang dimaksud dengan Web object?

a. browser process saja<br>
b. DNS root server<br>
c. Sebuah file yang dapat dialamatkan oleh satu URL<br>
d. TCP connection<br>
e. port number<br>
f. HTTP cookie database

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: c.** Sebuah file yang dapat dialamatkan oleh satu URL.<br>
*Penjelasan: Slide 2-18 mendefinisikan Web object (HTML, JPEG, audio, dll) sebagai entitas yang dapat di-address menggunakan sebuah URL.*
</details>

---

## 31. End System
Istilah apa yang digunakan untuk perangkat yang terhubung ke Internet dan menjalankan aplikasi network?

a. packet queue<br>
b. protocol header<br>
c. Circuit<br>
d. transmission channel<br>
e. routing domain<br>
f. end system

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** end system.<br>
*Penjelasan: Slide 1-3 menyatakan "hosts = end systems", yaitu perangkat yang menjalankan network applications di tepi (edge) Internet.*
</details>

---

## 32. HTTP dan TCP Recovery
Mengapa HTTP tidak perlu mengimplementasikan recovery sendiri dari lost segment ketika menggunakan TCP?

a. HTTP memperbaiki loss menggunakan checksum pada setiap request header.<br>
b. Web server mengulang setiap response sampai browser memberikan confirmation.<br>
c. DNS menyimpan backup copy dari seluruh HTTP object.<br>
d. TCP menyediakan reliable data transfer kepada HTTP.<br>
e. IP menjamin retransmission untuk setiap lost segment.<br>
f. Browser mengambil setiap Web object dua kali lalu membandingkan kedua copy.

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** TCP menyediakan reliable data transfer kepada HTTP.<br>
*Penjelasan: Slide 2-14 dan 2-19 menjelaskan bahwa HTTP menggunakan TCP, yang sudah menyediakan layanan reliable transport (menjamin data tidak hilang dan terurut).*
</details>

---

## 33. Web Cache sebagai Server/Client
Mengapa Web cache bertindak sebagai server sekaligus client?

a. Web cache menyajikan object kepada browser dan mengambil missing object dari origin server.<br>
b. Web cache memelihara FTP user state.<br>
c. Web cache selalu menjadi content owner.<br>
d. Web cache hanya mengirim dan menerima DNS zone.<br>
e. Web cache menetapkan IP address dan port number.<br>
f. Web cache menggantikan semua end system.

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Web cache menyajikan object kepada browser dan mengambil missing object dari origin server.<br>
*Penjelasan: Slide 2-43 menjelaskan Web cache (proxy server) bertindak sebagai server bagi client yang meminta, dan bertindak sebagai client saat meminta object ke origin server.*
</details>

---

## 34. Protocol Compatibility
Dua program yang dibuat secara independen dapat beroperasi bersama karena keduanya mengikuti message format dan response rule yang sama. Apa penjelasan terbaik?

a. Keduanya menggunakan satu socket object.<br>
b. Keduanya mengimplementasikan application-layer protocol yang sama.<br>
c. Keduanya memiliki link rate yang sama.<br>
d. Keduanya melewati transport service.<br>
e. Keduanya menggunakan source code yang identik.<br>
f. Keduanya berjalan pada host yang sama.

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: b.** Keduanya mengimplementasikan application-layer protocol yang sama.<br>
*Penjelasan: Slide 2-11 menyatakan bahwa open protocols (seperti RFC HTTP/SMTP) mendefinisikan syntax dan semantics, memungkinkan interoperabilitas antar program yang berbeda.*
</details>

---

## 35. P2P File Distribution
Sebuah file-distribution application membagi file menjadi beberapa chunk. Host A melakukan download chunk 1-10 dari permanent server, menerima chunk 11-15 dari Host B, dan secara bersamaan melakukan upload completed chunk kepada Host C dan D. Architectural classification mana yang paling sesuai dengan behavior tersebut?

a. Centralized computing karena satu server tetap online<br>
b. DNS hierarchy karena beberapa host berpartisipasi<br>
c. Web caching karena completed chunk disimpan secara lokal<br>
d. Strict client-server karena permanent server menyimpan file pada awalnya<br>
e. Circuit switching karena chunk mengikuti path yang berbeda<br>
f. P2P karena participating host menerima sekaligus menyediakan content

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** P2P karena participating host menerima sekaligus menyediakan content.<br>
*Penjelasan: Slide 2-7 mendefinisikan arsitektur P2P di mana arbitrary end systems berkomunikasi langsung, meminta layanan sekaligus menyediakan layanan (upload/download) satu sama lain.*
</details>

---

## 36. Cache Hit Rate
Sebuah cache memiliki hit rate 40% untuk request yang tanpa cache akan melintasi access link. Berapa persentase request yang tetap melintasi link tersebut?

a. 20%<br>
b. 50%<br>
c. 60%<br>
d. 40%<br>
e. 80%<br>
f. 100%

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: c.** 60%.<br>
*Penjelasan: Slide 2-47 menunjukkan bahwa jika hit rate adalah 0.4 (40%), maka sisanya (100% - 40% = 60%) adalah miss rate yang harus diteruskan ke origin server melintasi access link.*
</details>

---

## 37. Persistent HTTP/Pipelining
Dua site menyajikan object identik melalui link dengan rate yang sama dan memiliki RTT yang sama. Trace menunjukkan Site A membuka TCP connection baru untuk setiap object, sedangkan Site B menggunakan kembali satu connection dan mengirim beberapa request tanpa menunggu response sebelumnya. Mechanism mana yang paling tepat menjelaskan completion time Site B yang lebih rendah?

a. Connection reuse menghilangkan object transmission time<br>
b. Site B menghindari connection setup berulang dan dapat melakukan request pipelining<br>
c. Connection baru untuk setiap object mempertahankan satu shared congestion window<br>
d. Non-persistent HTTP menghilangkan handshake RTT setelah object pertama<br>
e. Pipelining menjamin setiap object sudah berada dalam cache<br>
f. Persistent HTTP meningkatkan physical propagation speed

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: b.** Site B menghindari connection setup berulang dan dapat melakukan request pipelining.<br>
*Penjelasan: Slide 2-25 menjelaskan Persistent HTTP (HTTP/1.1) meninggalkan koneksi terbuka, dan pipelining memungkinkan client mengirim request berturut-turut tanpa menunggu response, memangkas RTT.*
</details>

---

## 38. Application Layer Protocol Definition
Apa yang didefinisikan oleh application-layer protocol?

a. transport-layer retransmission timer<br>
b. message type, syntax, semantics, dan rule tentang kapan message dikirim<br>
c. hanya application name dan well-known port number<br>
d. user-interface appearance dan application source code<br>
e. routing path dan router queue policy<br>
f. physical signal encoding dan connector dimension

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: b.** message type, syntax, semantics, dan rule tentang kapan message dikirim.<br>
*Penjelasan: Slide 2-11 secara eksplisit merinci 4 hal yang didefinisikan protokol: types of messages, syntax, semantics, dan rules for when/how processes send & respond.*
</details>

---

## 39. FTP LIST Command
Setelah menerima FTP LIST command pada control connection, bagaimana server harus mentransfer directory-listing data?

a. menutup control connection tanpa mengirim listing data<br>
b. menunggu client mengirim HTTP Cookie header<br>
c. mengirim directory listing melalui separate data connection<br>
d. menyimpan listing dalam DNS record untuk client<br>
e. mengirim seluruh listing data secara langsung melalui control connection<br>
f. mengembalikan HTTP status line yang memuat listing

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: c.** mengirim directory listing melalui separate data connection.<br>
*Penjelasan: Karena FTP bersifat out-of-band (Slide 2-64), data aktual (termasuk hasil directory listing) dikirim melalui koneksi data terpisah, bukan melalui koneksi kontrol.*
</details>

---

## 40. Protocol Compatibility Reason
Mengapa entitas yang berkomunikasi harus menerapkan protocol yang kompatibel?

a. Jika tidak, packet tidak memiliki tujuan<br>
b. Jika tidak, propagation delay menjadi tak hingga<br>
c. Jika tidak, bandwidth menjadi nol<br>
d. Jika tidak, semua packet menjadi nirkabel<br>
e. Jika tidak, router berubah menjadi switch<br>
f. Jika tidak, mereka dapat menafsirkan format message atau tindakan yang diharapkan secara berbeda

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Jika tidak, mereka dapat menafsirkan format message atau tindakan yang diharapkan secara berbeda.<br>
*Penjelasan: Slide 1-7 mendefinisikan protokol sebagai aturan format, urutan, dan aksi. Tanpa standar yang sama, entitas tidak akan bisa memahami pesan satu sama lain.*
</details>

---

## 41. Queueing Delay Cause
Mengapa packet dapat mengalami queueing delay pada suatu output link?

a. Link mungkin sedang mentransmisikan packet lain<br>
b. Aplikasi berhenti berjalan<br>
c. Header packet menghilang<br>
d. Setiap packet membuat circuit<br>
e. propagation speed menjadi nol<br>
f. Router selalu menolak traffic simultan

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Link mungkin sedang mentransmisikan packet lain.<br>
*Penjelasan: Slide 1-31 menjelaskan queueing delay terjadi ketika packet harus menunggu di buffer karena output link sedang sibuk mentransmisikan packet lain yang tiba lebih dulu.*
</details>

---

## 42. Network App vs Protocol Scope
Mengapa network application lebih luas daripada application-layer protocol-nya?

a. Protocol menggantikan client dan server process<br>
b. Application hanya merupakan judul RFC<br>
c. Application tidak pernah bertukar message<br>
d. Protocol hanya ada pada physical layer<br>
e. Protocol memuat seluruh operating-system code<br>
f. Application juga mencakup user interface, data, dan implementation logic

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Application juga mencakup user interface, data, dan implementation logic.<br>
*Penjelasan: Slide 2-5 dan 2-11 membedakan aplikasi (program utuh yang ditulis developer termasuk UI/logika) dengan protokol (hanya aturan komunikasi standar pertukaran pesan).*
</details>

---

## 43. IP Spoofing
Sebuah packet yang diterima mengklaim berasal dari host tepercaya, tetapi penyerang secara manual memasukkan alamat host tersebut ke field sumber. Masalah apa yang ditunjukkan?

a. Transmission delay<br>
b. Packet queueing<br>
c. DNS caching<br>
d. Propagation loss<br>
e. IP spoofing<br>
f. Circuit switching

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** IP spoofing.<br>
*Penjelasan: Slide 1-63 mendefinisikan IP spoofing sebagai injeksi packet dengan source address palsu untuk menyamar sebagai host lain.*
</details>

---

## 44. Shared Access Capacity
Sebuah lingkungan memiliki 200 rumah yang terhubung melalui segmen kabel yang sama. Banyak rumah mulai mengunduh secara bersamaan. Sifat apa yang paling relevan terhadap access performance mereka?

a. Hanya standardisasi TCP/IP<br>
b. Hanya propagation speed optik<br>
c. Konvensi penamaan DNS<br>
d. Hanya format header packet<br>
e. Shared access capacity<br>
f. Sintaks API aplikasi

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** Shared access capacity.<br>
*Penjelasan: Slide 1-15 menjelaskan akses kabel (HFC) di mana rumah-rumah berbagi (share) access network menuju cable headend, sehingga kapasitas dibagi saat banyak yang aktif.*
</details>

---

## 45. Route/Path
Sebuah packet melewati laptop, access network Wi-Fi, sebuah router, beberapa router ISP, dan akhirnya sebuah Web server. Istilah apa yang paling tepat untuk menggambarkan urutan communication link dan packet switch yang dilewati?

a. Sesi<br>
b. Route atau path<br>
c. Frekuensi circuit<br>
d. Layanan transport<br>
e. Protocol<br>
f. Application interface

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: b.** Route atau path.<br>
*Penjelasan: Slide 1-26 dan 1-45 merujuk pada urutan link dan router dari sumber ke tujuan sebagai path atau route yang ditentukan oleh routing algorithm.*
</details>

---

## 46. Bottleneck Link Throughput
Sebuah path memiliki link capacity 20 Mbps dan 5 Mbps. Dengan mengabaikan traffic lain, berapa throughput end-to-end maksimum?

a. 5 Mbps<br>
b. 20 Mbps<br>
c. 10 Mbps<br>
d. 2,5 Mbps<br>
e. 100 Mbps<br>
f. 25 Mbps

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** 5 Mbps.<br>
*Penjelasan: Slide 1-57 menegaskan bahwa bottleneck link (link dengan kapasitas terkecil di sepanjang path) akan membatasi throughput end-to-end secara keseluruhan.*
</details>

---

## 47. Web Cache Response Time
Mengapa Web cache dapat mengurangi user-perceived response time?

a. Web cache meningkatkan physical access-link capacity untuk setiap request<br>
b. Web cache melakukan compression pada setiap Web object sebelum transmission<br>
c. Web cache menghilangkan DNS lookup untuk setiap cache miss<br>
d. Cached object yang dekat dapat dikirim tanpa melewati access path yang lebih lambat menuju origin server<br>
e. Web cache menjamin processing time yang lebih singkat pada origin server<br>
f. Web cache meningkatkan propagation speed pada Internet path

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** Cached object yang dekat dapat dikirim tanpa melewati access path yang lebih lambat menuju origin server.<br>
*Penjelasan: Slide 2-43 menyatakan cache mengurangi response time karena letaknya lebih dekat ke client dan mengurangi traffic yang harus melewati access link institusi yang lambat.*
</details>

---

## 48. Packet Switches
Dua perangkat apa yang diidentifikasi sebagai jenis packet switch yang paling menonjol?

a. Modem dan server<br>
b. DSLAM dan browser<br>
c. Host dan API<br>
d. TCP dan IP<br>
e. Router dan link-layer switch<br>
f. Klien dan server

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** Router dan link-layer switch.<br>
*Penjelasan: Slide 1-3 secara eksplisit menyebutkan "Packet switches: forward packets... routers, switches" sebagai dua perangkat utama di network core.*
</details>

---

## 49. Sensor Transport Choice
Sebuah sensor mengirim fresh temperature reading setiap detik. Reading yang tiba terlambat lebih dari dua detik tidak lagi bernilai karena reading yang lebih baru sudah tersedia. Application dapat mentoleransi occasional missing reading dan harus menghindari connection-establishment delay. Transport choice mana yang paling sesuai dengan requirement tersebut?

a. DNS karena memetakan setiap reading ke sebuah address<br>
b. UDP karena menghindari connection setup dan memungkinkan application mentoleransi loss<br>
c. HTTP karena menetapkan port bagi setiap sensor<br>
d. SMTP karena melakukan push reading kepada receiver<br>
e. FTP karena memisahkan control data dan sensor data<br>
f. TCP karena melakukan retransmission terhadap setiap missing reading hingga tiba

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: b.** UDP karena menghindari connection setup dan memungkinkan application mentoleransi loss.<br>
*Penjelasan: Slide 2-14 dan 2-102 menunjukkan UDP cocok untuk aplikasi loss-tolerant dan time-sensitive karena tidak memiliki connection setup delay dan tidak melakukan retransmisi yang memperlambat data.*
</details>

---

## 50. P2P Self-Scalability
Sebuah distribution service pada awalnya bergantung pada satu server. Ketika user baru bergabung, total demand meningkat, tetapi aggregate upload capacity juga meningkat karena para user saling bertukar chunk. Architectural property mana yang paling tepat menjelaskan perilaku ini?

a. TCP congestion loss<br>
b. client-server centralization<br>
c. HTTP statelessness<br>
d. P2P self-scalability<br>
e. DNS recursion<br>
f. out-of-band FTP control

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** P2P self-scalability.<br>
*Penjelasan: Slide 2-7 menyoroti "self scalability" sebagai keunggulan P2P: peer baru tidak hanya membawa demand baru, tetapi juga membawa service capacity (upload bandwidth) baru.*
</details>

---

## 51. P2P Aggregate Upload
Sebuah distributor memiliki upload capacity 100 Mbps. Setiap peer baru melakukan download hingga 20 Mbps dan menyumbangkan upload capacity 4 Mbps setelah menerima sebagian file. Hasil pengukuran menunjukkan distribution time pada awalnya meningkat cepat, tetapi pertumbuhannya melambat ketika additional peer bergabung. Penjelasan mana yang paling tepat untuk hasil tersebut?

a. DNS mendistribusikan bagian file yang berbeda kepada peer yang berbeda<br>
b. HTTP statelessness menghilangkan distributor bottleneck<br>
c. Peer download capacity menggantikan distributor upload capacity<br>
d. File menjadi lebih kecil ketika lebih banyak peer menerimanya<br>
e. TCP menjamin setiap peer menerima file dengan rate yang sama<br>
f. Aggregate upload capacity meningkat karena additional peer menjadi content supplier

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Aggregate upload capacity meningkat karena additional peer menjadi content supplier.<br>
*Penjelasan: Sama seperti Slide 2-7, dalam P2P, setiap peer yang bergabung bertindak sebagai supplier yang menambah total kapasitas upload jaringan, memperlambat laju peningkatan waktu distribusi.*
</details>

---

## 52. Pemrogram & Interface Layanan Internet
Seorang pemrogram ingin program pada Host A mengirim data ke program pada Host B. Menurut pandangan Internet sebagai penyedia layanan, apa yang secara konseptual harus digunakan pemrogram?

a. Interface yang disediakan end system untuk mengakses network communication services<br>
b. Route yang dikonfigurasi manual melalui setiap router<br>
c. Link satelit<br>
d. New physical-layer protocol<br>
e. Reservation circuit switching<br>
f. Kawat fisik khusus langsung ke Host B

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Interface yang disediakan end system untuk mengakses network communication services.<br>
*Penjelasan: Slide 1-6 (Services view) dan 2-9 (Sockets) menjelaskan bahwa Internet menyediakan API (Socket interface) di end system bagi developer untuk menghubungkan aplikasi ke layanan transport.*
</details>

---

## 53. TCP send() tanpa destination
Mengapa TCP client menggunakan send() tanpa menyertakan destination pada setiap call?

a. HTTP cookie mengarahkan segment.<br>
b. Server menggunakan UDP recvfrom().<br>
c. TCP tidak memiliki address.<br>
d. FTP control menyediakan address.<br>
e. Socket sudah dikaitkan dengan remote endpoint oleh connect().<br>
f. DNS memasukkan address ke setiap byte.

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** Socket sudah dikaitkan dengan remote endpoint oleh connect().<br>
*Penjelasan: Slide 2-106 dan 2-108 menunjukkan bahwa pada TCP, fungsi `connect()` sudah melakukan handshake dan mengikat socket ke IP/Port tujuan, sehingga `send()` tinggal mengirim byte stream.*
</details>

---

## 54. Peran ISP Tingkat Atas
Apa peran ISP tingkat atas dalam struktur Internet yang dijelaskan pada bab ini?

a. Hanya menyediakan layanan telepon suara<br>
b. Menyimpan setiap packet Internet<br>
c. Menjalankan setiap aplikasi pengguna<br>
d. Menghubungkan network tingkat bawah pada geographic region yang luas<br>
e. Menggantikan access network<br>
f. Menghilangkan routing

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** Menghubungkan network tingkat bawah pada geographic region yang luas.<br>
*Penjelasan: Slide 1-45 menjelaskan Tier-1 ISPs (seperti Level 3, Sprint) berada di "center" Internet dengan cakupan nasional/internasional yang menghubungkan ISP regional dan access.*
</details>

---

## 55. Sifat Protocol (Browser Request)
Sebuah browser mengirim connection request, menunggu respons, lalu mengirim permintaan Web. Sifat protocol apa yang paling langsung ditunjukkan?

a. Queue capacity<br>
b. propagation speed<br>
c. Bandwidth link<br>
d. Pertukaran message berurutan dan tindakan yang terkait<br>
e. Topologi fisik<br>
f. Pembagian frekuensi

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** Pertukaran message berurutan dan tindakan yang terkait.<br>
*Penjelasan: Slide 1-7 dan 1-8 mendefinisikan protokol berdasarkan format, urutan (order) pesan yang dikirim/diterima, dan tindakan (actions) yang diambil akibat pesan tersebut.*
</details>

---

## 56. Cookie dan State
Bagaimana cookie dapat membuat user session di atas stateless HTTP?

a. Browser mengembalikan server-issued identifier yang dikaitkan server dengan stored state.<br>
b. Browser mengirim Set-Cookie dalam request, bukan menerimanya dalam response.<br>
c. Server menyimpan seluruh session hanya di dalam TCP connection saat ini.<br>
d. Cookie mengenkripsi seluruh application data secara otomatis.<br>
e. Server menggunakan identifier yang sama untuk setiap user.<br>
f. Browser membuat identifier yang tidak memiliki corresponding server record.

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Browser mengembalikan server-issued identifier yang dikaitkan server dengan stored state.<br>
*Penjelasan: Slide 2-33 dan 2-34 menjelaskan komponen cookie: server memberi ID, menyimpan state di backend DB, dan browser mengembalikan ID tersebut pada request selanjutnya.*
</details>

---

## 57. Traceroute Delay Values
Apa arti beberapa nilai delay untuk satu hop pada traceroute?

a. Reservation circuit yang terpisah<br>
b. Server tujuan yang berbeda<br>
c. Kabel fisik yang berbeda di dalam host<br>
d. Protocol aplikasi yang berbeda<br>
e. Ukuran payload packet yang pasti berbeda<br>
f. Hasil pengukuran dari beberapa packet probe

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Hasil pengukuran dari beberapa packet probe.<br>
*Penjelasan: Slide 1-53 menjelaskan traceroute mengirimkan 3 probe packets per router, sehingga menampilkan 3 nilai waktu (delay) yang berbeda untuk setiap hop.*
</details>

---

## 58. Router Queueing (8Mbps vs 5Mbps)
Sebuah router menerima packet untuk output link pada rate 8 Mbps, sementara link tersebut hanya dapat mentransmisikan 5 Mbps dalam interval yang cukup lama. Perilaku langsung apa yang diharapkan?

a. Circuit khusus dibuat secara otomatis<br>
b. Packet menumpuk di queue<br>
c. Output link otomatis menjadi 8 Mbps<br>
d. Semua packet melewati router tanpa diproses<br>
e. Alamat IP ditulis ulang<br>
f. propagation speed meningkat

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: b.** Packet menumpuk di queue.<br>
*Penjelasan: Slide 1-31 dan 1-52 menunjukkan bahwa jika arrival rate (8 Mbps) melebihi transmission rate/service capacity (5 Mbps), packet akan mengantri (queue) dan akhirnya hilang jika buffer penuh.*
</details>

---

## 59. Enterprise Network Category
Sebuah perusahaan menghubungkan komputer desktop ke switch Ethernet pusat. Kategori network apa dari bab ini yang paling tepat menggambarkannya?

a. Link geostasioner<br>
b. circuit-switched telephone network<br>
c. access network perusahaan<br>
d. Backbone content provider<br>
e. Satellite access system<br>
f. Backbone ISP Tier-1

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: c.** access network perusahaan.<br>
*Penjelasan: Slide 1-19 mendefinisikan Enterprise Networks (access network untuk perusahaan/universitas) yang menggunakan mix of switches dan routers (seperti Ethernet) untuk menghubungkan end systems.*
</details>

---

## 60. HTTP Status Code 404
Apa arti HTTP status code 404?

a. Server tidak dapat memahami request syntax.<br>
b. Request berhasil dan response memuat resource.<br>
c. Server mengalami internal error.<br>
d. Requested resource tidak ditemukan pada server.<br>
e. Cached representation masih current.<br>
f. Resource telah berpindah secara permanen ke URL lain.

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** Requested resource tidak ditemukan pada server.<br>
*Penjelasan: Slide 2-30 secara eksplisit mencantumkan "404 Not Found: requested document not found on this server".*
</details>

---

## 61. Hubungan Antar Layer
Hubungan apa yang ada antara layer yang berdekatan?

a. Sebuah layer menyediakan layanan kepada upper layer sambil menggunakan layanan dari lower layer<br>
b. Lower layer menjalankan aplikasi<br>
c. Upper layer mengendalikan electrical signaling secara langsung<br>
d. Setiap layer menggunakan protocol yang identik<br>
e. Layer tidak pernah bertukar data<br>
f. Setiap layer beroperasi sepenuhnya independen dari layer lain

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Sebuah layer menyediakan layanan kepada upper layer sambil menggunakan layanan dari lower layer.<br>
*Penjelasan: Slide 1-69 menjelaskan konsep layering: setiap layer mengimplementasikan layanan melalui aksi internalnya dengan mengandalkan (relying on) layanan dari layer di bawahnya.*
</details>

---

## 62. Manfaat Layering
Mengapa layering berguna dalam sistem network yang kompleks?

a. Membagi fungsi menjadi modul dengan layanan dan interface yang terdefinisi<br>
b. Menjamin delay nol<br>
c. Menghilangkan protocol<br>
d. Menghilangkan physical media<br>
e. Menempatkan semua fungsi pada satu komponen<br>
f. Menjamin tidak ada kegagalan

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Membagi fungsi menjadi modul dengan layanan dan interface yang terdefinisi.<br>
*Penjelasan: Slide 1-70 menyatakan layering memberikan explicit structure, modularization yang memudahkan maintenance, dan pembaruan sistem tanpa mengganggu layer lain.*
</details>

---

## 63. Koneksi Antar ISP
Mengapa ISP yang dikelola secara independen harus saling terhubung?

a. Agar host yang terhubung melalui ISP berbeda dapat berkomunikasi<br>
b. Untuk menghilangkan protocol IP<br>
c. Untuk mengubah packet menjadi circuit<br>
d. Agar semua access link menjadi nirkabel<br>
e. Untuk menghilangkan kebutuhan akan router<br>
f. Untuk memberikan bandwidth yang sama kepada semua host

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** Agar host yang terhubung melalui ISP berbeda dapat berkomunikasi.<br>
*Penjelasan: Slide 1-37 menegaskan bahwa access ISPs harus saling terkoneksi (interconnected) sehingga "any two hosts (anywhere!)" dapat saling mengirim packet.*
</details>

---

## 64. Internetworking Architecture
Terdapat beberapa packet-switched network independen yang tidak dapat berkomunikasi satu sama lain. Perkembangan historis mana yang mengatasi masalah ini?

a. Hanya manajemen queue<br>
b. Amplifikasi optik<br>
c. Packet sniffing<br>
d. Reservation circuit<br>
e. Kompresi aplikasi<br>
f. Internetworking architecture

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Internetworking architecture.<br>
*Penjelasan: Slide 1-80 mencatat sejarah tahun 1974 di mana Cerf dan Kahn mengembangkan arsitektur internetworking (cikal bakal TCP/IP) untuk menghubungkan jaringan-jaringan yang independen.*
</details>

---

## 65. HTTP Optimization (Idle Gap)
Trace dari satu persistent TCP connection menunjukkan: request 1, response 1, idle gap; request 2, response 2, idle gap; request 3, response 3. Connection tidak pernah dibuka kembali. HTTP optimization mana yang belum digunakan dan dapat menghilangkan waktu tunggu sebelum request 2 dan 3?

a. DNS caching<br>
b. conditional GET<br>
c. cookie reuse<br>
d. pipelining<br>
e. parallel TCP connection<br>
f. non-persistent HTTP

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** pipelining.<br>
*Penjelasan: Slide 2-25 dan 2-49 menjelaskan bahwa tanpa pipelining, client harus menunggu response sebelum mengirim request berikutnya. Pipelining menghilangkan "idle gap" dengan mengirim request berturut-turut.*
</details>

---

## 66. Optical Fiber Advantages
Mengapa optical fiber menarik untuk network berkecepatan tinggi?

a. Tidak memiliki propagation delay<br>
b. Mendukung transmission rate tinggi dan tahan terhadap interferensi elektromagnetik<br>
c. Secara otomatis menjamin senderan yang andal<br>
d. Selalu lebih murah daripada semua media lain<br>
e. Tidak memerlukan pemancar atau receiver<br>
f. Menyimpan packet secara permanen

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: b.** Mendukung transmission rate tinggi dan tahan terhadap interferensi elektromagnetik.<br>
*Penjelasan: Slide 1-23 merinci keunggulan fiber optic: high-speed point-to-point transmission (10s-100s Gbps), low error rate, dan immune to electromagnetic noise.*
</details>

---

## 67. DSL vs Cable Access Difference
Pengamatan mana yang paling baik membedakan DSL access dan kabel sebagaimana dijelaskan dalam bab ini?

a. DSL tidak menggunakan modem<br>
b. Kabel tidak terhubung ke ISP<br>
c. Kabel hanya menggunakan radio sedangkan DSL hanya menggunakan optical fiber<br>
d. DSL tidak dapat membawa suara<br>
e. DSL biasanya menyediakan dedicated line dari setiap rumah ke central office, sedangkan capacity kabel digunakan bersama pada segmen lingkungan<br>
f. Kabel tidak dapat menyediakan layanan asimetris

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** DSL biasanya menyediakan dedicated line dari setiap rumah ke central office, sedangkan capacity kabel digunakan bersama pada segmen lingkungan.<br>
*Penjelasan: Slide 1-16 menunjukkan DSL menggunakan "dedicated line" ke DSLAM, sedangkan Slide 1-15 menunjukkan Cable (HFC) menggunakan "shared cable distribution network".*
</details>

---

## 68. UDP Services beyond IP
Apa yang disediakan UDP kepada application selain IP?

a. process-to-process delivery dan error checking tanpa reliability guarantee<br>
b. guaranteed minimum throughput<br>
c. Web caching<br>
d. application-layer encryption<br>
e. connection setup dan retransmission<br>
f. DNS name resolution

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: a.** process-to-process delivery dan error checking tanpa reliability guarantee.<br>
*Penjelasan: Slide 2-14 dan 2-102 menjelaskan UDP menambahkan proses-to-process delivery (melalui port) dan checksum (error checking) di atas layanan best-effort IP, tanpa jaminan keandalan.*
</details>

---

## 69. Traffic Intensity La/R > 1
Jika La/R > 1 berlangsung secara terus-menerus, kesimpulan mana yang paling tepat?

a. Network berubah menjadi circuit-switched<br>
b. Propagation delay menghilang<br>
c. Queueing delay harus nol<br>
d. Offered load melebihi service capacity, sehingga queue tidak dapat tetap stabil tanpa batas<br>
e. Tidak ada packet yang dapat hilang<br>
f. Ukuran packet otomatis mengecil

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** Offered load melebihi service capacity, sehingga queue tidak dapat tetap stabil tanpa batas.<br>
*Penjelasan: Slide 1-52 menjelaskan jika traffic intensity (La/R) > 1, maka "work" yang datang lebih besar dari yang bisa dilayani, menyebabkan average queueing delay menjadi infinite (tak terhingga).*
</details>

---

## 70. Full-Mesh ISP Impracticality
Mengapa full-mesh connection di antara semua access ISP tidak praktis?

a. optical fiber tidak dapat menghubungkan ISP<br>
b. TCP melarang interconnection<br>
c. Jumlah pairwise connections yang dibutuhkan tumbuh sangat cepat ketika jumlah ISP meningkat<br>
d. Packet tidak dapat melewati lebih dari satu ISP<br>
e. Router hanya bekerja di dalam satu network<br>
f. Access ISP tidak dapat bertukar traffic

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: c.** Jumlah pairwise connections yang dibutuhkan tumbuh sangat cepat ketika jumlah ISP meningkat.<br>
*Penjelasan: Slide 1-39 menyatakan menghubungkan setiap access ISP satu sama lain secara langsung "doesn't scale" karena membutuhkan O(N^2) koneksi.*
</details>

---

## 71. Elastic Application Throughput
Mengapa elastic application sering dapat mentoleransi throughput yang berubah-ubah?

a. Application tersebut selalu menggunakan UDP.<br>
b. Application tersebut memerlukan zero packet loss dan zero delay.<br>
c. Application tersebut melewati transport layer.<br>
d. Application tersebut tidak memiliki application process.<br>
e. Application tersebut tidak pernah mentransfer data.<br>
f. Application tersebut dapat menggunakan throughput yang tersedia tanpa memerlukan fixed minimum rate.

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Application tersebut dapat menggunakan throughput yang tersedia tanpa memerlukan fixed minimum rate.<br>
*Penjelasan: Slide 2-12 mendefinisikan "elastic apps" (seperti email, web, file transfer) sebagai aplikasi yang "make use of whatever throughput they get" (fleksibel terhadap bandwidth).*
</details>

---

## 72. Total Router Delay Calculation
Sebuah packet melewati empat router. Pada setiap router, processing delay 1 ms dan queueing delay 2 ms. Dengan mengabaikan transmission dan propagation, berapa total delay dari router yang ditambahkan?

a. 8 ms<br>
b. 24 ms<br>
c. 16 ms<br>
d. 12 ms<br>
e. 3 ms<br>
f. 4 ms

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** 12 ms.<br>
*Penjelasan: Slide 1-48 merinci nodal delay = d_proc + d_queue + d_trans + d_prop. Total per router = 1ms + 2ms = 3ms. Untuk 4 router: 4 × 3ms = 12ms.*
</details>

---

## 73. Encapsulation Process
Pada sender, header transport ditambahkan ke application message, kemudian header network ditambahkan. Pernyataan mana yang benar?

a. application message menghilang<br>
b. Frame dibuat sebelum segment<br>
c. Header network menggantikan header transport<br>
d. Header transport dihapus sebelum enkapsulasi network<br>
e. Payload network layer yang dihasilkan berisi seluruh transport segment<br>
f. Enkapsulasi hanya terjadi pada router

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** Payload network layer yang dihasilkan berisi seluruh transport segment.<br>
*Penjelasan: Slide 1-73 menunjukkan proses enkapsulasi di mana network layer membungkus (encapsulates) seluruh transport segment [Ht | M] dengan headernya (Hn) untuk membentuk datagram.*
</details>

---

## 74. TCP Welcoming vs Connection Socket
Mengapa TCP server menggunakan welcoming socket dan connection socket?

a. Welcoming socket mentransfer byte setiap client secara langsung.<br>
b. Yang satu UDP dan yang lain FTP.<br>
c. Connection socket hanya menyimpan cookie.<br>
d. Yang satu membawa DNS dan yang lain HTTP.<br>
e. Welcoming socket menerima client baru; setiap connection socket berkomunikasi dengan satu client.<br>
f. Keduanya selalu merujuk pada socket object yang sama.

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** Welcoming socket menerima client baru; setiap connection socket berkomunikasi dengan satu client.<br>
*Penjelasan: Slide 2-106 dan 2-109 menjelaskan server TCP membuat welcoming socket untuk `listen()`, lalu membuat connection socket baru saat `accept()` untuk berkomunikasi dengan client spesifik.*
</details>

---

## 75. Content Provider Private Backbone Impact
Sebuah content provider besar membangun backbone global privat dan terhubung langsung ke banyak access ISP. Apa dampak arsitektural dari langkah ini?

a. Menghilangkan semua packet switch dari Internet<br>
b. Mengubah Internet menjadi circuit-switched network<br>
c. Mencegah ISP lain beroperasi<br>
d. Dapat melewati sebagian hierarki ISP tradisional dan memberikan kendali lebih besar terhadap senderan konten<br>
e. Menghilangkan protocol transport<br>
f. Menjamin end-to-end delay nol

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: d.** Dapat melewati sebagian hierarki ISP tradisional dan memberikan kendali lebih besar terhadap senderan konten.<br>
*Penjelasan: Slide 1-44 dan 1-45 menjelaskan content provider networks (seperti Google, Facebook) membuat private network yang bypass tier-1/regional ISPs untuk mendekatkan konten ke end-users.*
</details>

---

## 76. Circuit Switching Capacity Division
Sebuah link 1 Mbps dibagi menjadi 10 circuit yang sama besar. Berapa capacity yang diperoleh setiap circuit?

a. 50 kbps<br>
b. 500 kbps<br>
c. 200 kbps<br>
d. 10 kbps<br>
e. 1 Mbps<br>
f. 100 kbps

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** 100 kbps.<br>
*Penjelasan: Slide 1-34 menjelaskan konsep FDM/TDM pada circuit switching di mana bandwidth link dibagi secara eksklusif ke sejumlah circuit. 1 Mbps (1000 kbps) / 10 = 100 kbps.*
</details>

---

## 77. SMTP Envelope vs Message Header
Mengapa mail message header "From:" tidak boleh disamakan dengan SMTP "MAIL FROM"?

a. MAIL FROM mengambil message.<br>
b. Keduanya merupakan TCP header yang identik.<br>
c. Keduanya tidak mengidentifikasi sender.<br>
d. Keduanya membuka data connection.<br>
e. From: adalah DNS record.<br>
f. Yang satu merupakan bagian dari message content; yang lain merupakan SMTP envelope command.

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: f.** Yang satu merupakan bagian dari message content; yang lain merupakan SMTP envelope command.<br>
*Penjelasan: Slide 2-65 membedakan header RFC 2822 (seperti "From:", "To:") yang merupakan bagian dari isi pesan, dengan command SMTP (seperti "MAIL FROM") yang digunakan untuk routing antar mail server.*
</details>

---

## 78. Pentingnya Web di 1990-an
Mengapa Web sangat penting bagi pertumbuhan Internet pada 1990-an?

a. Web menggantikan Internet protocol stack<br>
b. Web menghilangkan packet switching<br>
c. Web memerlukan circuit khusus untuk setiap pengguna<br>
d. Web membatasi penggunaan Internet hanya untuk universitas<br>
e. Web menciptakan platform yang mudah diakses untuk banyak aplikasi dan layanan komersial baru<br>
f. Web menghilangkan kebutuhan akan browser

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: e.** Web menciptakan platform yang mudah diakses untuk banyak aplikasi dan layanan komersial baru.<br>
*Penjelasan: Slide 1-82 mencatat sejarah awal 1990-an (Web, Mosaic/Netscape) yang memicu komersialisasi Internet dan melahirkan banyak "killer apps" baru.*
</details>

---

## 79. SMTP Command DATA
SMTP command mana yang menandai awal message content setelah sender dan recipient command?

a. RCPT TO<br>
b. USER<br>
c. DATA<br>
d. MAIL FROM<br>
e. GET<br>
f. QUIT

<details>
<summary><strong>Jawaban & Penjelasan</strong></summary>

**Jawaban: c.** DATA.<br>
*Penjelasan: Slide 2-63 (Sample SMTP interaction) menunjukkan urutan: HELO -> MAIL FROM -> RCPT TO -> DATA (untuk memulai transfer isi pesan) -> QUIT.*
</details>
