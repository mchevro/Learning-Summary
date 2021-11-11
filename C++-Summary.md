# CPP-Docs

## Tipe Data
|       Tipe       | Ukuran Memori |                      Rentang Nilai                     | Deskripsi                                  |
|:----------------:|:-------------:|:------------------------------------------------------:|--------------------------------------------|
|      `Char`      |     1 Byte    |                       -128 - 127                       | Untuk Menyimpan Satu Karakter ('A')        |
|       `Int`      |     4 Byte    |             -2,147,483,648 - 2,147,483,647             | Bilangan Bulat Negatif Dan Positif         |
|  `Unsigned Int`  |     4 Byte    |                    0 - 4,294,967,295                   | Bilangan Bulat Positif                     |
|      `Short`     |     2 Byte    |                    -32,768 - 32,767                    | Bilangan Bulat Negatif Dan Positif         |
| `Unsigned Short` |     2 Byte    |                       0 - 65,535                       | Bilangan Bulat Positif                     |
|      `Long`      |     8 Byte    | -9,223,372,036,854,775,808 - 9,223,372,036,854,775,807 | Bilangan Bulat Negatif Dan Positif         |
|  `Unsigned Long` |     8 Byte    |             0 - 18,446,744,073,709,551,615             | Bilangan Bulat Positif                     |
|      `Float`     |     4 Byte    |                     +/- 3.4 x 1038                     | Bilangan Dengan Nilai Pecahan              |
|     `Double`     |     8 Byte    |                     +/- 1.8 x 10308                    | Bilangan Dengan Nilai Pecahan Lebih Akurat |
|     `Boolean`    |               |                       True/False                       | Merepresentasikan Nilai True/False         |

## Basic Program
```c++
#include <iostream> //File Header
using namespace std; //Perintah Untuk Menggunakan Seluruh Library Standart

int main() {
    cout << "Hii"; 
    return 0;
}
```

## Refrensi :
- "Buku Panduan Pemrograman C++" Frieyadie
- https://www.geeksforgeeks.org/c-data-types/
