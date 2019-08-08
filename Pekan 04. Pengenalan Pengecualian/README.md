# Pengenalan Pengecualian

**Dasar-Dasar Pemrograman 0** | Penulis: Rafi Muhammad Daffa



## Daftar Isi

4A. Kesalahan Umum dalam Pemrograman

4B. Dokumentasi Program

4L. Latihan (Bergabung dengan 3L)



## 4A. Kesalahan Umum dalam Pemrograman

Dalam membuat sebuah program, kenyataan pahit yang terjadi adalah tidak ada program yang sempurna. Bahkan, program yang sudah didesain sedemikian rupa oleh tim yang besar masih mungkin mengalami kesalahan. Kesalahan tersebut dapat terjadi karena berbagai macam hal, misalnya:

1. Kalkulasi aritmatis yang meleset (presedensi, asosiasi, dan lain-lain).
2. Masukan pengguna yang tidak sesuai dengan rancangan program.
3. *Typing error*.
4. Dan-lain-lain.

Oleh karena itu, kita sebagai perancang program harus mampu mengidentifikasi kesalahan-kesalahan umum dalam pemrograman dan solusi yang dapat ditempuh untuk mencegah kesalahan tersebut terjadi.

Secara umum, ada tiga macam kesalahan dalam pemrograman, yaitu *syntax error*, *runtime error*, dan *logic error*.

### *Syntax Error*

Kesalahan sintaks mencakup segala kesalahan yang berkaitan dengan "kesastraan" Python. Kesalahan ini dapat mencakup namun tidak terbatas pada penggunaan tanda baca, indentasi, dan kesalahan ketik. Kesalahan ini merupakan kesalahan yang paling pertama ditangkap oleh Python dan akan mencegah program tersebut untuk dijalankan sama sekali. Contohnya:

~~~python
dev fungsi(arg1,arg2):
    print(arg1)

def fungsi2(arg3,arg4)
	print(arg3)
    
def fungsi3(arg5,arg6):
print(arg5)
~~~

Python akan secara otomatis menangkap kesalahan seperti ini dan akan dipresentasikan di IDLE dengan arsiran merah dan akan dicetak di Console untuk yang lainnya.

### *Runtime Error*

Kesalahan yang masuk dalam kategori ini adalah kesalahan yang terjadi pada saat programnya berjalan. Apabila kesalahan dalam kategori ini terjadi, program akan diberhentikan secara otomatis. Namun, hal ini tidak akan mencegah Python untuk menjalankan program tersebut pada awalnya. Mayoritas *runtime error* memiliki nama pengecualian khusus yang dapat digunakan untuk melakukan analisis kesalahan. Kesalahan yang lazim muncul adalah sebagai berikut:

1. <code>NameError</code>: Umumnya terjadi karena suatu variabel yang belum dideklarasikan digunakan untuk sesuatu.

   ~~~python
   print(a)
   ~~~

2. <code>TypeError</code>: Umumnya terjadi karena terdapat ketidakcocokan antara suatu tipe data dengan operasi yang dikenakan padanya atau ada tabrakan antar-tipe data.

   ~~~python
   "A" ** "3"
   ~~~

3. <code>ZeroDivisionError</code>: Kesalahan aritmatika khusus yang melibatkan pembagian suatu angka dengan nol.

   ~~~python
   1/0
   ~~~

4. <code>OverflowError</code>: Umumnya terjadi karena tipe-tipe data yang memiliki batas kapasitas telah melampaui batasnya.

   ~~~python
   310235.60481380235**121
   ~~~

5. <code>IndexError</code>: Umumnya terjadi ketika indeks suatu data yang dipanggil tidak ada.

   ~~~python
   my_lst = ["Type","Me"]
   my_lst[10000]
   ~~~

Setiap kesalahan dalam tipe ini terjadi, Python akan memberhentikan program tersebut dan akan memberikan laporan terhadap baris kode terakhir yang dijalankan sebelum kesalahan terjadi dan deskripsi singkat dari kesalahan yang terjadi. Laporan ini disebut *traceback* dan disusun seperti ini:

