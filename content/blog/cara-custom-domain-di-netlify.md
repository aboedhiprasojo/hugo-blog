---
title: "Cara Custom Domain Di Netlify"
date: 2021-05-21T02:49:56+07:00
draft: false
type: post

tags: 
    - tutorial
    - blog
    - internet
---

Hingga saat ini membuat website memanglah suatu kebutuhan penting. Apalagi di Era Digital seperti saat ini. Mulai dari kepentingan sharing pengalaman, berbagi informasi, berjualan, dll bisa dilakukan melalui website. Netlify adalah salah satu platform yang dapat men-deploy website dengan mudah dan cepat. Namun jika kita men-deploy kesana, maka akan menggunakan sub-domain dari mereka. Pada artikel kali ini saya akan sharing tentang bagaimana cara untuk mengarahkan domain yang kita beli sendiri untuk mengarahkan ke sub-domain Netlify. Tapi sebelum itu alangkah baiknya kita berkenalan terlebih dahulu sama tuan rumah kita, mari kita sambut ini dia Netlify.

### Apa Itu Netlify.

`Netlify` adalah suatu platform yang bisa kalian manfaatkan untuk membangun website, sebelum itu bisa kalian cek langsung di [netlify](https://www.netlify.com/). Dengan netlify, kalian bisa dengan mudah men-deploy, mengkolaborasikan, mengintegrasikan, bahkan mengkustomisasikan website dengan beberapa anggota dalam satu tim. Netlify menerapkan arsitektur pengembangan web modern yang disebut dengan `JAMstack`. Arsitektur ini berbasis Javascript, API, dan Markup. Arsitektur berbasis Javascript itu artinya Netlify support dengan variasi framework Javascript seperti *ReactJS, VueJS, NextJS, dan NuxtJS*. Selain itu dapat men-deploy website yang menggunakan API. Dengan menggunakan Netlify kinerja dan performa website akan lebih cepat.

### Kelebihan Dari Netlify

Adapun beberapa kelebihan yang bisa kalian gunakkan jika men-deploy website di netlify adalah sebagai berikut:

- Kolaborasi tim dapat dilakukan dengan mudah karena menggunakan sistem manajemen pengembangan yang populer seperti Github dan Gitlab.
- Bisa support website yang bersifat statis (HTML)
- Deployment website dengan mudah, hanya meng-upload, meng-konfigurasi, dan website sudah siap.
- Bisa menambahkan plugin yang telah disediakan oleh Netlify.

Nah, selanjutnya masuk ke inti dari materi pembahasan ini, yaitu bagaimana sih cara custom Domain ke Netlify. Oke langsung saja, cekibroott.

### Cara Custom Domain Ke Netlify
Bebarapa langkah- langkah yang harus kalian lakukan untuk melakukan custom domain ke Netlify adalah:

1. Login Ke Akun Netlify

Petama-tama yang harus kalian lakukan adalah login ke akun netlify. Kalian bisa langsung mengakses ke [netlify.com](https://www.netlify.com/) dan meng-klik `login`. Kemudian kalian tinggal pilih mau login menggunakan cara apa. Mau menggunakan *Github, Gitlab, Bitbucket, atau Email.* Jika sudah, tinggal ikutin saja prosedurnya 😊

![Halaman Login](/img/custom-domain/halaman-login-netlify-1.png)

2. Memilih Menu Sites

Setelah berhasil login, kalian bisa memilih menu `Sites` untuk menentukan website mana yang akan kalian custom domain. 

![Halaman Utama Netlify](/img/custom-domain/halaman-utama-netlify.png)

3. Memilih Website Project

Nah, pada tutorial ini adalah saya memilih nama project `sangito.` Maka nantinya akan berada di dashboard setting websitemu. Disini kalian bisa melakukan setting struktur website dan setting domain. Untuk melakukan custom domain, silahkan kalian klik `Domain Setting.`

![Halaman Setting Domain Netlify](/img/custom-domain/Frame-159.png)

4. Mengisi Nama Domain

Selanjutnya cari bagian `Custom Domains` jika sudah ketemu klik `Add custom domain.`

![Halaman Setting Domain Netlify](/img/custom-domain/Frame-160.png)

Kemudian akan muncul halaman baru seperti gambar di bawah ini. Lalu kalian isikan nama domain.

![Halaman Setting Domain Netlify](/img/custom-domain/Frame-161.png)

Dalam melakukan custom domain kalian bisa menggunakan domain utama atau subdomain. Jika kalian menggunakan domain utama maka tuliskan nama domain utama tersebut. Begitu sebaliknya, jika kalian ingin menggunakan subdomain tuliskan subdomain yang akan diarahkan. Sebagai contohnya, pada panduan kali ini saya menggunakan domain utama [aboedhiprasojo.com](https://aboedhiprasojo.com/). Jika kalian mau menggunakan subdomain, maka isikan `sangito.aboedhiprasojo.com.`

5. Login Ke Penyedia Jasa Layanan Hosting/Domain

Nah, kalian telah melakukan custom domain dari sisi akun Netlify. Sekarang saatnya melakukan custom domain dari sisi penyedia jasa domain-nya. Pertama kalian harus login dulu ke client area penyedia jasa-nya. Sebagai contohnya saya menggunakan jasa DomaiNesia. Jika kalian sama menggunakan domainNesia bisa langsung klik [disini](http://my.domainesia.com/). Disini saya tidak di-endors ya ☺️

![Halaman Login Jasa Layanan](/img/custom-domain/Frame-162.png)

6. Menambahkan CNAME Record dan A Record

Langkah selanjutnya adalah melakukan pengaturan DNS Record untuk domain atau subdomain kalian. Dalam melakukan custom domain, kalian bisa menggunakan domain utama atau subdomain. Kalian bisa memilih salah satu antara **domain utama atau subdomain**. Karena disini saya memakai domain utama ya saya tulis tentang custom domain utama 😁

7. Mengatur CNAME Record

Untuk mengatur CNAME Record pada domain utama, kalian bisa klik menu `Domains.`

![Halaman Login Jasa Layanan](/img/custom-domain/Frame-163.png)

Kemudian pilih nama domain kalian.

![Halaman Login Jasa Layanan](/img/custom-domain/Frame-164.png)

Setelah itu pilih menu `Addons.`

![Halaman Login Jasa Layanan](/img/custom-domain/Frame-165.png)

Pada *Addons* ada berbagai macam pilihan, kalian bisa pilih **DNS Zone Manager** dan klik `Manage.`

![Halaman Login Jasa Layanan](/img/custom-domain/Frame-166.png)


Kemudian tambahkan DNS Record baru dengan mengisikan `www` sebagai **Host name**. Selanjutnya pilih `CNAME` pada kolom **Type**. Terakhir masukkan alamat website netlify kalian misalnya disini adalah `sangito.netlify.app` pada kolom **Address/Value** dan klik `Save Changes.`

![Halaman Login Jasa Layanan](/img/custom-domain/Frame-167.png)

Sama halnya DNS Record, untuk A Record juga sama. Tambahkan DNS Record baru dengan mengisikan `@` pada kolom **Host name**. Selanjutnya pilih `A` pada kolom **Type**. Terakhir masukkan alamat IP Netlify 104.198.14.52 pada kolom **Address/Value** dan klik `Save Changes.`

![Halaman Login Jasa Layanan](/img/custom-domain/Frame-168.png)

Atau bisa menggunakan cara lain seperti berikut..

### Cara Custom Domain 

1. Masuk Ke Domain Setting

Langkah pertama kalian masuk dulu ke `site`, lalu kalian masuk `Domain settings` maka akan muncul tampilan seperti berikut. Kemudian kalian klik saja menu `Options.`

![Halaman Setting](/img/custom-domain/Frame-169.png)

2. Set Up Netlify DNS Domain

Langkah selanjutnya maka akan tampil seperti berikut. Pastikan nama domain kalian disini sudah benar ya 😉

Jika sudah benar, kalian langsung saja klik `Verify.`

![Halaman Setting DNS Domain](/img/custom-domain/Frame-170.png)

3. Set Up Netlify DNS Record

Untuk langkah ini, maka akan otomatis terisi. Jika kalian mau menambahkan **DNS record baru** silahkan bisa klik `Add New Record.` Jika sudah yakin, bisa kita lanjut klik saja `Continue.`

![Halaman Setting DNS Record](/img/custom-domain/Frame-171.png)

4. Set Up Netlify Domain NameServer

Untuk langkah ini, kita disuruh mengisi nameserver ke dalam layanan jasa domain kita. Kita Skip saja bagian ini dulu.

![Halaman Setting nameserver](/img/custom-domain/Frame-172.png)

5. Setting Name Server

Masuk ke Cpanel kalian, lalu masuk ke menu `Nameserver.`

![Halaman Setting nameserver Cpanel](/img/custom-domain/Frame-173.png)

6. Isi Name Server

Nah, disini kalian copy saja satu per satu dan pastekan ke Cpanel kalian.

![Halaman Setting nameserver Cpanel](/img/custom-domain/Frame-174.png)

Sebagai contohnya adalah seperti berikut ini...

![Halaman Setting nameserver Cpanel](/img/custom-domain/Frame-175.png)

Jika sudah terisi semua, bisa kalian klik `Change Nameservers.`

### Custom Domain ke Netlify Berhasil

Setelah semua langkah diatas dilakukan, saatnya mengecek apakah custom domain kalian berhasil dilakukan. Kalian bisa langsung akses nama domain utama atau subdomain yang dijadikan custom domain tadi di Address Bar browsermu. Jika muncul tampilan website yang kalian punya, itu artinya custom domain ke Netlify telah berhasil. Eiitss, saat-nya kita hubungkan ke HTTPS, terlihat bahwa domain kita masih belum menggunakan HTTPS...

...Jadi, sekarang kita aktifkan dulu HTTPS di domain Netlify menggunakan Let’s Encrypt. Di dashboard Netlify, klik tombol `Domain Settings.`

![Halaman Setting Domain](/img/custom-domain/Frame-159.png)

Cari **HTTPS** di menu yang ada di sebelah kiri, lali klik tombol `Verify DNS Configuration.` 

Selanjutnya, klik tombol `Let’s Encrypt certificate.` 

Dan terakhir saat muncul dialog **Automatic TLS Setup**, kalian klik saja tombol `Provision certificate.` 

Karena disini saya lupa untuk men-sekrinsut gambarnya, jadi saya ambil bagian ininya saja ya ☺️

![Halaman Setting https](/img/custom-domain/Frame-176.png)

Tunggu beberapa saat hingga proses pemasangan sertifikat berhasil.

![Halaman Setting https](/img/custom-domain/Frame-177.png)

Tunggu lagi hingga beberapa menit dan coba refresh browser yang sedang membuka domain kita. Perhatikan bahwa akses HTTPS sudah berhasil dengan tanda gembok hijau dan teks Secure yang menandakan pemasangan sertifikat Let’s Encrypt berjalan dengan baik.

![Halaman cek domain dan https](/img/custom-domain/Frame-178.png)

### Penutup

Custom domain ke netlify dapat dilakukan dengan mudah, tapi syaratnya kita harus punya akun dari netlify dan mempunyai domain sendiri. Buat kalian yang belum punya domain, cepat-cepatlah beli domain 😅

Nah, sekarang setiap kali kita akan membuat **Post Baru** dan melakukan push ke Github, secara otomatis netlify akan mendeteksinya lalu akan menjalankan perintah yang men-*generate* halaman statis dari file **markdown** yang kita tulis. 

