# CPP-Docs
<p align="center">
  <img src="https://user-images.githubusercontent.com/67460437/141405878-e3fe0b24-4841-4594-9682-825aeedd3fad.png">
</p>

## Daftar Isi 📝
- [Tipe Data](#tipe-data)
- [Basic Program](#basic-program)
- [Konstanta](#konstanta)
  * [Pengertian](#pengertian)
  * [Syntax](#syntax)
- [Variable](#variable)
  * [Pengertian](#pengertian-1)
  * [Ketentuan](#ketentuan)
  * [Syntax](#syntax-1)
- [Perintah Keluaran](#perintah-keluaran)
  * [Pengertian](#pengertian-2)
  * [Syntax](#syntax-2)
- [Perintah Masukan](#perintah-masukan)
  * [Pengertian](#pengertian-3)
  * [Syntax](#syntax-3)
- [Operator](#operator)
  * [Pengertian](#pengertian-4)
  * [Sifat Operator](#sifat-operator)
  * [Operator Aritmatika](#operator-aritmatika)
  * [Hirarki Operator Aritmatika](#hirarki-operator-aritmatika)
  * [Operator Relasi](#operator-relasi)
  * [Operator Logika](#operator-logika)
- [Operasi Kondisi](#operasi-kondisi)
  * [Pengertian](#pengertian-5)
  * [IF](#if)
    + [Syntax](#syntax-4)
  * [IF - ELSE](#if---else)
    + [Syntax](#syntax-5)
  * [Nested IF](#nested-if)
    + [Syntax](#syntax-6)
  * [IF - ELSE Majemuk](#if---else-majemuk)
    + [Syntax](#syntax-7)
- [Perintah Perulangan](#perintah-perulangan)
  * [For](#for)
    + [Syntax](#syntax-8)
  * [Nested For](#nested-for)
    + [Syntax](#syntax-9)
- [Refrensi](#refrensi)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>



## Tipe Data
|       Tipe       | Ukuran Memori |                      Rentang Nilai                     |                  Deskripsi                 | *Format Character  |
|:----------------:|:-------------:|:------------------------------------------------------:|:------------------------------------------:|:------------------:|
|      `Char`      |     1 Byte    |                       -128 - 127                       | Untuk Menyimpan Satu Karakter ('A')        | %c                 |
|       `Int`      |     4 Byte    |             -2,147,483,648 - 2,147,483,647             | Bilangan Bulat Negatif Dan Positif         | %d                 |
|  `Unsigned Int`  |     4 Byte    |                    0 - 4,294,967,295                   | Bilangan Bulat Positif                     | %u                 |
|      `Short`     |     2 Byte    |                    -32,768 - 32,767                    | Bilangan Bulat Negatif Dan Positif         |                    |
| `Unsigned Short` |     2 Byte    |                       0 - 65,535                       | Bilangan Bulat Positif                     |                    |
|      `Long`      |     8 Byte    | -9,223,372,036,854,775,808 - 9,223,372,036,854,775,807 | Bilangan Bulat Negatif Dan Positif         |                    |
|  `Unsigned Long` |     8 Byte    |             0 - 18,446,744,073,709,551,615             | Bilangan Bulat Positif                     |                    |
|      `Float`     |     4 Byte    |                     +/- 3.4 x 1038                     | Bilangan Dengan Nilai Pecahan              |                    |
|     `Double`     |     8 Byte    |                     +/- 1.8 x 10308                    | Bilangan Dengan Nilai Pecahan Lebih Akurat |                    |
|     `Boolean`    |               |                       True/False                       | Merepresentasikan Nilai True/False         |                    |
|     `String`     |               |                                                        | Untuk Membuat Kata                         | %s                 |

## Basic Program
```c++
#include <iostream> //File Header
using namespace std; //Perintah Untuk Menggunakan Seluruh Library Standard

int main() {
    //Write Here
    cout << "Hii"; 
    return 0;
}
```

## Konstanta
### Pengertian
Konstanta adalah suatu nilai yang sifatnya tetap. Secara garis besar konstanta dapat dibagi menjadi dua bagia, yaitu : <br>
- Konstanta Bilangan
- Konstanta Teks
### Syntax
```c++
const tipe_data nama_konstanta = nilai_konstanta; //Template

const float phi = 3.14; //Example
```

## Variable
### Pengertian
Variable adalah suatu tempat untuk menampung data dimemori yang mempunyai nilai atau data yang dapat berubah-ubah selama proses program.
### Ketentuan
- Tidak boleh ada spasi (ex: nama hero), untuk spasi bisa diganti dengan tanda garis bawah (ex: nama_hero).
- Tidak boleh diawali dengan angka dan operator aritmatika.

### Syntax
```c++
tipe_data nama_variable = nilai_variable; //Template

string nama_hero = "Alucard"; //Example

```

## Perintah Keluaran
### Pengertian
Perintah keluar atau output digunakan untuk menampilkan informasi program ke layar.
### Syntax
```C++
printf("String", argumen-1, argumen-2, dst); //Template
cout << string/argumen; //Template

printf("Nama Hero : %s \n", nama_hero.c_str()); //Example
cout << "Nama Hero : " << nama_hero; //Example
```

## Perintah Masukan
### Pengertian 
Perintah masukan atau input digunakan untuk menerima masukan atau nilai dari user ke dalam program.
### Syntax
```C++
cin >> nama_variable; //Template

cin >> nama_hero; //Example
```

## Operator
### Pengertian
Operator merupakan simbol atau karakter yang biasa dilibatkan dalam program untuk melakukan sesuatu operasi atau manipulasi, seperti penjumlahan, pengurangan dan lain-lain. <br>

### Sifat Operator
|   Sifat   |                                            Deskripsi                                           |    Contoh   |
|:---------:|:----------------------------------------------------------------------------------------------:|:-----------:|
|  `Unary`  | Sifat unary pada operator adalah hanya melibatkan sebuah operand pada suatu operasi artimatik. |    -5,++5   |
|  `Binary` |   Sifat binary pada operator adalah melibatkan dua buah operand pada suatu operasi aritmatik.  |    4 + 8    |
| `Ternary` |  Sifat ternary pada operator adalah melibatkan tiga buah operand pada suatu operasi aritmatik. | (4 + 8) - 2 |

### Operator Aritmatika
| Operator |  Deskripsi  | Contoh |
|:--------:|:-----------:|:------:|
|    `*`   |  Perkalian  |  4 * 5 |
|    `/`   |  Pembagian  |  4 / 5 |
|    `%`   |  Sisa Bagi  |  4 % 5 |
|    `+`   | Penjumlahan |  4 + 5 |
|    `-`   | Pengurangan |  4 - 5 |

### Hirarki Operator Aritmatika
|  Operator  |                                     Deskripsi                                     |
|:----------:|:---------------------------------------------------------------------------------:|
| `* atau /` | Tingkatan operator sama, penggunanya tergantung letak, yang di depan didahulukan. |
|     `%`    |                                   Sisa Pembagian                                  |
| `- atau +` | Tingkatan operator sama, penggunanya tergantung letak, yang di depan didahulukan. |

### Operator Relasi
Operator relasi digunakan untuk membandingkan dua buah nilai. Hasil dari perbandingan operator ini menghasilkan nilai numerik 1 (true) atau 0 (false).
| Operator |              Deskripsi              |  Contoh  |
|:--------:|:-----------------------------------:|:--------:|
|   `==`   | Sama Dengan (bukan pemberian nilai) | 10 == 10 |
|   `!=`   |          Tidak Sama Dengan          | 10 != 12 |
|    `>`   |              Lebih Dari             |  10 > 8  |
|   `>=`   |        Lebih Dari Sama Dengan       |  10 >= 8 |
|    `<`   |             Kurang Dari             |  10 < 12 |
|   `<=`   |       Kurang Dari Sama Dengan       | 10 <= 12 |

### Operator Logika
| Operator | Deskripsi |         Contoh         |
|:--------:|:---------:|:----------------------:|
|   `&&`   |    AND    |   true && true = true  |
|  `\|\|`  |     OR    | true \|\| false = true |
|    `!`   |    NOT    |      true = false      |

## Operasi Kondisi
### Pengertian
Pernyataan percabangan digunakan untuk memecahkan persoalan untuk mengambil suatu keputusan di antara sekian pernyataan yang ada.
### IF
Pernyataan if mempunyai pengertian "Jika kondisi bernilai benar, maka perintah akan dikerjakan dan jika tidak memenuhi syarat maka akan diabaikan".
#### Syntax
```C++
//Template
if(kondisi){
    Pernyataan;
}
    
//Example
if(10 > 9){
    cout << "Pernyataan Benar, Karena 10 Lebih Besar Dari 9";
}

```
### IF - ELSE
Pernyataan if mempunyai pengertian "Jika kondisi bernilai benar, maka perintah-1 akan dikerjakan dan jika tidak memenuhi syarat maka akan mengerjakan perintah-2 (else)".

#### Syntax
```C++
//Template
if(kondisi){
    perintah-1;
}else{
    perintah-2;
}
    
//Example
if(10 > 20){
    cout << "Pernyataan Benar, Karena 20 Lebih Kecil Dari 10";
}else{
    cout << "Pernyataan Salah, Karena 20 Lebih Besar Dari 10";
}
```

### Nested IF
Nested if merupakan pernyataan if yang berada di dalam pernyataan if yang lain.
#### Syntax
```C++
//Template
if(kondisi){
    if(kondisi){
        perintah;
    }else{
        perintah;
    }
}else{
    perintah;
}

//Example
int umur = 15; 
if(umur <= 18){
    if(umur<= 10){
        cout << "Anak-Anak";
    }else{
        cout << "Remaja";
    }
}else{
    cout << "Bukan Usia Anak Maupun Remaja";
}
```

### IF - ELSE Majemuk
Bentuk dari if-else majemuk sebernya mirip dengan nested if. Keuntungan penggunaan if-else majemuk dibanding dengan nested if adalah bentuk penulisanya yang lebih sederhana.
#### Syntax
```C++
//Template
if(kondisi){
    perintah;
}else if(kondisi){
    perintah;
}else{
    perintah;
}

//Example
int umur = 15; 
if(umur <= 10){
    cout << "Anak-Anak";
}else if(umur <= 18){
    cout << "Remaja";
}else{
    cout << "Bukan Usia Anak Maupun Remaja";
}
```

## Perintah Perulangan
Beris kode atau instruksi yang dieksekusi oleh komputer secara berulang-ulang sampai suatu kondisi tertentu terpenuhi.
### For
Perulangan for merupakan perulangan yang termasuk dalam *couted loop*, karena sudah jelas berapa kali ia akan mengulang.
#### Syntax
```c++
//Template
for(inisialisasi; kondisi; interasi){
  pernyataan;
}

//Example
for(int i = 0; i <= 5; i++){
    cout << i << endl;
}
```
### Nested For
Penggunaan nested-for, perulangan yang didalam telebih dahulu dihitung hingga selesai, baru kemudian perulangan yang diluar diselesaikan.
#### Syntax
```c++
//Template
for(inisialisasi; kondisi; interasi){
    for(inisialisasi; kondisi; interasi){
    pernyataan;
  }
}

//Example
for(int x = 1; x <= 5; x++){
    for(int y = x; y <= 5; y++){
        cout << x << " ";
    }
    cout << endl;
}
```


## Refrensi 
- "Buku Panduan Pemrograman C++" Frieyadie
- https://www.geeksforgeeks.org/c-data-types/
- https://www.cplusplus.com/reference/cstdio/printf/
- https://www.petanikode.com/cpp-input-output/
- https://kelasprogrammer.com/contoh-program-c-if-bersarang-nested-if/
- https://jagongoding.com/python/dasar/perulangan-for/
- https://www.petanikode.com/cpp-perulangan/
