**LAPORAN PRAKTIKUM**

**PEMROGRAMAN WEB**

**Pratikum: Pratikum Semantik HTML dan CSS**

![A logo with a star and a wreath AI-generated content may be
incorrect.](media/image1.png){width="2.8194444444444446in"
height="2.8194444444444446in"}

Oleh:

Renald Kevin Azzaky (42430029)

**PROGRAM STUDI TEKNOLOGI INFORMASI**

**FAKULTAS TEKNIK DAN INFORMATIKA**

**UNIVERSITAS PENDIDIKAN NASIONAL**

**2025**

1.  **PENDAHULUAN**

> Semantic HTML merupakan praktik penulisan kode HTML dengan
> memanfaatkan elemen-elemen yang memiliki makna khusus sesuai fungsi
> konten yang ditampilkan. Tujuan utamanya adalah agar struktur dokumen
> dapat dipahami tidak hanya oleh pengguna manusia, tetapi juga oleh
> browser dan mesin pencari. Elemen semantik seperti \<header\>,
> \<footer\>, \<article\>, \<section\>, dan \<nav\> memberikan deskripsi
> eksplisit mengenai peran masing-masing bagian, berbeda dengan elemen
> generik seperti \<div\> atau \<span\> yang tidak memiliki makna
> khusus.
>
> Penerapan semantic HTML memberikan beberapa keuntungan, antara lain:

1.  **Aksesibilitas**: Membantu pengguna dengan keterbatasan tertentu,

    > khususnya yang menggunakan assistive technologies seperti _screen
    > reader_.

2.  **Optimasi Mesin Pencari (SEO)**: Memudahkan mesin pencari dalam

    > mengenali struktur dan bagian penting dari halaman, sehingga
    > berpotensi meningkatkan peringkat pencarian.

3.  **Keteraturan Kode**: Membuat struktur dokumen lebih rapi,
    > konsisten, serta lebih mudah dipelihara dalam jangka panjang.

> Dalam tugas pratikum ini, prinsip semantic HTML kami terapkan melalui
> pemilihan elemen yang tepat untuk setiap jenis konten, penyusunan
> hierarki heading secara logis, serta penambahan atribut aksesibilitas
> bila diperlukan. Dengan demikian, halaman web yang dibangun memiliki
> struktur yang jelas, konsisten, dan berorientasi pada pengalaman
> pengguna.
>
> Selain semantic HTML, CSS (Cascading Style Sheets) juga memiliki peran
> penting dalam perancangan tampilan halaman web. CSS digunakan untuk
> memisahkan antara struktur (HTML) dan presentasi (desain), sehingga
> pengembangan menjadi lebih fleksibel. Beberapa aspek yang kami
> terapkan melalui CSS meliputi:

- **Pengaturan Layout**: Pemanfaatan Flexbox dan CSS Grid untuk

  > menghasilkan tata letak yang terstruktur dan responsif.

- **Tipografi**: Penentuan jenis font, ukuran, serta spasi antar

  > elemen teks agar informasi mudah dibaca.

- **Warna dan Estetika**: Pemberian warna latar, pemilihan palet yang

  > konsisten, serta penambahan efek interaktif seperti _hover_.

- **Responsivitas**: Penyesuaian desain agar halaman dapat ditampilkan
  > secara optimal pada berbagai perangkat, mulai dari komputer
  > desktop hingga smartphone.

> Dengan mengombinasikan Semantic HTML dan CSS, struktur halaman web
> yang dihasilkan tidak hanya bermakna secara semantik dan mudah
> dipahami oleh mesin pencari, tetapi juga memiliki tampilan yang
> menarik, responsif, serta ramah bagi pengguna. Hal ini sekaligus
> menjadi fondasi yang kuat untuk pengembangan fitur interaktif
> menggunakan JavaScript pada tahap berikutnya..

2.  **PEMBAHASAN**

**Index.html**

![](media/image2.png)

- **Deklarasi dokumen** → Menandakan bahwa dokumen menggunakan standar
  HTML5.

- **Elemen html** → Menjadi pembungkus seluruh isi halaman, sekaligus
  menetapkan bahasa utama dokumen.

- **Bagian head** → Tempat meletakkan metadata, link eksternal, dan
  pengaturan halaman.

- **Meta charset** → Mengatur karakter encoding ke UTF-8 agar teks dan
  simbol tampil dengan benar.

- **Meta viewport** → Membuat tampilan halaman responsif di berbagai
  ukuran layar perangkat.