~~~
Traceback (most recent call last):
  File "<pyshell#2>", line 1, in <module>
    310235.60481380235**121
OverflowError: (34, 'Result too large')
~~~



### *Logic Error*

Kesalahan ini merupakan kesalahan yang paling sulit dicari karena Python tidak akan bisa mengetahui bahwa program tersebut memiliki kesalahan dengan jenis ini. Kesalahan ini bergantung pada pengetahuan perancang program dalam alur program yang diharapkan pada awalnya. Mari kita ambil contoh dalam perhitungan kombinasi:

~~~python
factorial(n)/factorial(r)*factorial(n-r)
~~~

Seharusnya, perhitungan <code>factorial(r)*factorial(n-r)</code> berada di tingkatan yang sama (di bawah pembagian) seperti berikut ini:

![](assets/combi.png)

Karena Python hanya mengetahui bahwa pembagian dan perkalian memiliki presedensi yang sama, maka Python akan mengevaluasi rumus tadi dari kiri kanan sehingga akan dibagi terlebih dahulu kemudian dikali.



## 4B. Dokumentasi Program

Salah satu hal baik yang dapat membantu perancang program dalam membuat program yang baik adalah memberikan dokumentasi yang memadai terhadap program yang dirancang. Dokumentasi ini diimplementasi dalam bentuk catatan/komentar yang diberikan di antara program yang dapat membantu penjelasan dari program tersebut. Ada dua cara untuk menyusun sebuah komentar:

1. *Inline*: Komentar dapat ditempatkan di seluruh penjuru kode (di samping, di atas, maupun di bawah). Cara menggunakannya adalah menambahkan tanda pagar (<code>#</code>) sebelum menuliskan komentar.

   ~~~python
   fav_course = [] # Implemented as 2-D List
   ~~~

   ~~~python
   # Variable must contain Integer only
   counter = 0
   ~~~

2. *Block*: Komentar ini hanya dapat ditempatkan di atas atau di bawah suatu baris kode. Namun, komentar ini dapat dibuat dengan baris rangkap. Cara menggunakannya adalah menambahkan tiga tanda petik (<code>"""</code>) di awal dan di akhir blok komentar.

   ~~~python
   """
   Author: Rafi Muhammad Daffa
   Date: 8 August 2019
   Version: 0.1alpha1
   """
   startprogram()
   ~~~

3. *Docstring*: Komentar ini merupakan pengembangan khusus dari *block* yang ditempatkan di bawah definisi fungsi. Komentar ini adalah satu-satunya komentar yang akan dianggap oleh Python dan dijadikan sebagai bentuk dokumentasi dari fungsi yang didefinisikan tersebut.

   ~~~python
   def print_if_even(number):
       """
       This program prints a number only if it is even
       """
       if number%2 == 0:
           print(number)
   ~~~

   Karakteristik spesial lain yang dimiliki oleh komentar seperti ini adalah komentar tersebut dapat diakses saat program berjalan dengan menggunakan fungsi <code>help(nama_fungsi)</code>. Contohnya, anggaplah ada sebuah fungsi <code>hitungTHB</code>.

   ~~~python
   help(hitungTHB)
   ~~~

   Hasil yang dicetak adalah:

   ~~~
   Help on function hitungTHB in module __main__:
   
   hitungTHB(berangkat, datang)
       Hitung Harga THB untuk stasiun yang menerima THB
   ~~~

Dalam menyusun sebuah program, idealnya setiap komentar di atas berkontribusi dalam menjelaskan sebuah program. Misalnya, ada sebuah konsep yang mendasari pembuatan blok kode yang kemungkinan akan menimbulkan kebingungan di kemudian hari. Kamu dapat "mencatat" hal tersebut dalam bentuk komentar untuk mencegah lupa saat program kamu akan dipakai atau dikembangkan oleh dirimu sendiri dan orang lain.

