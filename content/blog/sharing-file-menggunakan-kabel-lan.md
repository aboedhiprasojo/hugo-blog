---
title: "Sharing File Menggunakan Kabel Lan"
date: 2022-04-04T22:53:37+07:00
draft: true

tags: 
    - tutorial
    - blog
    - internet
    - komputer
---

Sedikit mau sharing pengalaman saya dari tahun ke tahun, dan terakhir kemarin saya menemui sebuah problem baru bahwa saya mau share file PES Terbaru dari laptop ke PC rumah menggunakan flashdisk. Namun ternyata itu gak bisa karena size terlalu besar. Saya pindah karena spek PC rumah sedikit memadai daripada di laptop saya.

![Folder PES](/img/sharing-data/Size.png)

Cara ini sebenernya digunakan jika problem yang dialami itu sama seperti saya. Nantinya kita akan menggunakan Sharing File tersebut menggunakan kabel LAN atau yang sering disebut **Ad-Hoc**. Ad-Hoc ini adalah koneksi jaringan sementara yang dibuat untuk tujuan tertentu ya contohnya seperti tadi, mentransfer data dari satu PC/Laptop ke PC/Laptop lain.


Nah sebelum lanjut ke tutorialnya, kita berkenalan dulu ya. Tak kenal maka tak sayang. Cekibrot...

Kabel LAN adalah salah satu jenis media transmisi yang sering kita gunakan. Mulai dari membuat jaringan komputer, menghubungkan ke Router, menghubungkan komputer ke printer dan lainnya.


## Jenis Kabel LAN

1. **Kabel UTP (Unshielded Twisted Pair)**

	Kabel LAN ini juga sering kali disebut dengan kabel Twisted Pair. Umumnya, kabel ini secara khusus digunakan untuk mengurangi kebisingan. Maka dari itu, jenis kabel inilah yang paling banyak digunakan untuk membuat jaringan lokal.

	![Jenis Kabel UTP](/img/sharing-data/jenis-kabel-utp.png)

	Kabel twisted pair adalah jenis kabel dengan pilihan yang paling hemat biaya dari ketiganya, tetapi juga transmisi Bandwidth-nya lebih rendah serta mempunyai redaman yang tinggi.

2. **Kabel Coaxial**

	Berbeda dengan kabel UTP tadi, kabel ini justru lebih banyak terbuat dari kawat tembaga. Diluar kawat tembaga terdapat pelindung yaitu berupa isolator, konduktor, hingga bahan PVC.

	![Kabel Coaxial](/img/sharing-data/kabel-coaxial.png)

	Kabel coaxial adalah jenis kabel transmisi frekuensi tinggi yang terdiri dari tembaga padat tunggal, dimana data di transfer secara elektrik melalui konduktor dalam dan memiliki kapasitas transmisi 80x lebih besar dari kabel twisted pair. Dan kini penggunaannya lebih banyak oleh kabel twisted pair, maka dari itu kabel ini sudah kian jarang ditemui di berbagai tempat.

3. **Kabel Fiber Optik**

	Kabel ini adalah teknologi terbaru dalam kabel transmisi, daripada menstransfer data melalui kabel tembaga, kabel fiber optik ini mengandung serat optik dan bisa mentransmisikan data melalui cahaya.

	Dan terbukti koneksi sangatlah super cepat yang memiliki kapasitas transmisi data 26.000x lebih banyak dibandingkan kabelb twisted pair. Dan bisa dikatakan untuk saat ini kabel fiber optik-lah jenis kabel terbaik, namun dalam sisi pembangunan jaringan kabel ini sangatlah mahal.

	![Kabel Fiber Optik](/img/sharing-data/kabel-fiber-optik.png)


Selain itu kabel LAN juga memiliki berbagai macam jenisnya lagi yang terdiri dari kabel Straight-Through, kabel Cross-Over, dan kabel Roll-Over. Nah ketiga kabel ini juga memiliki fungsi dan kegunaan yang berbeda loh. Namun untuk melakukan sharing file dan folder ke sesama komputer ataupun sharing file ke printer bisa menggunakan **kabel Straight**. 

Nah di artikel ini, saya ingin membahas pengalaman saya yang juga nggak boleh dilewatkan untuk kalian, yaitu *sharing file* menggunakan kabel LAN.

Untuk kalian yang ingin mencobanya, disini saya buat tutorialnya.. Silahkan disimak sampai selesai langkah demi langkahnya.

### Persiapan Bahan