- **Link stylesheet** → Menghubungkan file CSS eksternal untuk
  mengatur desain dan tata letak.

- **Preconnect ke Google Fonts** → Mempercepat proses pemanggilan font
  dengan menyiapkan koneksi lebih awal.

- **Preconnect ke gstatic** → Menyediakan koneksi langsung ke server
  penyimpanan font, dengan dukungan akses lintas domain.

- **Link Google Fonts** → Mengimpor font tertentu (misalnya Roboto
  Slab) dengan variasi ketebalan dan opsi swap.

- **Title** → Menentukan judul halaman yang muncul di tab browser
  maupun hasil mesin pencari.

- **Penutup head** → Mengakhiri bagian head sebelum masuk ke body
  halaman.

![](media/image3.png)**Navigation Bar.html**

> .

- **Body** → Bagian utama halaman web yang berisi semua konten yang
  akan ditampilkan ke pengguna.

- **Nav** → Elemen navigasi yang menandakan bahwa bagian ini adalah
  menu untuk berpindah antar halaman atau bagian.

- **Div wrapper** → Pembungkus seluruh isi navigasi agar lebih mudah
  diatur tata letaknya dengan CSS.

- **Div name** → Menampilkan teks nama \"Kevin Azzaky\", biasanya
  digunakan sebagai identitas atau logo sederhana di navbar.

- **Div menu** → Bagian khusus untuk menampung daftar menu navigasi.

- **Ul (unordered list)** → Daftar tak berurutan yang digunakan untuk
  menyusun item menu.

- **Li dengan link Home** → Item pertama daftar yang berisi tautan
  menuju halaman utama.

- **Li dengan link Project** → Item kedua daftar yang mengarah ke file
  Project.html.

- **Li dengan link CV** → Item ketiga daftar yang mengarah ke file
  CV.html.

- **Penutup ul, div, dan nav** → Menutup daftar, kontainer menu,
  wrapper, dan akhirnya elemen navigasi

**Navigation.css**

![](media/image4.png)

- **wrapper**\
  Mengatur lebar kontainer sebesar 1024px, memposisikannya ke tengah
  dengan margin auto, serta memberi padding atas dan bawah agar isi
  tidak menempel ke tepi.

- **nav**\
  Memberikan warna latar belakang gelap (#17313e), menambahkan
  bayangan bawah dengan efek box-shadow, membuat posisi sticky agar
  selalu menempel di bagian atas saat di-scroll, serta memastikan
  berada di lapisan terdepan dengan z-index 100.

- **nav \> .wrapper**\
  Menjadikan isi wrapper di dalam nav sebagai flex container, mengatur
  jarak antar elemen secara merata (space-around), dan menetapkan
  ukuran font sebesar 1rem.

- **.menu**\
  Mengatur lebar area menu agar menempati 50% dari ruang yang
  tersedia.

- **.menu \> ul**\
  Menyusun daftar menu menggunakan flexbox, memberi jarak antar item
  dengan space-around, menghilangkan bullet list (list-style-type:
  none), serta menghapus margin dan padding bawaan.

- **ul \> li \> a**\
  Menghapus garis bawah pada link (text-decoration: none) dan
  mengganti warna teks menjadi putih.

- **.name**\
  Menampilkan teks nama dengan fleksibel menggunakan flexbox, memberi
  warna putih, dan mengatur agar isi tersebar merata di antara ruang
  (space-between).

- **.menu \> ul \> li \> a:hover**\
  Memberikan efek hover pada link menu: saat kursor diarahkan ke link,
  link tersebut mendapat padding tambahan 5px agar terasa interaktif.

**Section.html**

![](media/image5.png)

- **Section dengan class \"about\"**\
  Menandai sebuah bagian khusus di halaman yang berisi informasi
  tentang pemilik portofolio. Class about dipakai agar mudah diberi
  style melalui CSS.

- **Div dengan class \"header-opacity\"**\
  Elemen kosong yang kemungkinan digunakan untuk efek visual (misalnya
  transparansi atau overlay) pada bagian header.

- **Div dengan class \"header-about\"**\
  Wadah utama yang berisi konten teks di dalam section _about_.

- **Heading h4 \"Haloo\"**\
  Sebagai judul kecil atau sapaan pembuka untuk bagian perkenalan.

