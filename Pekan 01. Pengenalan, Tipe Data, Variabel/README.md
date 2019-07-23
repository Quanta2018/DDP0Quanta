# Pengenalan, Variabel, dan Tipe Data

**Dasar-Dasar Pemrograman 0** | Penulis: Harnindyto Wicaksana, Rafi Muhammad Daffa

*Diperbarui pada 22 Juli 2019*



## Daftar Isi

[1A. Instalasi Python](https://github.com/Quanta2018/DDP0Quanta/tree/master/Pekan%2001.%20Pengenalan%2C%20Tipe%20Data%2C%20Variabel#1a-instalasi-python)

[1B. Mengenal IDLE dan Shell](https://github.com/Quanta2018/DDP0Quanta/tree/master/Pekan%2001.%20Pengenalan%2C%20Tipe%20Data%2C%20Variabel#1b-mengenal-idle-dan-shell)

[1C. Tipe Data](https://github.com/Quanta2018/DDP0Quanta/tree/master/Pekan%2001.%20Pengenalan%2C%20Tipe%20Data%2C%20Variabel#1c-tipe-data)

[1D. Variabel](https://github.com/Quanta2018/DDP0Quanta/tree/master/Pekan%2001.%20Pengenalan%2C%20Tipe%20Data%2C%20Variabel#1d-variabel)

[1L. Latihan](https://github.com/Quanta2018/DDP0Quanta/tree/master/Pekan%2001.%20Pengenalan%2C%20Tipe%20Data%2C%20Variabel/Latihan)



## 1A. Instalasi Python

Pada dasarnya, pemrograman dengan menggunakan Python membutuhkan setidaknya 2 komponen utama:

1. Kode sumber (*source code*) Python beserta *shell* dan *interpreter* yang berfungsi sebagai "tulang belakang" dari Python itu sendiri.
2. *Integrated Development Environment* (IDE) yang berfungsi sebagai tempat program yang dibuat dengan Python dibuat dan dikembangkan.

Instalasi dasar Python yang dapat diunduh dari situs resminya sudah terpaketkan dengan kode sumber Python, *shell*, *interpreter*, beserta IDE yang diberi nama "*Integrated Development and Learning Environment*" (IDLE) yang dirancangkan sebagai IDE yang ramah terhadap pembelajaran.

Perlu diketahui bahwa saat ini terdapat dua cabang utama versi Python yakni:

1. **Python 2.x** yang merupakan versi *legacy* dari Python dan saat ini dikelola sebagai perpanjangan masa guna program yang dirancang sebelum Python 3.x dirilis akibat adanya perbedaan mendasar antara Python 2.x dan 3.x.
2. **Python 3.x** yang merupakan versi terkini dari Python dan versi yang direkomendasikan untuk program yang dirancang saat ini. Akibat adanya perbedaan mendasar di antara kedua versi, Python 3.x kemungkinan besar tidak dapat menjalankan program Python 2.x dan sebaliknya dengan baik.

Untuk keperluan standar, versi Python di atas 3.5 sudah memenuhi syarat dalam mengikuti pembelajaran pemrograman yang ada saat ini (termasuk perkuliahan di Fasilkom UI). Namun, sebagai tindak pencegahan, usahakan untuk menggunakan versi Python terbaru (melihat lingkungan pemrograman yang ditempati).

### Instalasi Python untuk Windows

1. Cek terlebih dahulu *bit* dari *processor* dan sistem operasi yang digunakan (32-bit atau 64-bit).

   Langkah ini akan menentukan tipe instalasi Python yang akan digunakan nantinya. Salah satu cara mudah untuk mengecek hal ini adalah menggunakan Dxdiag:

   1. Tekan tombol <code>Win</code> dan <code>R</code> secara bersamaan untuk memunculkan *Run Dialog*.
   2. Ketik <code>dxdiag</code> pada kolom Open dan tekan <code>Enter</code>.
   3. Pilih <code>Yes</code> pada pertanyaan yang muncul (bila ada).
   4. Bit yang digunakan dapat dilihat pada kolom Sistem Operasi.

2. Pada [laman pengunduhan Python ini](https://www.python.org/downloads/release/python-374/), pilih tulisan yang sesuai berikut ini pada bagian Files:

   1. Windows x86 executable installer untuk 32-bit
   2. Windows x86-64 executable installer untuk 64-bit

3. Jalankan instalasi Python yang sudah diunduh sebelumnya.

4. Centang opsi "Add Python 3.7 to PATH" agar Python nantinya dapat dijalankan dengan mudah melalui Command Prompt/PowerShell dan dapat digunakan bersama IDE lain yang akan datang.

5. Pilih "Install Now" untuk memulai instalasi untuk satu pengguna (pilih Customize Installation untuk instalasi *system-wide* - opsional).

6. Saat instalasi selesai, pilihlah untuk "Disable Path Length Limit" sebagai tindak pencegahan.

   Langkah ini akan membantu Python dalam menggunakan direktori yang lebih panjang dari batasan yang dimiliki oleh Windows.

7. Pastikan bahwa IDLE (Python 3.7 xx-bit) sudah muncul di daftar program dan kata kunci <code>python</code> dapat memanggil versi Python yang dipasang sebelumnya melalui Command Prompt atau PowerShell.

### Instalasi Python untuk macOS

> **Catatan**:
>
> Beberapa program yang dirancang untuk macOS bergantung pada versi Python 2.x sehingga macOS membawa versi Python 2.x secara *default*. Akibatnya, kata kunci <code>python</code> pada Bash atau terminal lainnya akan memanggil Python 2.x tersebut. Untuk memanggil Python 3.x, kata kunci <code>python3</code> dapat digunakan.

1. Pada [laman pengunduhan Python ini](https://www.python.org/downloads/release/python-374/), pilih tulisan "macOS 64-bit/32-bit installer" pada bagian Files.
2. Jalankan instalasi Python yang sudah diunduh sebelumnya. 
3. Tekan tombol "Continue" atau "Lanjutkan" pada laman Introduction, Read Me, License, dan Destination Select (tekan "Agree" bila ada).
4. Tekan tombol "Install" untuk melakukan instalasi standar (masukkan password pengguna macOS apabila diminta). Tanda centang dengan latar hijau menandakan selesainya instalasi Python.
5. Untuk alasan keamanan, tekan tombol "Install Certificates" bila diminta.
6. Pastikan IDLE dan Python Launcher sudah muncul pada Launchpad (tekan F4 untuk mengakses Launchpad) dan kata kunci <code>python3</code> dapat memanggil Python 3.x pada Bash atau terminal lainnya.

### Instalasi Python untuk Linux

Bahasa pemrograman dasar yang digunakan oleh Linux adalah Python dan umumnya distribusi Linux sudah membawa versi Python 3.x secara *default*. Hal ini dapat dicek dengan kata kunci <code>python</code> pada Bash atau terminal lainnya. Apabila versi yang ditunjukkan bukan 3.x, silakan gunakan *package manager* bawaan distribusi masing-masing untuk memasang <code>python3</code>. Apabila IDLE belum terpasang, gunakan langkah yang sama untuk memasang <code>idle3</code>.



## 1B. Mengenal IDLE dan Shell

Ketika IDLE dijalankan atau ketika Python dijalankan melalui CMD/PowerShell/Terminal, kamu akan disambut dengan Python 3.x Shell. Shell ini berfungsi sebagai antarmuka antara pengguna dengan program. Di sini, kamu dapat menulis satu blok program yang akan dijalankan langsung oleh Python. Hal ini dapat digunakan untuk mempelajari cara kerja Python dan mencoba-coba beberapa ekspresi dalam Python.

> **Your first program!**
>
> Pernah mendengar kata-kata "Hello World" sebelumnya? Yuk, coba untuk mencetak kalimat tersebut sebagai program pertama kamu di Python dengan mengetikkan ekspresi berikut di Shell (di samping tanda ">>>"):
>
> ~~~python
> print("Hello World!")
> ~~~
>
> Python akan "mencetak" kalimat Hello World! tanpa tanda kutip setelah kamu menekan <code>Enter</code>.

Saat menggunakan Shell, kamu hanya dapat menjalankan ekspresi program satu per satu. Sehingga, kamu akan kesulitan untuk membuat suatu program dengan rangkaian ekspresi yang panjang di Shell. (Cara untuk merangkai ekspresi panjang menjadi sebuah program akan dipelajari di Pekan 02). Namun, dampak dari ekspresi yang kamu jalankan sebelumnya masih dapat kamu rasakan sampai kamu menutup Shell.

Cobalah untuk melakukan ekspresi berikut untuk memberikan nilai terhadap suatu variabel:

~~~python
euler_number = 2.718
~~~

Kemudian, panggil variabel tersebut:

~~~python
euler_number
~~~

Python akan menunjukkan bahwa nilai <code>euler_number</code> adalah 2.718.



## 1C. Tipe Data

> **Tipe data** mendefinisikan suatu kelompok nilai dan operasi-operasi yang dapat dilakukan oleh tipe data tersebut.

Secara sederhana, tipe data merupakan "perjanjian" antara suatu nilai dengan program tentang perilaku dari nilai tersebut dan bagaimana nilai tersebut dapat digunakan dan dimodifikasi oleh program. Misalnya, tipe data Integer yang menyimpan nilai berupa bilangan bulat memungkinkan nilai bilangan bulat tersebut untuk dioperasikan secara matematis (penambahan, pengurangan, dan lain-lain).

Dalam Python, tipe data ditafsirkan secara dinamis oleh program. Setiap tipe data memiliki kelompok nilai yang sesuai dan apabila kelompok nilai tersebut digunakan, maka Python akan menyimpulkan sendiri tipe data yang digunakan.

| Tipe Data      | Inisial | Contoh               | Penggunaan umum                        |
| -------------- | ------- | -------------------- | -------------------------------------- |
| String         | str     | "HAHA"               | Rangkaian karakter yang membentuk teks |
| Integer        | int     | 123                  | Bilangan bulat                         |
| Floating Point | float   | 3.14                 | Bilangan bulat dan/atau non-bulat      |
| Boolean        | bool    | True                 | Nilai kebenaran                        |
| List           | list    | [1,2,3]              | Wadah kelompok data yang dinamis       |
| Tuple          | tuple   | (1,2,3)              | Wadah kelompok data yang statis        |
| Dictionary     | dict    | {"A":"ei", "B":"bi"} | Mirip kamus                            |
| Set            | set     | {1,2,3,4}            | Mirip dengan himpunan dalam matematika |

### String (<code>str</code>)

> Contoh:
>
> ~~~python
> "Ini string"
> "123"
> "True"
> "Hello World!"
> "Pr0gr4mm1Ng 1tU g4mP4ng!"
> "^ bohong"
> 
> 'i\'m just testing some stuff'
> 
> """first line,
> second line,
> third line"""
> 
> 'is this the same as above?\nmaybe'
> 
> '''
> can i do this?\nwhy so random?
> dunno
> '''
> ~~~

#### Penjelasan Umum

Tipe data String merepresentasikan data berupa teks yang merupakan untaian (*strings*) karakter-karakter. Untuk menandakan bahwa nilai yang diberikan adalah sebuah String, nilai tersebut harus diapit oleh salah satu dari tiga pengapit berikut ini:

1. Tanda petik tunggal (*apostrophe*): <code>'Hello World!'</code>.
2. Tanda petik ganda (*double quote*): <code>"Hello World!"</code>.
3. Tiga buah tanda petik tunggal/ganda: <code>'''Hello World!'''</code> atau <code>"""Hello World!"""</code>.

Pengapit tiga buah tanda petik tunggal/ganda dapat digunakan untuk menyusun teks yang memiliki lebih dari satu baris, contoh:

~~~python
"""
Mereka bilang aku pawang ular piton,
padahal aku barista kopi jawa.
"""
~~~

#### *Indexing*

Karena String merupakan untaian karakter-karakter, setiap karakter (terlepas dari apa jenis karakternya) memiliki nomor indeks yang bisa dipanggil. Nomor indeks pada String dimulai dari 0 untuk karakter paling kiri dari String tersebut.

Contoh:

~~~python
"Harnin Todi"
~~~

| H    | a    | r    | n    | i    | n    |      | T    | o    | d    | i    |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 0    | 1    | 2    | 3    | 4    | 5    | 6    | 7    | 8    | 9    | 10   |

Untuk memanggil suatu karakter dalam untaian teks, kamu dapat memanggil variabel yang menyimpan teks tersebut dan menambahkan [nomor index].

Contoh:

~~~python
my_name = "Harnin Todi"
print(my_name[1])
~~~

Hasil:

~~~python
a
~~~

Nomor indeks juga dapat bernilai negatif. Nomor indeks negatif merupakan kebalikan dari nomor indeks non-negatif di mana nomor indeks negatif -1 dimulai dari karakter paling kanan dan seterusnya ke arah kiri.

Contoh:

~~~python
"Rafi M Daffa"
~~~

| R    | a    | f    | i    |      | M    |      | D    | a    | f    | f    | a    |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| -12  | -11  | -10  | -9   | -8   | -7   | -6   | -5   | -4   | -3   | -2   | -1   |

Kedua nomor indeks ini dapat digunakan secara bersama-sama dan nomor indeks pada posisi yang sama akan mengembalikan karakter yang sama, misalnya:

~~~python
my_faculty = "Fasilkom"
print(my_faculty[1])
print(my_faculty[-7])
~~~

Hasil:

~~~python
a
a
~~~

#### *Slicing*

Misalnya kita ingin mengambil sebagian dari String tertentu untuk membentuk suatu String baru. Kita dapat menggunakan metode *slicing* yang diturunkan dari *indexing* pada materi sebelumnya di mana pemanggilan nomor indeks dapat dibongkar menjadi format berikut:

~~~python
text_var[x:y:z]
~~~

> x: Indeks mulai untuk pemotongan (inklusif - default 0)
>
> y: Indeks akhir untuk pemotongan (eksklusif - default -1)
>
> z: *Stepping* (Jarak longkapan dalam pemotongan - default 1 / tidak ada pelongkapan)

Ketiga nilai tersebut tidak perlu untuk dicantumkan semua. Selama pemisahnya (<code>:</code>) tercantum, maka Python akan menggunakan nilai-nilai *default* yang ada di atas. Bahkan, pemisah antara y dan z seringkali tidak diperlukan apabila tidak ada longkapan. Contohnya:

~~~python
me = "Noni, do you wanna be my gf?"
noni1 = me[25:] 
noni2 = me[:2]
print(noni1)
print(noni2)
~~~

Hasil:

~~~
gf?
No
~~~

Manipulasi pemotongan secara kreatif dapat menghasilkan hal-hal yang memudahkan dalam pengolahan teks. Amatilah hasil dari blok program ini di Python-mu!

~~~
brain = "borrow or rob"
print(brain[::-1])
~~~

#### Operasi String

Dalam Python, String mendukung tanda operasi <code>+</code> yang digunakan untuk melakukan penggabungan dua buah String dan <code>*</code> yang digunakan untuk melakukan duplikasi (menggandakan sebuah teks)

Contoh:

~~~python
first_name = "mind your own "
last_name = "business"
full_name = first_name + last_name
on_my_mind = last_name * 3
print(full_name)
print(on_my_mind)
~~~

Hasil:

~~~python
mind your own business
businessbusinessbusiness
~~~

Selain itu, String juga memiliki beberapa metode (perlakuan yang dapat diberikan terhadap suatu String) sebagai berikut:

`len(var)` -> mengembalikan panjang String

`var.find()` -> mengembalikan indeks dari nilai yang dicari

`var.isdigit()` -> mengembalikan True jika semuanya adalah angka

`var.upper()` -> mengembalikan String yang semuanya kapital

`var.lower()` -> mengembalikan String yang semuanya bukan kapital

`var.isupper()` -> mengembalikan True jika semuanya kapital

`var.islower()` -> mengembalikan True jika semuanya bukan kapital

> **Catatan**:
>
> Mengembalikan tidak selalu berarti data asli yang diberi perlakuan berubah. Dalam hal ini, pengembalian berarti akan dibuat suatu data baru yang merupakan hasil dari perlakuan tersebut.

Contoh:

~~~python
me = "ME SO ANGRY"
print(len(me))
print(me.find("S"))
print(me.lower())
~~~

Hasil:

~~~python
11
3
me so angry
~~~



### Integer (<code>int</code>)

> Contoh:
>
> ~~~python
> 10
> 78
> 1928
> 9223372036854775807
> ~~~

#### Penjelasan Umum

Pada dasarnya, Integer (bilangan bulat) merupakan tipe data yang berkaitan dengan, ya, bilangan bulat. Python akan secara otomatis menganggap data-data bilangan bulat yang tidak diapit oleh pembatas lain sebagai sebuah Integer. Perlu diketahui bahwa Python tidak memiliki batasan konkret terhadap data Integer yang digunakan, namun akan ada hal lain yang berkaitan dengan tipe data Integer dan memiliki batas praktis, seperti nomor indeks.

#### Operasi Matematika

> **Catatan**:
>
> Semua operasi matematika di bawah ini akan mengembalikan sebuah angka baru yang merupakan hasil dari operasinya. *Operand* (angka yang dilakukan operasi) tidak mengalami perubahan.

Tipe data Integer digunakan untuk mengoperasikan data-data dengan operasi matematis, di antaranya:

| Operasi                                  | Contoh    | Catatan                         | Presedensi    |
| ---------------------------------------- | --------- | ------------------------------- | ------------- |
| Penjumlahan (<code>+</code>)             | 1024+2048 | -                               | 3 (terendah)  |
| Pengurangan (<code>-</code>)             | 766-9128  | -                               | 3 (terendah)  |
| Perkalian (<code>*</code>)               | 827*5     | -                               | 2             |
| Pembagian (<code>/</code>)               | 30/5      | Menghasilkan <code>float</code> | 2             |
| Pembagian Lantai (<code>//</code>)       | 3//2      | Pembulatan ke bawah             | 2             |
| Sisa Pembagian / Modulo (<code>%</code>) | 3%2       | -                               | 2             |
| Pemangkatan (<code>**</code>)            | 2**3      | -                               | 1 (tertinggi) |

Perlu dicatat bahwa presedensi dan sifat asosiatif dan komutatif dari operasi matematika tetap berlaku di Python dan Python akan secara otomatis menghitung operasi sesuai dengan peraturan tersebut. Selain itu, penggunaan tanda kurung <code>()</code> juga akan meningkatkan presedensi dari operasi yang ada di dalamnya menjadi tertinggi seperti pada operasi matematika.

Contoh:

~~~python
print(1+2*3**4)
~~~

Hasil:

~~~python
163
~~~

#### Operasi Matematika + Pemberian Nilai

Operasi dengan tipe ini umumnya digunakan bersama dengan variabel. Sebelumnya telah disinggung bahwa seluruh operasi matematika tidak akan mengubah *operand*, namun akan menghasilkan sebuah angka baru yang merupakan hasil dari operasi yang digunakan. Maka, jika kita ingin mengubah suatu nilai dalam variabel, kita harus melakukan seperti ini:

~~~python
my_var = 5
my_var = my_var * 2
~~~

Pada operasi matematika yang ada di baris kedua program, ada dua hal yang terjadi:

1. Operasi perkalian akan dievaluasi dengan mengambil nilai dari <code>my_var</code> dan mengalikannya dengan 2 sehingga menghasilkan suatu angka baru 10.
2. Angka baru 10 tersebut diberikan sebagai nilai baru dari <code>my_var</code>. (Sistem pemberian nilai variabel akan dijelaskan pada subbab berikutnya).

Operasi seperti ini dapat dipersingkat dengan menggunakan operasi matematika yang disatukan dengan pemberian nilai sebagai berikut:

> Asumsikan ada sebuah variabel var1 dengan nilai 10

| Operasi                        | Contoh     | Ekuivalen dengan | Nilai <code>var1</code> setelah operasi |
| ------------------------------ | ---------- | ---------------- | --------------------------------------- |
| Penjumlahan (`+=`)             | var1 += 10 | var1 = var1 + 10 | 20                                      |
| Pengurangan (`-=`)             | var1 -= 10 | var1 = var1 - 10 | 0                                       |
| Perkalian (`*=`)               | var1 *= 5  | var1 = var1 * 5  | 50                                      |
| Pembagian (`/=`)               | var1 /= 4  | var1 = var1 / 4  | 2.5                                     |
| Pembagian Lantai (`//=`)       | var1 //= 4 | var1 = var1 // 4 | 2                                       |
| Sisa Pembagian / Modulo (`%=`) | var1 %= 3  | var1 = var1 % 3  | 1                                       |
| Pemangkatan (`**=`)            | var1 **= 2 | var1 = var1 ** 2 | 100                                     |

Cobalah untuk melakukan operasi di bawah ini:

~~~python
13 // 5 * 5 + 13 % 5
-13 %  3
-17 // 7
-13 % -3
'D' * 2 + 'P' + '0'
~~~

#### Fungsi Integer

> **"Fun Fact"**:
>
> Meskipun <code>abs(x)</code> hanya dapat digunakan untuk Integer, <code>min(a,b,...,z)</code> dan <code>max(a,b,...,z)</code> dapat digunakan untuk tipe data apapun yang bisa diurutkan (*orderable*), termasuk String, Boolean, List, dan lain-lain.
>
> **Further Learning**:
>
> Relasi terurut yang membahas tentang keterurutan (apakah suatu himpunan data dapat diurutkan) akan dipelajari pada mata kuliah Matematika Diskret 2 (CSGE601011)

Untuk memanipulasi sebuah angka bertipe Integer, ada beberapa fungsi yang dapat digunakan, di antaranya:

1. <code>abs(x)</code>: Menerima suatu angka x dan mengembalikan nilai mutlak (absolut) dari angka tersebut.
2. <code>min(a,b,....,z)</code>: Menerima himpunan angka yang dipisahkan dengan koma dan menghasilkan angka terkecil dari himpunan tersebut.
3. <code>max(a,b,....,z)</code>: Menerima himpunan angka yang dipisahkan dengan koma dan menghasilkan angka terbesar dari himpunan tersebut.

### Float (<code>float</code>)

> Contoh:
>
> ~~~python
> 3.14
> 2.718
> 1.0
> 2.
> ~~~

#### Penjelasan Umum

Tipe data Float (singkatan dari *floating point*) merupakan tipe data yang mengolah data berupa bilangan (bisa bulat atau tidak) dan dapat menyimpan angka di belakang koma. Float dibedakan dari Integer karena representasi kedua tipe tersebut sangat berlainan di tingkat mesin akibat perlu adanya penanda khusus untuk menyatakan bilangan di belakang koma untuk Float.

Implementasi bilangan Float mengacu pada standar IEEE 754 dan idealnya memiliki dua tingkatan akurasi:

1. *Single-Precision*: Menyediakan ruang data sebesar 32-bit dengan angka maksimal kurang lebih 3.40282346638528860e+38.
2. *Double-Precision*: Menyediakan ruang data sebesar 64-bit dengan angka maksimal kurang lebih 1.7976931348623157e+308.

Pada Python, semua bilangan Float secara otomatis menggunakan *double-precision*, apapun angkanya. Hal ini belum tentu benar untuk bahasa pemrograman lainnya.

> **Further Learning**:
>
> Sistem representasi bilangan pada komputer akan disinggung pada mata kuliah Dasar-Dasar Pemrograman 1 (CSGE601020) dan akan dibahas lebih dalam pada mata kuliah Pengantar Sistem Digital (CSCM601150) untuk program studi Ilmu Komputer.

#### Relasi antara Integer dan Float

Mayoritas operasi yang berlaku pada Integer juga berlaku pada Float. Salah satu perbedaannya terletak pada Pembagian Lantai (<code>//</code>). Pada Integer, operasi ini akan menghasilkan pembagian yang dibulatkan ke bawah dalam bentuk Integer. Pada Float, pembulatan ke bawah tetap terjadi namun hasil yang diberikan tetap merupakan Float.

Contoh:

~~~python
print(11.0 // 5)
~~~

Hasil:

~~~python
2.0
~~~

Integer dan Float dapat dioperasikan secara bersamaan dalam satu operasi matematis. Jika salah satu dari *operand* adalah Float, maka hasil yang diberikan merupakan Float karena Float memiliki presisi lebih tinggi dibanding Integer. Contoh di atas menunjukkan pembagian lantai antara Float dengan Integer yang menghasilkan data berupa Float.

Pada Python, Integer dan Float juga dapat dibandingkan satu sama lain. Sehingga, data Integer 5 dan data Float 5.0 akan dianggap sama oleh Python. Hal ini belum tentu berlaku pada bahasa pemrograman lainnya.



### Boolean (<code>bool</code>)

> Hanya ada dua nilai dalam tipe data Boolean:
>
> ~~~python
> True
> False
> ~~~

#### Penjelasan Umum

Tipe data Boolean merupakan tipe data yang merepresentasikan suatu nilai kebenaran atau kesalahan. Dalam tipe data Boolean, hanya ada dua nilai yang sah, yaitu <code>True</code> dan <code>False</code> (perhatikan kapitalisasinya). Implementasi dari masing-masing nilai tersebut bisa berbeda antara satu bahasa dengan yang lainnya, namun True sudah pasti merepresentasikan benar dan False sudah pasti merepresentasikan salah.

#### Operasi Pembanding

Kasus di mana tipe data Boolean umumnya digunakan adalah sebagai hasil dalam operasi pembanding. Operasi pembanding dapat dilakukan terhadap data dengan berbagai macam tipe di mana hasilnya akan mengembalikan salah satu dari dua nilai Boolean di mana True berarti perbandingan yang dilakukan merupakan perbandingan yang valid dan False berarti perbandingan yang dilakukan merupakan perbandingan yang keliru.

| Operasi                             | Contoh | Hasil |
| ----------------------------------- | ------ | ----- |
| Kurang dari (`<`)                   | 1 < 2  | True  |
| Kurang dari atau sama dengan (`<=`) | 2 <= 2 | True  |
| Sama dengan (`==`)                  | 3 == 4 | False |
| Tidak sama dengan (`!=`)            | 4 != 9 | True  |
| Lebih dari atau sama dengan (`>=`)  | 3 >= 5 | False |
| Lebih dari (`>`)                    | 4 > 4  | False |

Umumnya, operasi pembanding hanya dapat digunakan untuk dua data yang memiliki tipe sama. Namun, ada beberapa tipe data yang dapat dibandingkan dengan tipe data lain, seperti Integer dan Float.

Contoh:

~~~python
# Dapat dilakukan
1 < 2
2 > 3.0
"A" > "B"

# Tidak dapat dilakukan (akan error)
"A" >= 1
~~~

##### Perbandingan String

Setiap karakter yang tersedia memiliki representasi angka yang bertindak sebagai penerjemah antara bahasa mesin (yang sederhananya hanya terdiri dari 0 dan 1) dengan bahasa manusia. Representasi ini mulanya diatur pada standar ASCII dan dikembangkan dengan standar Unicode dengan menambah karakter-karakter lain dari berbagai macam bahasa.

> **Catatan**:
>
> **Setiap** karakter memiliki representasi angkanya masing-masing. Karakter "A" dan "a", misalnya, memiliki representasi angka yang berbeda (65 dan 97).

Untuk mengetahui tabel dari representasi tersebut, [situs ini](https://www.utf8-chartable.de/unicode-utf8-table.pl?number=1024&utf8=dec) akan membantumu.

Pada Python, perbandingan String dilakukan dengan mencari perbedaan pertama dari kiri kemudian membandingkan karakter pada indeks yang berbeda tersebut melalui representasi angka Unicode-nya. Tidak ditemukannya perbedaan berarti kedua String yang dibandingkan tersebut adalah sama.

Contoh:

~~~python
print("Wow" > "Wau")
~~~

Hasil:

~~~python
True
~~~

Penjelasan:

Pada indeks ke-0 dari kedua String ditemukan karakter yang identik, "W", sehingga tidak dapat dijadikan perbandingan. Pada indeks ke-1 ditemukan perbedaan karakter, "o" dan "a". Karakter "o" direpresentasikan dengan angka 111 dan karakter "a" direpresentasikan dengan angka 97. Karena 111 > 97, maka operasi pembanding akan mengembalikan True.

Cobalah untuk melakukan operasi di bawah ini:

~~~python
3 == 3.0
1 == True
0 == False
3 < 5
'string' == 'String'
~~~

#### Aljabar Boolean

Layaknya perlakuan operasi matematis pada Integer dan Float, Boolean juga memiliki operasi yang mengambil *operand* dan memberikan hasil berupa nilai Boolean. Operasi-operasi Boolean inilah yang mendasari konsep komputasi dan digunakan mulai tingkat mesin (untuk mengolah 0 dan 1) hingga tingkat interpretasi bahasa manusia (penggunaan pada bahasa pemrograman seperti Python).

Sebelum memasuki operasi Boolean, perlu diketahui bahwa ada tiga macam operator umum:

1. Operator uner: Operator yang menerima satu *operand* (contoh: - untuk menandakan angka negatif)
2. Operator biner: Operator yang menerima dua *operand* (contoh: penjumlahan, pengurangan)
3. Operator terner: Operator yang menerima tiga *operand* (contoh: <code>a if True else b</code>)

Operasi logika (Boolean) sebenarnya terdiri dari beberapa jenis, di antaranya adalah AND, OR, NOT, XOR, XNOR, NAND, dan NOR. Modul ini hanya akan membahas penggunaan AND, OR, dan NOT pada Python untuk melakukan operasi Boolean.

| Nama Operasi | Singkatan | Tipe Operator | Penggunaan | Contoh                     |
| ------------ | --------- | ------------- | ---------- | -------------------------- |
| Konjungsi    | AND       | Biner         | a and b    | <code>True and True</code> |
| Disjungsi    | OR        | Biner         | a or b     | <code>True or False</code> |
| Negasi       | NOT       | Uner          | not a      | <code>not True</code>      |

Untuk memudahkan pemahaman terhadap konsep ini, amati tabel kebenaran di bawah ini:

| A     | B     | not A | A and B | A or B |
| ----- | ----- | ----- | ------- | ------ |
| True  | True  | False | True    | True   |
| True  | False | False | False   | True   |
| False | True  | True  | False   | True   |
| False | False | True  | False   | False  |

Layaknya operasi matematika, operasi logika juga dapat dirangkai dan memiliki presedensi terhadap sesama operasi logika maupun dengan operasi pembanding dan/atau operasi matematika.

> **Presedensi operasi logika**:
>
> 1. NOT
>
> 2. AND
> 3. OR
>
> **Presedensi antar-operasi**:
>
> 1. Operasi matematika
> 2. Operasi pembanding
> 3. Operasi logika

Contoh:

~~~python
not 1%2==1 and 1%3!=1 or 1%4==1
~~~

Penjelasan:

1. 1%2, 1%3, dan 1%4 dievaluasi terlebih dahulu sebagai operasi matematika (semua hasilnya adalah 1).
2. Kemudian, setiap operasi pembanding dievaluasi yang menghasilkan, secara berurutan, True, False, dan True.
3. Kemudian, operasi NOT dievaluasi sehingga hasil True pada 1%2==1 menjadi False.
4. Kemudian, operasi AND dievaluasi dengan *operand* hasil False pada not 1%2==1 dan hasil False pada 1%3!=1 yang menghasilkan False.
5. Terakhir, operasi OR dievaluasi dengan *operand* hasil False pada operasi AND dan hasil True pada 1%4==1 yang menghasilkan True.

Hasil:

~~~python
True
~~~

### List (<code>list</code>)

> Contoh:
>
> ~~~python
> ["Lonely"]
> ["Red", "Green", "Blue"]
> [1,2,3]
> [True, True, False]
> [["I","Love","You"], 3000, False]
> [[[[[[[[[[1,2]]]]]]]]]]
> ~~~

#### Penjelasan Umum

Sesuai namanya, tipe data List merupakan tipe data yang dapat mengelompokkan berbagai tipe data (termasuk List lain) dalam satu wadah. Python akan menerjemahkan suatu nilai sebagai List jika data apapun yang ingin kita simpan di List diapit dengan tanda kurung siku (<code>[]</code>) dan setiap data dipisahkan dengan tanda koma. Pada Python, suatu List dapat berisi berbagai macam tipe data sekaligus.

Suatu List bersifat *mutable*, artinya ukuran dan isi dari List tersebut dapat dimanipulasi secara langsung. Kita dapat menambahkan data baru ke dalam List yang sudah kita buat dan kita dapat mengubah konten yang sudah ada di dalam List tersebut, bahkan membuangnya sama sekali.

#### *Indexing*

Sama seperti String, setiap data yang berada di dalam List memiliki nomor indeksnya masing-masing dan dapat dipanggil dengan menambahkan [nomor indeks] pada pemanggilan variabel List.

Contoh:

~~~python
grocery_list = ["Cabbage", "Spices", "Corn"]
print(grocery_list[1])
~~~

Hasil:

~~~python
Spices
~~~

Pemanggilan melalui *indexing* ini juga dapat digunakan untuk memanipulasi data yang terletak pada indeks tersebut.

Contoh:

~~~python
favourite_course = ["DDP1", "Matdis 1", "MPKT B"]
favourite_course[1] = "PSD"
print(favourite_course[1])
~~~

Hasil:

~~~python
PSD
~~~

Jika data yang terletak pada nomor indeks dalam suatu List merupakan koleksi dari data-data yang memiliki nomor indeks tersendiri, *nested indexing* dapat dilakukan.

Contoh:

~~~python
interests = ["UI/UX", "Data Science", "Software Engineering"]
print(interests[0][2])
~~~

Hasil:

~~~python
/
~~~

### Tuple (<code>tuple</code>)

> Contoh:
>
> ~~~python
> ("Lonely",)
> (1,2,3)
> ("A", 10, True)
> ~~~

Mirip seperti List, tipe data Tuple ditujukan sebagai wadah untuk menampung berbagai macam tipe data (bahkan Tuple lain). Yang membedakan antara List dengan Tuple di antaranya adalah sebagai berikut:

1. Konstruksi Tuple yang berisi hanya satu data harus diikuti dengan tanda koma untuk mencegah ambiguitas dengan pengurungan untuk menaikkan presedensi.
2. Tuple bersifat *immutable*, artinya konten Tuple yang sudah dibentuk tidak dapat diganti dengan data lain. Modifikasi terhadap Tuple harus melalui pembuatan Tuple baru yang memuat perubahan yang diinginkan.
3. Penomoran indeks masih berlaku layaknya List, namun penggantian konten dari data pada indeks tersebut tidak dapat dilakukan (modifikasi tertentu dapat dilakukan jika data tersebut bersifat *mutable*).

Contoh:

~~~python
# Valid
list_in_tuple = ([1,2],[3,4])
list_in_tuple[0][1] = 3

# Invalid
my_tuple = (1,2,3)
my_tuple[0] = 2
~~~

### Tipe Data Lainnya

Masih banyak tipe data lain yang dimiliki oleh Python, seperti Dictionary dan Set. Bahkan, Python yang pada prinsipnya merupakan bahasa pemrograman berorientasi objek (OOP) dapat mengakomodasi pembuatan "tipe data" baru melalui penggunaan <code>class</code> (referensi lebih lanjut: OOP). Tipe data yang telah dibahas di atas telah mencakup tipe-tipe dasar yang lazim digunakan dan menjadi pondasi dalam mengembangkan tipe-tipe data lainnya.

### *Type Casting*

> **Perhatian**
>
> Gunakan fitur ini dengan bijak. Tidak semua tipe data dapat di-"cast" ke semua tipe data lainnya. Kegagalan proses ini dapat menimbulkan *error* dan berhentinya program secara utuh.

*Type casting* adalah sebuah teknik untuk membuat suatu data yang memiliki suatu tipe data diperlakukan seperti tipe data lain yang diinginkan. Dalam hal ini, kita melakukan *overidding* terhadap inferensi tipe data yang dilakukan oleh Python terhadap data yang dibuat. Suatu data dapat di-*cast* ke tipe data lain dengan memanggil inisial dari tipe data tujuannya (dibahas pada subbab 1C) sebagai berikut:

~~~python
# <tipe data tujuan>(data asal)
# Contoh valid:
int('12')
str(12)
bool(1)

# Contoh invalid:
int("Z")
~~~



## 1D. Variabel

Seperti di matematika, variabel adalah sebuah "referensi" atau "*placeholder*" terhadap suatu nilai dalam program. Variabel dalam Python diimplementasikan sebagai suatu blok memori yang dialokasikan untuk menyimpan suatu referensi dari sebuah blok memori lain yang menyimpan data yang kita inginkan.

Analoginya, variabel dalam Python dapat diibaratkan sebagai penunjuk arah di mana ketika kita ingin menggunakan suatu nilai dalam blok memori, kita meminta variabel untuk mengarahkan kita menuju tempat nilai tersebut disimpan. Pada bahasa pemrograman lain, beberapa tipe data langsung menyimpan nilainya pada blok memori yang dialokasikan untuk variabel tersebut. Untuk memudahkan, semua tipe data di Python menggunakan referensi sebagai prinsip dalam variabel.

Untuk membentuk suatu variabel, cukup gunakan ekspresi berikut ini:

~~~python
nama_variabel = "Sebuah data String"
nama_variabel = 129120192
~~~

Pada bahasa pemrograman Python, variabel tidak memiliki tipe data secara spesifik sehingga setiap variabel di Python dapat digunakan untuk semua tipe data terlepas dari tipe data yang direferensikan oleh variabel tersebut pertama kali. Hal ini berbeda dengan bahasa pemrograman seperti Java di mana suatu variabel yang dibuat harus memiliki suatu deklarasi tipe data dan tipe data tersebut berlaku permanen.

### Kebijakan Pembuatan Variabel

> Kebijakan ini dan beberapa kebijakan penulisan lainnya merupakan bagian dari standar yang ditetapkan oleh pengembang Python yang dinamakan PEP 8 yang dapat diakses pada [tautan ini](https://www.python.org/dev/peps/pep-0008/).

Di bawah ini merupakan beberapa kebijakan pembuatan variabel yang mendasar dan beberapa di antaranya wajib diikuti:

1. Nama variabel hanya dapat terdiri atas huruf, angka, dan tanda garis bawah (<code>_</code>).
2. Nama variabel tidak boleh dimulai dari sebuah angka.
3. Nama variabel bersifat *case-sensitive* sehingga <code>variabelku</code> dan <code>Variabelku</code> tidak sama di mata Python dan dapat digunakan bersama-sama dalam satu program.
4. Nama variabel dapat dibuat sepanjang mungkin namun disarankan bahwa suatu baris program tidak melebihi 79 karakter.
5. Untuk nama variabel yang seharusnya terdiri dari spasi, salah satu dari kedua metode ini dapat digunakan:
   1. snake_case --> my_variable_yeay
   2. mixedCase -> myVariableYeay
6. Disarankan untuk menggunakan nama variabel yang representatif terhadap data yang akan diberikan kepada variabel tersebut.
   1. Do: username, email, nilai_pi
   2. Don't: xyz, ashaihsia, xzxz

Contoh:

~~~python
course_name = "Dasar-Dasar Pemrograman 0"
course_id = "DZE00001"
~~~

