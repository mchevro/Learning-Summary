# CSharp-Docs

## Tipe Data
| Tipe      | Deskripsi                                     | Rentang Nilai |
| --------- | --------------------------------------------- | ------------- |
| `bool`    | Merepresentasikan nilai true/false            | True Atau False 
| `byte`    | Integer tak-bertanda 8-bit                    | 0-255
| `char`    | Untuk Menyimpan karakter (1 Huruf)            | Tidak Tersedia
| `decimal` | Nilai Numerik Untuk Perhitungan Keuangan      | 28 Angka Penting
| `double`  | Bilangan Dengan Nilai Pecahan (Lebih Akurat)  | -1.79769313486232e308 - 1.79769313486232e308	
| `float`   | Bilangan Dengan Nilai Pecahan                 | -3.402823e38 - 3.402823e38
| `int`     | Bilangan Bulat 32-Bit                         | -2,147,483,648 - 2,147,483,647
| `long`    | Bilangan Bulat 64-Bit                         | -9,223,372,036,854,775,808 - 9,223,372,036,854,775,807
| `sbyte`   | Bilangan Bulat 8-bit                          | -128 - 127
| `short`   | Bilangan Bulat 16-Bit                         | -32,768 - 32,767
| `uint`    | Bilangan Bulat Positif 32-Bit                 | 0 - 4,294,967,295
| `ulong`   | Bilangan Bulat Positif 64-Bit                 | 0 - 18,446,744,073,709,551,615
| `ushort`  | Bilangan Bulat Positif 16-Bit                 | 0 - 65,535

## Loop For
```C#
//Contoh
for (inisialisasi; kondisi; iterasi) statemen; //Syntax

for (int i=0; i < 10; i++) Console.WriteLine(i); // Nilai i kurang dari 10 adalah *true*
```
Eksekusi program secara berulang menggunakan loop *for*. **inisialisasi** menetapkan nilai awal dari variable kendali loop. **kondisi** adalah ekspresi Boolean yang menguji variable kendali loop. Jika ekspresi kondisi bernilai true, maka loop for akan berlanjut ber**iterasi**

## Deklarasi Variable
```C#
//Contoh
int a; //Deklarasi Satu Variable
int a,b,c; //Deklarasi 3 Variable Dalam Satu Baris Code
```
Pendeklarasian variable bisa dilakukan dengan manuliskan statemen deklarasi yang sama. Hanya perlu memisahkan nama-nama variable dengan tanda koma.

## Operator Aritmatika
| Operator | Arti |
| -------- | ---- |
| `+` | Penjumalahn   |
| `-` | Pengurangan   |
| `*` | Perkalian     |
| `/` | Pembagian     |
```C#
//Contoh
int a = 10 * 10; //Menghitung Perkalian
Console.WriteLine(a);
//Result : 100
```

## Operator Ralasional
| Operator | Arti |
| -------- | ---- |
| `<` | Kurang Dari               |
| `<=`| Kurang Dari Sama Dengan   |
| `>` | Lebih Dari                |
| `>=`| Lebih Dari Sama Dengan    |
| `==`| Sama Dengan               |
| `!=`| Tidak Sama Dengan         |

## Statemen Kondisi
```C#
//Contoh
if (kondisi) statemen; //Syntax

if (1 < 2) Console.WriteLine("Benar"); //Jika Hasil 1 Kurang Dari 2 Bernilai *True* Maka Akan Mencetak Tulisan *Benar*
```
**Kondisi** adalah sebuah ekspresi Boolean (bernilai true atau false). Jika **kondisi** bernilai true, maka **statemen** akan dieksekusi.

















