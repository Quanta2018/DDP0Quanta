# Latihan Pekan 1: Variabel dan Tipe Data

**Dasar-Dasar Pemrograman 0** | Penulis: Muhammad Dzikra Muzaki, Rafi Muhammad Daffa



## Daftar Isi

Materi Pekan 1

L1. Konversi Masalah ke Ekspresi Python (Bahasa Inggris)

L2. Pencarian Keluaran dan Tipe Data (Bahasa Inggris)

L3. Pemecahan Masalah (Bahasa Inggris)

L4. Latihan Pemrograman (Bahasa Indonesia)

L5. Penguatan Teori (Bahasa Indonesia)



## L1. Konversi Masalah ke Ekspresi Python

Convert the following statements to a Python algebraic expression using arithmetic operators and/or functions:

1. The average age of Azis (age 22), Dzikra (age 19), and Rafi (age 34)
2. 3 to the 7th power
3. The number of times 64 goes to 572 rounded to the integer quotient of the result
4. The sum of 3 squared and 4 squared is equal to 25
5. The absolute value of the difference between Alghi’s height (168 cm) and Okto’s height (174 cm)
6. The lowest price among the following prices: Rp 186.000, Rp 49.000, and Rp 144.000



## L2. Pencarian Keluaran dan Tipe Data

What is the result and data type of the following statements?

1. 2 * 17.5
2. ‘-7’ + ‘19’
3. (108/2) == ‘54’
4. ‘24’ * 3
5. “Python is easy” != “python is easy”
6. 15 + (-4) * 6



## L3. Pemecahan Masalah

Fill in the blanks to complete the program as described below:

1. A program that outputs the remainder of 91 divided by 13:

   ~~~python
   a = ... 
   b = ..... 13 
   print(...)
   ~~~

2. A program that switches the integer value of a and b without using a third variable:

   ~~~python
   a = 17 
   b = 5 
   a = ... 
   b = ... 
   a = ...
   ~~~

3. A program that outputs the result if your score is greater than or equal to 80 and your age is lower than or equal to 19:

   ~~~python
   score = 97 
   age = 18
   result_if_passed = 'You passed!' 
   result_if_failed = 'Sad :('
   if (...): 
       print(result_if_passed)
   else: 
       print(...)
   ~~~

   

## L4. Latihan Pemrograman

### 1. Cek Angkatan dari NPM

Coba kalian amati Nomor Pokok Mahasiswa (NPM) yang tertera pada Kartu Identitas Mahasiswa (KIM) kalian. Dengan sistem penomoran NPM yang ada sekarang, kalian bisa mengetahui angkatan dari seorang mahasiswa dari NPM yang ia miliki (tepatnya pada dua digit pertama dari NPM tersebut).

> **Contoh**:
>
> NPM kamu 1906128302, berarti kamu berasal dari angkatan 2019 (19) 

Buatlah suatu program yang dapat menerima *input* berupa NPM suatu mahasiswa dan mengecek apabila mahasiswa tersebut adalah angkatan 2019 atau tidak menggunakan **operasi matematika**.

Contoh Input:

```
Masukkan NPM yang akan dicek: 1906128302
```

Contoh Output:

```
Apakah mahasiswa tersebut angkatan 2019? True
```

Asumsi dan petunjuk berikut ini mungkin akan membantu kalian:

1. Asumsikan bahwa pengguna akan memasukkan NPM utuh (10 digit).

2. Fungsi <code>print()</code> dapat menerima beberapa argumen dan akan mencetak seluruh argumen dipisahkan dengan spasi:

   ```python
   >>> print("Fasilkom", "UI")
   Fasilkom UI
   ```

3. Program ini tidak membutuhkan <code>if else</code>, kalian cukup menggunakan operator pembanding.

### 2. Perhitungan Kalor Air

Dalam menghitung jumlah kalor yang dibutuhkan/dilepaskan untuk menaikkan/menurunkan suhu suatu benda, kalian dapat menggunakan rumus berikut ini:

> #### Q = m * c * &Delta;t
>
> Q = Kalor yang dibutuhkan/dilepaskan
> m = Massa benda (gram)
> c = Kalor jenis benda (J/gram * &deg;C)
> &Delta;t = Perubahan suhu (&deg;C, nilai mutlak)

Pada program yang kalian buat, terimalah *input* berupa massa air yang akan dipanaskan/didinginkan, suhu awal, dan suhu akhir. Kemudian, hitunglah kalor yang dibutuhkan/dilepaskan dan sajikan hasilnya kepada pengguna. (Untuk c, gunakan kalor jenis air yaitu 4.186).

Contoh Input:

```
Masukkan massa air yang akan dipanaskan/didinginkan (gram): 500
Masukkan suhu awal (celcius): 1
Masukkan suhu akhir (celcius): 95
```

Contoh Output:

```
Hasil: 196742.0 J
```

Asumsi dan petunjuk di bawah ini akan membantu kalian:

1. Asumsikan bahwa suhu berada di rentang 0 - 100&deg;C dan sepenuhnya berbentuk cair (tidak ada kalor lebur atau didih).
2. Gunakan nilai mutlak saat menghitung perubahan suhu.



## L5. Penguatan Teori

1. Apa yang salah dari program berikut ini?

   ```python
   import math
   
   radius = input("Radius lingkaran: ")
   area = math.pi * (radius ** 2)
   ```

2. Apa yang salah dari program berikut ini?

   ```python
   print("15"*2)
   ```

3. Apa hasil yang dikeluarkan oleh program berikut ini?

   ```python
   print(1 == "1")
   print(1 == int("1"))
   ```

4. Apa hasil yang dikeluarkan oleh program berikut ini?

   ```python
   print("A" < "b")
   ```

5. Dalam Python, bilangan bulat direpresentasikan dengan tipe data <code>             </code> .

6. Implementasi tanda <code>+</code> bisa berbeda sesuai konteks tipe data yang digunakan. Pada tipe data String, apa yang dilakukan jika dua buah String dijumlahkan?

7. Argumen yang ada pada fungsi <code>input("Sesuatu")</code> berfungsi sebagai <code>             </code>.