- **Paragraf \<p\>**\
  Berisi teks perkenalan pemilik portofolio (Renald Kevin Azzaky),
  termasuk latar belakang pendidikan, minat di bidang teknologi
  informasi, fokus pada web development (front-end, back-end, dan
  keamanan), serta motivasi pribadi dalam memanfaatkan teknologi untuk
  memberikan solusi.

- **Penutup paragraf, div, dan section**\
  Mengakhiri elemen teks, menutup kontainer, serta menutup section
  _about_.

> **Section.css**
>
> ![](media/image6.png)

- **Class .about**\
  Digunakan untuk mengatur tampilan latar belakang pada section
  _about_. Gambar dijadikan background, diposisikan di tengah, diatur
  agar menutupi seluruh area (cover) tanpa mengulang. Tinggi elemen
  dibuat 130vh agar lebih besar dari layar. Posisi relatif dipakai
  supaya elemen di dalamnya bisa diposisikan absolut.

- **Class .header-opacity**\
  Berfungsi sebagai lapisan hitam transparan di atas background.
  Memiliki warna hitam dengan opacity 0.5. Lebarnya dan tingginya 100%
  agar menutupi seluruh area section. Diposisikan absolut sehingga
  menempel penuh di bagian atas.

- **Class .header-about**\
  Menjadi wadah utama untuk teks perkenalan. Diposisikan absolut di
  dalam section, dengan jarak tertentu dari atas (top) dan kiri
  (left). Menggunakan flexbox dengan arah kolom agar teks tersusun
  vertikal.

- .**header-about \> h4**\
  Mengatur gaya untuk heading (judul "Haloo"). Warna putih supaya
  kontras, ukuran font besar (2rem), serta margin dan padding
  dihilangkan agar lebih rapi.

- .**header-about \> p**\
  Mengatur gaya teks paragraf perkenalan. Warna putih supaya terbaca
  jelas, margin dan padding dihilangkan. Ukuran font lebih kecil
  (15px), teks dibatasi lebar maksimum agar tidak melebar ke samping,
  dan diberi line-height 1.5 supaya nyaman dibaca.

**Footer.html**

![](media/image7.png)

- Class \"foter\"\
  Menjadi pembungkus untuk bagian footer. Meskipun ada tag \<footer\>,
  penggunaan class ini memungkinkan penambahan gaya (CSS) khusus bila
  diperlukan.

- Tag \<footer\>\
  Merupakan elemen semantik HTML yang digunakan khusus untuk bagian
  kaki (penutup) dari halaman atau section. Biasanya berisi informasi
  hak cipta, kontak, atau link tambahan.

- Tag \<div\>\
  Dipakai sebagai wadah (container) untuk menampung isi footer agar
  lebih mudah diatur dengan CSS, misalnya untuk posisi atau tata
  letak.

- Tag \<p\> dengan &copy;\
  Menampilkan teks hak cipta. Simbol &copy; secara otomatis dirender
  menjadi tanda ©. Teks yang ada menyatakan bahwa hak cipta website
  berlaku pada tahun 2025. Namun ada sedikit salah ketik, seharusnya
  "reserved" bukan "reseved"

**Footer.css**

![](media/image8.png)

- Class .foter\
  Digunakan untuk memberikan gaya khusus pada bagian footer website.

- background-color: #ddd;\
  Memberikan warna latar belakang abu-abu terang pada footer agar
  berbeda dengan bagian lain.

- padding: 10px;\
  Menambahkan jarak di dalam area footer antara teks dengan tepi
  elemen, sehingga terlihat lebih rapi dan tidak menempel langsung.

- text-align: center;\
  Membuat teks di dalam footer rata tengah secara horizontal, sehingga
  posisi hak cipta terlihat simetris di bagian bawah halaman.

**Project.html**

**Section project.html**

![](media/image9.png)

- Class \"portfolio\" dengan id=\"Project-1\"\
  Membuat sebuah section khusus untuk menampilkan proyek. Class
  portfolio dipakai untuk styling, sedangkan id berguna jika ingin
  dijadikan target navigasi (misalnya dari menu).

- Div \"project-hero\"\
  Berfungsi sebagai wadah atau header kecil untuk judul bagian proyek.
  Bisa diberi gambar atau gaya visual khusus di CSS.

- Heading \<h2\> \"My Project\"\
  Judul utama section yang menandakan daftar proyek akan ditampilkan
  di bawahnya.

- Div \"grid-container\"\
  Menjadi wadah utama untuk menampung semua item proyek. Biasanya
  digunakan bersama CSS Grid atau Flexbox agar tata letak proyek
  tersusun rapi.

