# CPP-Docs
<p align="center">
  <img src="https://user-images.githubusercontent.com/67460437/141405878-e3fe0b24-4841-4594-9682-825aeedd3fad.png">
</p>

## Daftar Isi 📝
- [Tipe Data](#tipe-data)
- [Escape Sequences](#escape-sequences)
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
  * [Switch - Case](#switch---case)
    + [Syntax](#syntax-8)
- [Perintah Perulangan](#perintah-perulangan)
  * [For](#for)
    + [Syntax](#syntax-9)
  * [Nested For](#nested-for)
    + [Syntax](#syntax-10)
- [Array](#array)
  * [Pengertian](#pengertian-6)
  * [Syntax](#syntax-11)
  * [Array Satu Dimensi](#array-satu-dimensi)
    + [Syntax](#syntax-12)
  * [Array Dua Dimensi](#array-dua-dimensi)
    + [Syntax](#syntax-13)
  * [Array Tiga Dimensi](#array-tiga-dimensi)
    + [Syntax](#syntax-14)
- [Pretty Table](#pretty-table)
  * [Tanda Format. Pertaaan Kiri dan Kanan](#tanda-format-pertaaan-kiri-dan-kanan)
    + [Syntax](#syntax-15)
- [Function](#function)
    + [Syntax](#syntax-16)
- [Struktur](#struktur)
    + [Syntax](#syntax-17)
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

## Escape Sequences
| Symbol |        Description       |
|:------:|:------------------------:|
|  `\n`  | Membuat Baris Baru/Enter |
|  `\t`  | Horizontal Tab           |
|  `\v`  | Vertical Tab             |

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

### Switch - Case
Bentuk switch case merupakan pernyataan yang dirancang khusus untuk menangani pengambilan keputusan yang melibatkan sejumlah atau banyak alternatif. Pernyataan switch-case ini memiliki kegunaan yang sama seperti if - else majemuk, tetapi untuk memeriksa data yang bertipe karakter atau integer.
#### Syntax
```C++
//Template
switch(nama_variable){
  case konstanta-1:
      perintah;
      break;
      
  case konstanta-2:
      perintah;
      break;
      
  default:
      perintah;
      break;
}

//Example
char kode;
cout << "Input Kode Barang [A,B] : ";
cin >> kode;
    
switch(kode){
    case 'a':
    case 'A':
        cout << "Alat Olah Raga";
        break;
        
    case 'b':
    case 'B':
        cout << "Bola Basket";
        break;
    default:
        cout << "Kode Tidak Ada!";
        break;
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

## Array
### Pengertian
Variable array adalah tipe terstruktur yang terdiri dari sejumlah elemen yang mempunyai tipe data yang sama. Suatu array mempunyai jumlah elemen yang tetap. Banyaknya elemen dalam array ditunjukkan oleh suatu indeks yang berfungsi untuk membedakan variable yang satu dengan variable lainnya.
![image](https://user-images.githubusercontent.com/67460437/141649960-a6455fe1-bbc0-4648-a8a8-7b71af29c726.png)
### Syntax
```C++
//Template
tipe_data nama_array[jumlah_elemen] = {value_array};

//Example
char kata[5] = {'V','I','D','E','O'};
cout << "Kata Anda Di Indeks[1] Adalah : " << kata[1];
```

### Array Satu Dimensi
![image](https://user-images.githubusercontent.com/67460437/141698139-729ad887-ab71-4ca1-809c-efc3a0ff43b2.png)

Array satu dimensi yaitu kumpulan elemen-elemen identik yang hanya terdiri dari satu baris atau hanya satu kolom alamat penyimpanan data (indeks).
#### Syntax
```C++
//Template
tipe_data nama_array[jumlah_elemen] = {value_array};

//Example
string nama[3] = {"UZUMAKI NARUTO", "UCIHA SASUKE", "NARA SHIKAMARU"};

for(int i = 0; i < 3; i++){
    cout << "Value Array Index Ke - " << i << " = " << nama[i] << endl;
}
```

### Array Dua Dimensi
![image](https://user-images.githubusercontent.com/67460437/141698736-a7f5b9c4-3b41-416a-89e4-2cb79b275de2.png)

Array dua dimensi dalam bentuk baris dan kolom, dimana indeks pertama menunjukkan baris dan indeks kedua menunjukkan kolom.
#### Syntax
```C++
//Template
tipe_data nama_array[jumlah_baris][jumlah_kolom] = {nilai_array};

//Example
int nilai[2][5] = {{99, 89, 93, 87, 85}, {77, 85, 55, 64, 78}};
for(int i=0; i < 2; i++){
	for(int j=0; j < 5; j++){
		cout << nilai[i][j] << " ";
	}
	cout << endl;
}
```
### Array Tiga Dimensi
![image](https://user-images.githubusercontent.com/67460437/143504145-93109b7d-04dc-4f81-afc1-5309c6f248cc.png)

#### Syntax
```C++
//template 
tipe_data nama_array[jumlah_baris][jumlah_kolom][jumlah_isi_dari_baris] = {value}

//Syntax
int penjualan[2][2][3] = { {{99, 89, 100}, {100, 89, 20}}, {{99, 89, 50}, {99, 89, 40}} };
    
    cout << "---------------------------------------------------------------------------" << endl;
    cout << "Tahun\t\tHasil\t\t\t\tPenjualan Bulan" << endl;
    cout << "ke\t\tke\t\t-------------------------------------------" << endl;
    cout << "\t\t\t\t|Januari\t| Februari\t| Maret" << endl;
    cout << "---------------------------------------------------------------------------" << endl;
    
    
    for(int i=0; i<2; i++){
        for(int j=0; j<2; j++){
            cout << i+1 << "\t\t" << j+1 << "\t\t";
            for(int k=0; k<3; k++){
                cout << penjualan[i][j][k] << "\t\t";
            }
            cout << endl;
        }
        cout << endl;
    }
```

## Pretty Table
Fungsi *setiosflags()* merupakan suatu fungsi manipulator yang digunakan untuk mengatur sejumlah format keluaran data. Fungsi ini biasa ada pada fungsi cout(). File header yang harus disertakan adalah file header **iomanip**.
### Tanda Format. Pertaaan Kiri dan Kanan
Ada dua buah tanda format yang digunakan untuk perataan kiri dan kanan. Pengaturan lebar variable untuk rata kiri dan kanan ini dilakukan melalui fungsi *setw()*.
- **ios::left** digunakan untuk mengatur perataan sebelah kiri.
- **ios::right** digunakan untuk mengatur pertaan sebelah kanan.

#### Syntax
```C++
//Example
#include <iostream>
#include <iomanip>

using namespace std;

int main()
{
    string nama[2][2] = {{"Takiya Genji", "Shun Oguri"}, {"Yoshinobu Kuroiwa", "Suzunosuke Tanaka"}};
    
    cout << "Pemain Crows Zero" << endl;
    cout << "--------------------------------------------" << endl;
    cout << setiosflags(ios::left) << setw(5) << "No";
    cout << setiosflags(ios::left) << setw(24) << "Nama Samaran";
    cout << setiosflags(ios::left) << setw(15) << "Nama Asli";
    cout << endl;
    cout << "--------------------------------------------" << endl;
    for(int i=0; i<2; i++){
        cout << setiosflags(ios::left) << setw(5) << i+1;
        for(int j=0; j<2; j++){
            cout << setiosflags(ios::left)<<setw(24) << nama[i][j];
        }
        cout << endl;
    }

    return 0;
}
```

## Function
Fungsi (function) merupakan blok dari kode yang dirancang untuk melaksanakan tugas khusus. Kegunaan dari fungsi ini adalah :
- Untuk mengurangi pengulangan penulisan program yang sama.
- Agar program menjadi lebih terstruktur sehingga mudah dipahami dan dapat lebih dikembangkan.

#### Syntax
```C++
//Template
tipe_data nama_fungsi(argumen){	
	statemen;
}

//Example
#include <iostream>
using namespace std;

void garis(){
    cout << "----------------------";
}

int main(){
    garis();
    
    return 0;
}
```

## Struktur
Struktur (structure) digunakan untuk mengelompokan sejumlah data yang mempunyai tipe dan ukuran yang berbeda. Variable-variable yang membentuk sebuah struktur dinamakan elemen struktur.

#### Syntax
```C++
//Template 1
struct nama_struktur
{
	elemen_struktur 1;
	elemen_struktur 2;
	elemen_struktur 3;
};

//Template 2
struct
{
	elemen_struktur 1;
	elemen_struktur 2;
	elemen_struktur 3;
	
}nama_struktur;

//Example
#include <iostream>
using namespace std;

int main(){
    struct{
        string nama;
    }mahasiswa;
    
    mahasiswa.nama = "Naruto";
    
    cout << mahasiswa.nama;
    return 0;
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
- https://en.cppreference.com/w/cpp/language/escape
- https://www.youtube.com/watch?v=8WhUADLI4RQ