- Pertama jelas dong ya siapkan terlebih dahulu kabel LAN + RJ45. Disini saya menggunakan **kabel Straight** ya. Jika kalian belum punya bisa beli di toko komputer, yah kisaran harga 20 ribuan tergantung wilayah. Jadi silahkan disesuaikan budget kalian ya.
- Kedua jelas kita membutuhkan PC/laptop-nya.

### Proses Konfigurasi

Setelah semua bahannya sudah lengkap, sekarang ikuti langkahnya yang akan saya bagikan.

Disini saya akan menjelaskan se-detail mungkin agar kalian lebih mudah memahami dan mempraktekkan sendiri. Nah pada tutorial ini, saya menggunakan Windows 10 ya, untuk windows lain pun kemungkinan sama, tinggal disesuaikan saja.

**Langkah 1: Mengatur kedua PC/Laptop terlebih dahulu**

Silahkan kalian nyalakan kedua alat PC/Laptop yang akan digunakan nantinya, lalu jika sudah sambungkan menggunakan kabel LAN. 

Kenapa harus 2 alat PC/Laptop bang?? 

Okeh, jadi gini.. PC/Laptop yang pertama itu digunakan untuk share file penting yang ingin dibagikan (Server), lalu yang PC/Laptop yang kedua itu digunakan untuk mengakses file (meng-copy file jika dibutuhkan). Sampai sini semoga mudeng ya 😄.

Nah silahkan kalian perhatikan gambar dibawah ya. Yang tadinya tanda silang merah (Unplugged) akan berubah menjadi tanda seru berwarna kuning. 

![Share Data LAN](/img/sharing-data/Share-Data-LAN.png)

Selanjutnya, ikuti  langkah-langkah berikut ya.

- Di PC/Laptop pertama, kalian klik bagian bawah seperti gambar, lalu klik `Open Network & Internet settings`

![Share Data LAN](/img/sharing-data/Share-Data-LAN-01.png)

- Jika sudah silahkan cari dan klik `Network and Sharing Center`

![Share Data LAN](/img/sharing-data/Share-Data-LAN-02.png)

- Selanjutnya kalian klik `Change adapter settings`

![Share Data LAN](/img/sharing-data/Share-Data-LAN-03.png)

- Pilih koneksi LAN yang telah terdeteksi otomatis (biasanya bernama Local Area Connection atau Ethernet). Klik kanan pada LAN yang terdeteksi tadi (disini punya saya Ethernet ya, jika beda silahkan disesuaikan)

![Share Data LAN](/img/sharing-data/Share-Data-LAN-04.png)

- Jika sudah klik kanan tadi, kalian klik `Properties` lalu pilih cari dan klik `Internet Protocol Version (TCP/IPv4)`. Nah jika muncul tampilan baru silahkan kalian isikan dengan IP Address bebas ya. Oh iya untuk mengisi IP Address silahkan klik radio button `Use the following IP Address`. 

![Share Data LAN](/img/sharing-data/Share-Data-LAN-05.png)

- Isikan IP Address-nya ya. Silahkan kalian mau mengikuti IP dari saya monggo, mau bebas monggo. Asalkan sesuai dengan aturan Class IP Address ya yaitu Class A, Class B, Class C. Jika sudah di isi silahkan klik OK.

![Share Data LAN](/img/sharing-data/Share-Data-LAN-06.png)

- Nah silahkan kalian buka PC/Laptop yang kedua,, lalu lakukan konfigurasi langkah seperti diatas. Caranya sama kok 😄

- Nah ini adalah konfigurasi IP Address milik PC/Laptop dari saya. Lagi dan lagi saya ingatkan, silahkan kalian mau mengikuti IP dari saya monggo, mau bebas monggo. Asalkan sesuai dengan aturan Class IP Address ya yaitu Class A, Class B, Class C. Jika sudah di isi silahkan klik OK. 

![Share Data LAN](/img/sharing-data/Share-Data-LAN-07.png)

**Langkah 2: Mengatur Sharing Network Options pada Control Panel**

Pengaturan inilah yang sangat penting. Kalau tidak di setting, nanti *folder* yang akan kita share juga tidak akan muncul di PC/Laptop client (Kedua). Dan otomatis kita juga tidak bisa meng-copy data tersebut kan.

Okeh, tanpa banyak cingcong, yuk simak tutorial lanjutannya ya.

- Silahkan masuk kembali ke `Change advanced sharing settings`

![Share Data LAN](/img/sharing-data/Share-Data-LAN-08.png)