- Div \"grid-item\"\
  Mewakili setiap kotak proyek individual. Di dalamnya ada:

- Heading \<h3\> untuk judul proyek (Project 1, Project 2, dst).

- Paragraf \<p\> berisi keterangan sementara \"soon.\" sebagai
  placeholder sebelum isi proyek asli ditambahkan.

- Penutup \</div\> dan \</section\>\
  Menutup kontainer grid dan section portfolio.

**Section project.css**

![](media/image10.png)

- Class .portfolio\
  Mengatur seluruh section portfolio agar teks rata tengah
  (text-align: center) dan memberi jarak di dalam section dengan
  padding atas-bawah 40px, kiri-kanan 20px.

- Selector .portfolio h2\
  Mengatur judul bagian proyek. Ukuran font 28px, jarak bawah 30px
  agar tidak terlalu menempel dengan isi, serta warna teks hitam.

```{=html}
<!-- -->
```

- Class .grid-container\
  Membuat wadah proyek berbentuk grid.

```{=html}
<!-- -->
```

- display: grid; → mengaktifkan grid layout.

- grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); → kolom
  akan otomatis menyesuaikan ukuran layar, minimal 250px, maksimal
  membagi rata ruang.

- gap: 20px; → jarak antar item grid.

- max-width: 1100px; dan margin: 0 auto; → membuat lebar maksimum
  1100px dan posisi di tengah halaman.

- padding: 10px; → memberi jarak dalam kontainer grid.

```{=html}
<!-- -->
```

- Class .grid-item\
  Mengatur tampilan tiap kotak proyek.

```{=html}
<!-- -->
```

- Latar belakang warna gelap #17313e.

- Sudut melengkung border-radius: 10px.

- Padding 15px agar isi tidak menempel ke tepi.

- box-shadow memberikan efek bayangan halus.

- transition mengatur efek animasi halus saat ada perubahan (misalnya
  hover).

```{=html}
<!-- -->
```

- Selector .grid-item h3\
  Mengatur judul proyek dalam setiap kotak. Margin diberi 10px 0 5px,
  ukuran font 20px, warna teks azure.

- Selector .grid-item p\
  Mengatur deskripsi proyek. Font-size 15px dan warna teks azure agar
  kontras dengan background.

```{=html}
<!-- -->
```

- Selector .grid-item:hover\
  Memberi efek interaktif saat kursor diarahkan ke kotak proyek.

```{=html}
<!-- -->
```

- transform: scale(1.05); → memperbesar sedikit item (zoom-in).

- box-shadow lebih tebal agar terlihat menonjol

**CV.html**

**Section CV.html**

![](media/image11.png)

**Section: About (Tentang)**

- section class=\"section-1\" id=\"About\": Membuka bagian utama
  tentang diri (About) dengan class untuk styling dan id untuk
  navigasi.

- h2Tentang saya : Judul sub-bagian \"Tentang saya\".

- P : Membuka paragraf yang berisi perkenalan diri, latar belakang
  pendidikan, minat utama (pengembangan web front-end dan back-end),
  motivasi belajar, dan harapan kontribusi di bidang teknologi
  informasi.

- P : Menutup paragraf.

- section : Menutup bagian About.

**Section: Biodata Diri**

- section class=\"section-1\" id=\"biodata\": Membuka bagian Biodata
  Diri.

- h2 Biodata Diri\</h2\>: Judul sub-bagian \"Biodata Diri\".

- P Nama : Renald Kevin Azzaky\</p\>: Menampilkan informasi **Nama**.

- p Email : kevinazzakyl@gmail.com\</p\>: Menampilkan informasi
  **Email**.

- p Tempat/Tanggal Lahir : Singaraja/27-03-2006\</p\>: Menampilkan
  informasi **Tempat/Tanggal Lahir**.

- section : Menutup bagian Biodata Diri.

**Section: Pendidikan**

- section class=\"section-1\" id=\"pendidikan\" : Membuka bagian
  Pendidikan.

- h2 Pendidikan\</h2\>: Judul sub-bagian \"Pendidikan\".

- ul : Membuka daftar tak berurut (_unordered list_) untuk riwayat
  pendidikan.

- li Sekolah Dasar MI Insan Mulia\</li\>: Item pertama: Pendidikan
  **SD**.

