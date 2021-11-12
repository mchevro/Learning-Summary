# CPP-Docs

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
using namespace std; //Perintah Untuk Menggunakan Seluruh Library Standart

int main() {
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

## Refrensi :
- "Buku Panduan Pemrograman C++" Frieyadie
- https://www.geeksforgeeks.org/c-data-types/
- https://www.cplusplus.com/reference/cstdio/printf/
- https://www.petanikode.com/cpp-input-output/