- Pada langkah ini, kalian lakukan pengaturan seperti berikut ya :

![Share Data LAN](/img/sharing-data/Share-Data-LAN-09.png)

Pilih **Turn On Network Discovery**

Pilih **Turn On File and Printer Sharing**

Pilih **Turn On Public Folder Sharing**

Pilih **Turn Off Password Protected Sharing**
	
> Sesuaikan settingan seperti yang kalian inginkan ya 😄

- Setelah setting konfigurasi sharing datanya, silahkan kalian `Save Changes`.. Oh iya lupa, lakukan cara ini di kedua PC/Laptop kalian.

**Langkah 3: Mengatur & Menyiapkan Folder yang ingin di Share**

Langkah terakhir nih, kita harus mengatur dulu settingan foldernya yang akan dibagi ke PC/Laptop client (Kedua). Nah contohnya disini saya akan share folder PES Update Terbaru ke PC rumah (client), berikut tutorialnya.

- Pertama kalian tentukan dulu nih File/Folder mana yang ingin di share. Dalam artian seperti ini.. Disini kan saya akan share Folder PES Update Terbaru ke PC rumah (client), nah Folder PES Update Terbaru tersebut berada di laptop utama katakanlah (server). Jadi pengaturan Folder yang akan saya setting adalah di laptop utama tadi ya, berdasarkan Folder yang ingin di share. Begitu juga nanti kalian, tentukan dulu dimana File/Folder mana yang ingin di share dan siapa yang akan menerimanya tersebut. Okeh, semoga paham ya 😄

- Lanjut, klik kanan pada Folder yang di-inginkan tadi.. lalu klik `Properties`

![Share Data LAN](/img/sharing-data/Share-Data-LAN-10.png)

- Nantinya akan muncul sebuah tab baru yang bernama **Folder Sharing Properties**. Nah pada saat pertama kali muncul kan kalian masih berada di tab **General**, kalian klik saja menu `Sharing` lalu kalian cari button Share. Nah jika sudah ketemu tinggal kalian klik saja.

![Share Data LAN](/img/sharing-data/Share-Data-LAN-11.png)

- Jika muncul tab barau lagi yang bernama File Sharing, kalian masuk ke kolom menu pencarian lalu cari dan pilih `Everyone`.. jika sudah silahkan klik Add.

![Share Data LAN](/img/sharing-data/Share-Data-LAN-12.png)

- Terakhir nih kalian ubah pengaturan sharing-nya menjadi `Read/Write`.. jika sudah silahkan klik Share.

![Share Data LAN](/img/sharing-data/Share-Data-LAN-13.png)

Nah untuk konfigurasi setelan kan sudah, sekarang nih **bagaimana cara akses File atau Folder yang sudah di share tadi ?** Okeh, tenang. Begini cara aksesnya versi saya.

- Nah setelah kalian tadi meng-klik button share, kan nantinya akan muncul tab baru tuh yaitu letak akses File atau Folder yang kita share tadi.. nah kalian ingat dan catat itu, nantinya letak alamat tersebut yang nantinya kita eksekusi.

![Share Data LAN](/img/sharing-data/Share-Data-LAN-14.png)

- Okeh anggep saja langkah pertama tadi aman. Nah karena saya tadi saya menggunakan PC rumah (client), jadi saya akses menggunakan PC rumah tadi. Jika kalian berbeda silahkan disesuaikan. Klik tombol `Windows + R` kemudian ketikkan letak alamat yang tadi ya. Atau semisal kalian lupa nih, bisa kok menggunakan IP Address PC/Laptop utama atau kedua. Tapi menurut saya lebih enak dan cepet menggunakan alamat yang tadi.

![Share Data LAN](/img/sharing-data/Share-Data-LAN-15.png)

- Nah ini adalah folder PES Update Terbaru yang di share Laptop pertamaa dan sudah saya akses di PC rumah. Dan yah, saya bisa meng-copas folder ini dengan mudah, tenang tanpa memikirkan size penyimpanan flashdisk sisa berapa 😅

![Share Data LAN](/img/sharing-data/Share-Data-LAN-16.png)

### Akhir Kata

Dengan demikian sedikit curhatan catatan kecil mengenai tutorial cara sharing data menggunakan kabel LAN. Cara-cara diatas murni dari pengalaman saya sendiri, dan bahkan pada pembuatan tutorial ini bisa mencapai size besar kan yaitu 15 GB, lihat bukti ada pada foto paling atas. 

