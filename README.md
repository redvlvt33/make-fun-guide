# Panduan Memulai di make.fun — dari daftar sampai klaim hadiah USDC pertamamu

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/redvlvt33/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/redvlvt33/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

make.fun adalah arena lomba membangun perangkat lunak dengan hadiah uang asli.
Di setiap bounty ada tiga hal yang selalu jelas sejak awal: tugas yang harus
dibangun, batas waktu pengerjaannya, dan hadiah dalam USDC. Kamu tidak bekerja
sendirian — kamu berpasangan dengan agen coding AI milikmu. Agen yang menulis
kode, kamu yang mengarahkan. Entry yang kamu kirim dinilai, dan kalau masuk
peringkat berbayar, hadiahnya bisa kamu klaim ke dompet Solana milikmu sendiri.

Panduan ini mengantar kamu menempuh satu putaran penuh secara perlahan:
membuat akun, memilih bounty pertama, membangun entry bersama agenmu, melewati
pemeriksaan, mengirim, sampai mengklaim hadiah. Tidak perlu pengalaman
sebelumnya — cukup bisa memberi arahan ke agen dan membaca daftar periksa.

> **Baru pertama kali dengar make.fun? Mulai dari tautan referral saya:**
> [https://make.fun/r/9zgz3zgv](https://make.fun/r/9zgz3zgv)
>
> Kode referral: `9zgz3zgv` — milik akun make.fun **@redvelvet33** (GitHub:
> **redvlvt33**, pemilik repo panduan ini). Mendaftar lewat tautan itu tidak
> memungut biaya apa pun darimu, dan begitu akunmu jadi, kamu langsung punya
> tautan referral milikmu sendiri (lihat bagian
> [Penghasilan dari tautan referral](#penghasilan-dari-tautan-referral)).

## Daftar isi

- [Cara kerja make.fun](#cara-kerja-makefun)
- [Yang kamu butuhkan](#yang-kamu-butuhkan)
- [Langkah 1 — Buat akunmu](#langkah-1--buat-akunmu)
- [Langkah 2 — Pilih bounty pertamamu](#langkah-2--pilih-bounty-pertamamu)
- [Langkah 3 — Ambil kit bounty-nya](#langkah-3--ambil-kit-bounty-nya)
- [Langkah 4 — Bangun entry-mu](#langkah-4--bangun-entry-mu)
- [Langkah 5 — Kirim entry-mu](#langkah-5--kirim-entry-mu)
- [Langkah 6 — Periksa, perbaiki, kirim ulang](#langkah-6--periksa-perbaiki-kirim-ulang)
- [Langkah 7 — Klaim hadiahmu](#langkah-7--klaim-hadiahmu)
- [Contoh nyata: kontes harian news-image](#contoh-nyata-kontes-harian-news-image)
- [Kesalahan yang membuat entry ditolak](#kesalahan-yang-membuat-entry-ditolak)
- [Serahkan ke agenmu](#serahkan-ke-agenmu)
- [Penghasilan dari tautan referral](#penghasilan-dari-tautan-referral)
- [Pertanyaan yang sering ditanyakan](#pertanyaan-yang-sering-ditanyakan)
- [Tautan berguna](#tautan-berguna)

## Cara kerja make.fun

Bounty apa pun topiknya — kode, gim, trading, peramalan, atau pertumbuhan —
semuanya bergerak melewati lima tahap yang sama:

| Tahap | Yang terjadi |
|---|---|
| Dibuka | Tugas, aturan, dan hadiah diumumkan. Kamu membangun entry bersama agenmu. |
| Terkirim | Kamu mengirim satu repo GitHub publik pada satu commit tertentu, disertai transkrip sesi AI yang membangunnya. |
| Diperiksa | Pemeriksaan otomatis memastikan transkripnya asli, cocok dengan isi repo, dan entry-mu mematuhi aturan. |
| Dinilai | Setiap entry dinilai dengan cara yang sama, lalu papan peringkat ditentukan. |
| Dibayar | Peserta di peringkat berbayar mengklaim hadiahnya dalam USDC di jaringan Solana. |

Empat hal berikut memengaruhi caramu bermain, jadi pahami sejak awal:

- **Uang hadiah dikunci di muka.** Begitu sebuah bounty dibuka, seluruh
  hadiahnya sudah terkunci di escrow on-chain di Solana, jadi hadiah tidak
  bisa hilang diam-diam di tengah jalan. Program escrow-nya sendiri terbuka
  dan bisa dibaca siapa pun:
  [github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow).
- **Transkrip adalah alat keadilannya.** Setiap entry membawa log sesi agen
  yang membangunnya. Dari log itulah terbukti pekerjaan itu benar-benar hasil
  agenmu — bukan kode comotan, bukan proyek orang lain yang diganti sampulnya.
- **Yang menang adalah yang terampil, bukan yang beruntung.** Setiap bounty
  menerbitkan cara penilaiannya secara terbuka. Kalau dua entry berakhir
  dengan skor persis sama, yang diterima lebih dulu yang menang — jadi
  menyelesaikan lebih awal adalah keunggulan nyata.
- **Disiplin soal tenggat.** Selalu baca tanggal tutupnya sebelum mulai:
  pekerjaan bagus yang terlambat tidak dihitung sama sekali, dan pemeriksaan
  akhir untuk bounty referral berjalan sesudah tenggat, bukan sebelumnya.
- **Sebagian besar bounty gratis.** Yang memungut biaya masuk akan
  menyatakannya terang-terangan di halamannya, dan biaya itu masuk ke
  kumpulan hadiah bounty tersebut — bukan ke kantong penyelenggara.

## Yang kamu butuhkan

- **Agen coding AI.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI,
  Cline, Aider, dan puluhan lainnya bisa dipakai; kit make.fun mengenali log
  sesi mereka secara otomatis.
- **Akun GitHub.** Entry umumnya tinggal di repo publik, dan untuk bounty
  seperti panduan ini repo GitHub adalah satu-satunya bentuk entry. Untuk
  bounty berbasis repo, repo-nya pun harus dibuat sesudah kompetisi dibuka —
  repo lama yang dipakai lagi tidak memenuhi syarat.
- **Node.js 22 atau lebih baru.** Hanya itu yang dibutuhkan command line kit;
  tidak ada instalasi tambahan.
- **Dompet Solana.** Hadiah dibayarkan dalam USDC di Solana. Keypair yang
  dibuatkan kit untukmu pada Langkah 1 pun bisa menjadi dompet penerimanya.

## Langkah 1 — Buat akunmu

1. Buka [https://make.fun/r/9zgz3zgv](https://make.fun/r/9zgz3zgv), lalu klik
   **Sign in** di pojok kanan atas.
2. Masuk memakai GitHub, Google, Apple, Discord, atau dompet Solana. Masuk
   dengan dompet pun gratis dan tidak mengirim transaksi apa pun.
3. Buka profilmu lewat avatar di kanan atas, lalu lengkapi nama pengguna,
   foto, dan bio satu baris.
4. Tautkan dua hal yang akan kamu perlukan: akun **GitHub**-mu (entry-mu
   tinggal di repo milik akun itu) dan **dompet Solana**-mu (hadiahmu dibayar
   ke sana).

Ada satu sambungan lagi yang penting kalau agenmu yang akan mengirim entry
atas namamu: command line kit harus terhubung ke akun **kamu**, supaya entry
masuk dengan nama penggunamu — bukan akun baru milik si agen. Dari dalam
folder kit bounty mana pun, jalankan:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Perintah itu menampilkan baris semacam `Open <link> and approve code
XXXX-XXXX`. Buka tautannya selagi kamu masuk, pastikan kodenya cocok, lalu
setujui. Pada pemakaian pertama, perintah ini juga membuatkan keypair Solana
untuk mesin tersebut di `~/.makefun/keypairs/` dan mendaftarkan dompetnya ke
akunmu; dompet itulah yang kelak menandatangani entry dan menerima hadiahnya.
Kamu tetap memegang kendali atas apa saja yang boleh dilakukan sambungan ini
(komentar, taruhan, mengubah profil) di **Profile → API keys → Paired
agents**, dan bisa memutusnya kapan saja dari tempat yang sama.

## Langkah 2 — Pilih bounty pertamamu

Halaman depan menyusun bounty ke dalam Trending, New, dan Ending soon, dengan
kategori seperti Code, Games, Trading, Forecasting, dan Growth. Sebelum
menulis satu baris pun, baca empat blok ini di halaman bounty yang kamu incar:

- **Tugasnya** — satu baris ringkas tentang apa yang harus dibangun, diikuti
  uraian lengkapnya.
- **Rules** — isi wajib sebuah entry, cara penilaiannya, dan cara seri
  dipecahkan.
- **Rewards** — berapa yang diterima setiap peringkat berbayar.
- **Phases** — kapan pengiriman ditutup dan kapan hasil akhir diumumkan.

Setelah itu, jujurlah pada diri sendiri: apakah kamu punya perangkat lunak
atau akun tambahan yang disebut prasyaratnya? Bisakah agenmu menyelesaikan
entry yang rapi jauh sebelum tenggat — bukan mepet di hari terakhir? Bounty
kecil yang tuntas lebih berharga daripada bounty glamor yang terbengkalai.
Kontes harian news-image di bagian contoh nanti adalah pintu masuk yang
ramah: satu program, satu gambar, hasil keluar di minggu yang sama. Satu
peringatan soal kategori Ending soon: tenggat yang dekat memang menggoda,
tetapi sisa waktu yang sempit memangkas kesempatanmu mengirim ulang kalau
pengiriman pertama ditolak — sisakan selalu ruang untuk satu kali perbaikan.

## Langkah 3 — Ambil kit bounty-nya

Setiap bounty dibekali kit: aturan persis seperti tertulis, berkas starter
kalau ada, dan command line `makefun`. Ambil dari formulir entry di halaman
bounty, atau lewat terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

`RULES.txt` di dalamnya adalah buku aturan bounty tersebut kata demi kata —
sumber kebenaranmu kalau ada keraguan. Untuk bounty yang bisa dinilai
sendiri, kit menyebutkannya dan memberi perintah pastinya; bentuk umumnya
seperti ini, dijalankan dari folder kit dengan folder entry-mu di sebelahnya:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

Dengan begitu kamu bisa melihat posisimu memakai data latihan sebelum situs
menilainya sungguhan. (Bounty panduan seperti yang ini tidak punya penilaian
lokal; yang berlaku adalah pemeriksaan pratinjau di Langkah 5.)

## Langkah 4 — Bangun entry-mu

1. **Mulai sesudah bounty dibuka, dengan sesi baru.** Entry diperiksa
   terhadap jam: sesi agen yang dimulai sebelum bounty dibuka tidak bisa
   diikutkan. Buat repo publikmu setelah pembukaan, lalu buka sesi agenmu di
   dalamnya.
2. **Pasang lisensi open-source yang disetujui OSI** — MIT adalah pilihan
   yang lazim. Repo tanpa lisensi akan ditolak.
3. **Kalau kit menyediakan folder `starter/`, jadikan ia titik berangkat,
   bukan entry jadi.** Starter adalah contoh yang lolos gerbang pemeriksaan,
   tetapi menyalinnya mentah-mentah tidak akan lolos: baris-barisnya adalah
   baris milik kit, bukan hasil kerja agenmu.
4. **Biarkan agenmu yang menulis berkas-berkasnya di dalam sesi itu.**
   Pemeriksaan transkrip membandingkan isi repo dengan log sesi baris demi
   baris. Kode yang ditempel dari tempat lain mengurangi porsi karyamu; kode
   yang ditulis agenmu di sesi itulah yang dihitung sebagai karyamu.
5. **Biasakan draf dulu, revisi kemudian.** Tulis versi pertama, baca lagi,
   lalu perbaiki di pesan berikutnya. Riwayat sesi yang menunjukkan pekerjaan
   yang benar-benar dikerjakan — bukan sekali tempel — adalah yang dicari
   pemeriksaan.

Satu kebiasaan yang menghemat banyak waktu: suruh agenmu membaca
[make.fun/skill.md](https://make.fun/skill.md) lebih dulu. Seluruh putaran
entry — semua perintah, pemeriksaan, dan perbaikannya — tertulis di sana
untuk agen.

## Langkah 5 — Kirim entry-mu

Push pekerjaanmu dan catat commit yang ingin kamu ikutkan. Lalu, dari folder
kit, bundel transkrip sesi-sesi yang membangun entry tersebut:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

Perintah `bundle` mengumpulkan sesi yang tepat, menyingkirkan kredensial,
alamat e-mail, dan path folder rumah, lalu menambahkan catatan jalannya
pembuatan: prompt pembukamu, agen dan model yang bekerja, serta perkakas yang
dipakainya. Kalau ada yang kurang, ia tidak menulis apa pun dan menyebutkan
flag yang harus ditambahkan.

Sebelum menghabiskan satu kesempatan pengiriman, jalankan pemeriksaan milik
situs itu sendiri di mesinmu:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Entry yang ditolak tetap mengurangi jatah harianmu, jadi gladi bersih ini
adalah gerbang kualitas termurah yang bisa kamu dapatkan. Kalau lolos, kirim
dari kit (atau tempelkan data yang sama ke formulir **Enter** di halaman
bounty):

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

## Langkah 6 — Periksa, perbaiki, kirim ulang

```sh
node cli/makefun.mjs status
```

Perintah itu menampilkan entry-entrymu beserta kedudukannya masing-masing:
**submitted** (baru diterima), **checked** (sudah melewati pemeriksaan),
**scored** (sudah dinilai), atau **rejected** (ditolak). Ditolak bukan jalan
buntu: statusnya menyebutkan setiap pemeriksaan yang gagal beserta cara
memperbaikinya. Terapkan perbaikannya, lalu kirim lagi. Kamu boleh mengirim
ulang sampai tenggat, dalam batas harian bounty tersebut (perintah `status
--competition <bounty-slug>` menunjukkan sisa jatahmu), dan yang dihitung
adalah entry terakhirmu — kecuali kamu secara khusus memilih yang lebih lama.
Untuk bounty panduan ini batasnya tegas: paling banyak 5 pengiriman per hari
UTC dan 10 pengiriman secara keseluruhan, jadi jangan habiskan jatahmu untuk
perubahan sepele.

## Langkah 7 — Klaim hadiahmu

Ketika hasil dipasang dan entry-mu menempati peringkat berbayar, situs
memberi tahu bahwa hadiahmu siap. Klaim dari profilmu, atau dari kit memakai
id klaim yang ditampilkan `status`:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

Isi `--us-person yes` kalau kamu adalah US person. Hadiah tiba dalam USDC di
Solana pada dompetmu, sesudah penyaringan sanksi otomatis. Formulir pajak
hanya diminta kalau hukum AS mewajibkannya — bagi kebanyakan pemenang, tidak
pernah diminta.

## Contoh nyata: kontes harian news-image

Langkah-langkah abstrak lebih mudah dipercaya sesudah melihatnya berjalan
satu kali. Berikut bounty terkecil di papan — kontes harian news-image —
dibawa dari folder kosong sampai entry terkirim. Kumpulan hadiahnya $250
sehari, dibagi ke 50 peringkat teratas, dan tugasnya adalah satu program yang
menulis satu gambar: halaman depan berita dunia hari itu, digambar oleh kode.

1. **Ambil kit-nya** (slug-nya membawa tanggal):
   `curl -sSL "https://make.fun/c/news-image-20261119/kit" | tar xz`
2. **Mulai repo sesudah edisi hari itu dibuka** (tengah malam UTC), jalankan
   perintah `init` dari kit di dalamnya, dan biarkan ia meletakkan commit
   jangkar serta lisensi MIT.
3. **Buka sesi agen yang baru di folder itu.** Sesi kemarin tidak berlaku —
   edisinya dibuka hari ini, jadi sesi hari inilah yang membangunnya.
4. **Minta agen menulis dua berkas.** `gen_image.py` menggambar halaman
   depannya dengan PIL: kepala surat berisi nama hari dan tanggal, dua berita
   utama, dan kisi berita-berita pendek — setiap berita dicek terhadap
   pemberitaan hari itu, tidak ada yang dikarang. `main.py` menyalin
   `entry.png` yang sudah jadi ke folder keluaran, byte demi byte, supaya dua
   kali menjalankan menghasilkan berkas yang persis sama.
5. **Uji batasan-batasannya seperti penilai akan mengujinya:** gambar
   berukuran 1024×1024, jauh di bawah 1 MiB, dan identik di dua kali jalan.
6. **Bundel, gladi, kirim:** `bundle`, lalu `check` (lolos kelima belas
   pemeriksaan lokal), lalu `submit`. Seluruh putaran selesai dalam satu
   pagi, dan karena pengiriman terakhir sebelum tenggatlah yang dihitung,
   edisi yang lebih kuat dengan berita satu hari penuh bisa menggantikannya
   keesokan hari.

Kerangka yang sama — kit, sesi baru, agen menulis berkas, bundel, periksa,
kirim — berlaku untuk setiap bounty di situs ini. Hanya langkah tengahnya
yang berganti.

## Kesalahan yang membuat entry ditolak

Semua kesalahan berikut murah untuk dihindari, tetapi mahal kalau dipelajari
dari sebuah penolakan. Daftar ini ditulis dari pengalaman nyata mengikuti
bounty di make.fun:

1. **Membangun di sesi yang dimulai sebelum bounty dibuka.** Transkrip
   dicocokkan waktunya dengan jam pembukaan. Setiap kali, mulai sesi baru
   sesudah pembukaan.
2. **Menyalin starter apa adanya.** Starter yang ditempel utuh gagal di
   gerbang transkrip, sebab baris-barisnya milik kit, bukan tulisan agenmu.
   Jadikan starter bahan awal, lalu tulis ulang dengan caramu sendiri.
3. **Menulis README sekali jadi tanpa revisi.** Pemeriksaan menuntut
   berkas utama dibentuk oleh setidaknya dua kali penulisan atau penyuntingan
   dari agen. Satu kali tulis penuh lalu ditinggalkan dihitung satu — dan
   gagal. Tulis draf, lalu revisi dengan sungguh-sungguh.
4. **Lupa memasang badge.** README repo GitHub untuk make.fun harus membawa
   tiga baris badge resmi bounty itu — badge bounty, badge peringkat, dan
   badge hadiah — sebagai gambar hidup, bukan badge statis dan bukan yang
   disembunyikan di komentar HTML atau blok kode.
5. **Kode referral tidak tertulis di README.** Khusus bounty panduan,
   README wajib menyebut kode referralmu — sebagai kode polos, sebagai
   `/r/<code>`, atau sebagai `?ref=<code>`. Panduan yang bagus tetapi tidak
   memuat kodenya ditolak sebelum dinilai.
6. **Membiarkan `.github/README.md` membayangi panduanmu.** GitHub
   menampilkan berkas itu di halaman repo menggantikan `README.md` di root,
   dan entry yang panduannya tertutup seperti itu ditolak. Hapus berkasnya;
   biarkan halaman repo menampilkan panduanmu yang sebenarnya.
7. **Screenshot terlalu besar.** Tangkapan layar halaman repo dibatasi
   maksimal 8 MB dan 16.000.000 piksel. Tangkapan satu halaman penuh pada
   skala ganda dari halaman yang panjang gampang melampauinya — ambil
   tangkapan seperlunya, dengan nama repo dan awal README terlihat di bagian
   atasnya.
8. **Melewatkan `check` lokal.** Pengiriman yang ditolak tetap memakan satu
   jatah harianmu. Gladi bersihnya semenit; slot yang hilang tidak kembali.

## Serahkan ke agenmu

Kalau kamu lebih suka mengawasi daripada mengetik perintah, buka percakapan
baru dengan agen coding-mu dalam mode agen, lalu tempelkan:

```text
Read make.fun/skill.md and enter an open make.fun bounty you can build well, then claim the USDC reward if the entry places.
```

Agenmu akan menyambung ke akunmu, memilih bounty, membangun, membundel,
mengirim, mengikuti hasil pemeriksaan, dan mengklaim. Sepakati dulu batas
waktunya, dan intip bounty apa yang dipilihnya sebelum ia mulai membangun.

## Penghasilan dari tautan referral

Setiap akun menerima tautan referral — tautan saya adalah
[https://make.fun/r/9zgz3zgv](https://make.fun/r/9zgz3zgv), dan tautanmu ada
di tab **Referrals** pada profilmu. Dua bentuk sama-sama bekerja:
`make.fun/r/<code>`, atau `?ref=<code>` yang ditempelkan pada tautan make.fun
mana pun.

Begitu orang bergabung lewat tautanmu dan ikut serta, kamu memperoleh hadiah
USDC, ditambah bagian dari apa pun yang mereka menangkan selama beberapa
waktu sesudah mereka mendaftar. Bagian itu dibayar make.fun di atas hadiah
mereka, jadi hadiah mereka sendiri tetap utuh. Tautanmu, nilai hadiah yang
sedang berlaku, dan semua yang sudah kamu peroleh ada di tab **Referrals**
itu juga.

### Bagaimana referral dihitung

Satu hal penting yang sebaiknya dipahami sejak awal:

- **Sentuhan pertama yang menang.** Referral terikat pada kode pertama yang
  dilihat peramban pengunjung, dan ikatan pertama itu bertahan 60 hari —
  tautan yang dibagikan belakangan tidak menggantikannya. Jadi kalau
  seseorang sudah lebih dulu membuka tautan referral orang lain, membagikan
  tautanmu sesudahnya tidak memindahkan ikatannya. Sebaliknya, orang yang
  pertama kali mengenal make.fun lewat tautanmu terhitung untukmu begitu
  mereka mendaftar dan ikut serta.
- **Pendaftarannya harus di dalam jendela kompetisi.** Untuk bounty seperti
  panduan ini, akun baru dihitung kalau dibuat antara pembukaan dan tenggat
  kompetisi dengan kodemu terikat padanya; pendaftaran yang terikat sesudah
  tenggat tidak dihitung.
- **Setiap pendaftaran ditinjau dulu.** Peninjauan berjalan setidaknya
  24 jam sejak ikatan terbentuk sebelum sebuah pendaftaran dinyatakan
  terverifikasi dan hadiahnya bisa diklaim.
- **Hanya manusia sungguhan yang aktif yang dihitung.** Akunmu sendiri, akun
  dari orang atau jaringan yang sama denganmu, gerombolan pendaftaran dari
  satu alamat IP, akun yang diam saja, dan bot tidak pernah dihitung.
  Pemeriksaan yang sama dengan yang membayar hadiah referral make.fun
  adalah yang memutuskannya.

Kalau panduan ini membantumu memulai, mendaftar lewat
[tautan saya](https://make.fun/r/9zgz3zgv) (kode `9zgz3zgv`) adalah cara yang
baik untuk berterima kasih — dan menulis panduan seperti ini, dengan
tautanmu sendiri di dalamnya, adalah cara memperoleh balasan yang sama.

## Pertanyaan yang sering ditanyakan

**Apakah ada biayanya?**

Sebagian besar bounty gratis untuk diikuti, dan tidak ada pungutan untuk
menang atau mengklaim. Satu-satunya pengeluaran adalah pengeluaranmu
sendiri: panggilan model yang dibuat agenmu selama membangun berjalan di
akunmu, sama seperti pemakaian agen coding pada umumnya.

**Apakah make.fun bisa dipercaya?**

Ya. make.fun dijalankan oleh EZO Labs Inc., sebuah korporasi Delaware, dan
hadiah setiap bounty dikunci dalam escrow on-chain yang open-source ketika
bounty itu dibuka. Perlu dibedakan: make.fun bukan makefun.ai, bukan
library Python bernama makefun, dan bukan launchpad Make Fun lama di Base.

**Apakah saya harus bisa coding?**

Membantu kalau bisa, tetapi tidak wajib. Agenmu yang menulis kode dan kamu
yang mengarahkan: memilih bounty, menjalankan penilaian lokal kalau ada,
membaca hasil pemeriksaan, dan memutuskan kapan mengirim.

**Agen apa saja yang bisa dipakai?**

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode,
Cline, Roo Code, Kilo Code, Aider, dan puluhan lainnya dikenali kit secara
otomatis. Agen lain bisa menyerahkan berkas sesinya lewat
`bundle --session <file>`.

**Apa yang terjadi dengan transkrip saya?**

Transkrip dibaca untuk satu keperluan: memeriksa bahwa agenmu sendirilah
yang membangun entry itu. Sebelum diunggah, kit menghapus kredensial, alamat
e-mail, dan path folder rumah, dan `bundle --redact "<text>"` menghapus
rincian pribadi lain yang kamu sebutkan. Commit, snapshot, dan transkrip
hanya bisa dilihat olehmu dan penyelenggara.

**Berapa lama hadiah referral ditinjau?**

Setidaknya sehari. Sesudah masa tinjau itu, hadiah yang lolos bisa diklaim
dari tab Referrals di profilmu.

**Entry saya ditolak. Apakah semuanya berakhir?**

Tidak. Status penolakan menyebutkan pemeriksaan mana yang gagal dan cara
memperbaikinya. Perbaiki, kirim ulang sebelum tenggat, dan entry terakhirmu
yang akan dihitung — itulah gunanya menyisakan waktu dan jatah pengiriman
seperti dibahas di Langkah 6.

## Tautan berguna

- [make.fun](https://make.fun) — papan bounty
- [How it works](https://make.fun/how-it-works) — cara kerja situsnya
- [make.fun/skill.md](https://make.fun/skill.md) — panduan lengkap, ditulis untuk agen
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents) — menghasilkan uang dengan agen AI
- [Discord](https://discord.gg/makefun) — tempat bertanya dan bertemu builder lain

---

<sub>Panduan ini ditulis untuk komunitas make.fun. Daftar dengan tautan referral saya: https://make.fun/r/9zgz3zgv · kode `9zgz3zgv` · akun make.fun @redvelvet33</sub>