- li Sekolah Menengah Pertama SMP Negeri 2 Kuta Selatan\</li\>: Item
  kedua: Pendidikan **SMP**.

- li Sekolah Menengah Kejuruan SMK TI Bali Global Jimbaran\</li\>:
  Item ketiga: Pendidikan **SMK**.

- li Kuliah Universitas Pendidikan Nasional Denpasar\</li\>: Item
  keempat: Pendidikan **Kuliah**.

- ul : Menutup daftar tak berurut.

- section : Menutup bagian Pendidikan.

**Section: Skill**

- section class=\"section-1\" id=\"skill\" : Membuka bagian
  Keterampilan (Skill).

- h2 Skill h2 : Judul sub-bagian \"Skill\".

- p HTML\</p\>: Menampilkan keterampilan **HTML**.

- p CSS\</p\>: Menampilkan keterampilan **CSS**.

- p Javascript\</p\>: Menampilkan keterampilan **Javascript**.

- p Photoshop\</p\>: Menampilkan keterampilan **Photoshop**.

- p Figmas\</p\>: Menampilkan keterampilan **Figma** (ada kesalahan
  ketik, seharusnya Figma).

- Section : Menutup bagian Skill

**Section CV.css**

![](media/image12.png)

### Selektor .section-1 (Baris 1-6)

- **border: 1px solid #ddd;** (Baris 2): Memberi batas atau **bingkai
  tipis** di sekeliling setiap elemen yang menggunakan class
  section-1. Bingkai ini berukuran **1 pixel**, **solid** (garis
  penuh), dan berwarna **abu-abu muda** (#ddd).

- **padding: 15px;** (Baris 3): Memberi **jarak internal** (ruang
  kosong) sebesar **15 pixel** antara konten di dalam elemen (teks,
  judul, dll.) dengan bingkai (border) elemen tersebut.

- **margin: 20px 0;** (Baris 4): Memberi **jarak eksternal** (ruang
  kosong) sebesar **20 pixel** di bagian **atas** dan **bawah**
  elemen. Nilai 0 berarti tidak ada _margin_ di bagian kiri dan kanan.
  Ini berfungsi memisahkan antar _section_.

- **box-shadow: 0 0 5px #aaa;** (Baris 5): Membuat **efek bayangan**
  tipis di sekitar elemen untuk memberikan kesan kedalaman. Bayangan
  ini tidak memiliki offset horizontal atau vertikal (0 0), memiliki
  blur sebesar **5 pixel**, dan berwarna **abu-abu sedang** (#aaa).

### Selektor .section-1 (Baris 8-9)

- **.section-1** (Baris 8): Selektor ini adalah pengulangan dari yang
  di atas.

- **margin: 20px 0;** (Baris 9): Properti ini **mengulang** pengaturan
  _margin_ yang sama persis dengan yang sudah didefinisikan di Baris
  4, sehingga secara praktis **tidak memiliki efek tambahan** pada
  _styling_ kecuali menimpa nilai sebelumnya jika ada konflik (namun
  dalam kasus ini nilainya sama). Dalam kode yang efisien, baris ini
  seharusnya dihapus.

3.  **KESIMPULAN**

> Praktikum ini berhasil mengimplementasikan penggunaan Semantic HTML
> bersama dengan **CSS** untuk membangun halaman web yang terstruktur
> dan terdesain dengan baik. Semantic HTML (menggunakan elemen seperti
> \<nav\>, \<section\>, dan \<footer\>) diterapkan untuk memberikan
> makna yang jelas pada setiap bagian konten, yang meningkatkan
> aksesibilitas dan mendukung SEO. CSS digunakan untuk mengatur
> presentasi dan tata letak, termasuk penerapan Flexbox dan CSS Grid
> untuk menghasilkan struktur halaman yang responsif dan terorganisir.
> Sinergi kedua teknologi ini menghasilkan halaman web yang tidak hanya
> bermakna secara kode, tetapi juga memiliki tampilan menarik,
> konsisten, dan optimal di berbagai perangkat.

**LAMPIRAN**

Tampilan halaman home (index.html)

![](media/image13.png){width="5.8144881889763775in"
height="3.058817804024497in"}

Tampilan halaman project (Project.html)

![](media/image14.png){width="6.5in" height="3.415277777777778in"}

Tampilan halaman (CV.html)

![](media/image15.png){width="6.5in" height="3.4194444444444443in"}

Tampilan footer

![](media/image16.png){width="6.5in" height="0.3659722222222222in"}
