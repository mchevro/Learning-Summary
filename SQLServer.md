# MS. SQL SERVER Docs
<p align="center">
  <img src="https://user-images.githubusercontent.com/67460437/144825129-7a33d901-6527-41f9-9a7e-502d07bc65d5.png">
</p>

## Daftar Isi 📝
- [Tipe Data](#tipe-data)
  * [Numerik](#numerik)
  * [Character Strings](#character-strings)
- [SQL Commands](#sql-commands)
  * [Data Definition Language](#data-definition-language)
    + [CREATE](#create)
      - [Membuat Database](#membuat-database)
      - [Membuat Table](#membuat-table)
    + [ALTER](#alter)
      - [ADD Column](#add-column)
      - [Modify Column](#modify-column)
      - [DROP Column](#drop-column)
    + [DROP](#drop)
      - [Hapus Database](#hapus-database)
      - [Hapus Table](#hapus-table)
- [Refrensi](#refrensi)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>



## Tipe Data
### Numerik
|   Tipe   | Ukuran Memori |                      Rentang Nilai                     |
|:--------:|:-------------:|:------------------------------------------------------:|
|  BigInt  |     8 Byte    | -9,223,372,036,854,775,808 - 9,223,372,036,854,775,807 |
|    Int   |     4 Byte    | -2,147,483,648 - 2,147,483,647                         |
| SmallInt |     2 Byte    | -32,767 - 32,768                                       |
|  TinyInt |     1 Byte    | 0-255                                                  |
|    Bit   |     1 Byte    | 1                                                      |
|  Decimal |  6 - 17 Byte  | -10^38+1 - 10^38-1                                     |

### Character Strings
|      Tipe     |   Ukuran Memori   |   Rentang Nilai   |
|:-------------:|:-----------------:|:-----------------:|
|      Char     |       n Byte      | 0 - 8000 chars    |
|    Varchar    |  n Byte + 2 Byte  | 0 - 8000 chars    |
| Varchar (max) |  n Byte + 2 Byte  | 2 ^ 31 chars      |
|      Text     | n Bytes + 4 Bytes | 0 - 2,147,483,647 |

## SQL Commands
<p align="center">
  <img src="https://user-images.githubusercontent.com/67460437/144828875-2ed8d476-2962-4a9d-ac40-d0184b7d7f77.png" width=750>
</p>

### Data Definition Language
#### CREATE
##### Membuat Database
```sql
/*Template*/
CREATE DATABASE nama_database;

/*Example*/
CREATE DATABASE kampus;
```

##### Membuat Table
```sql
/*Template*/
CREATE TABLE nama_table(
    column1 data_type,
    column2 data_type
);

/*Example*/
CREATE TABLE Mahasiswa(
    npm_mhs varchar(10) NOT NULL PRIMARY KEY,
    nama_mhs varchar(30),
    umur_mhs tinyint
);
```

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### ALTER
Perintah untuk merubah atau memodifikasi tabel yang sudah ada, seperti membuat kolom baru, modifikasi kolom ataupun menghapus kolom.
##### Tambah Column
```sql
/*Template*/
ALTER TABLE nama_tabel 
ADD nama_kolom tipe_data;

/*Example*/
ALTER TABLE Mahasiswa
ADD alamat_mhs varchar(50);
```

##### Edit Column
```sql
/*Template*/
ALTER TABLE nama_tabel 
ALTER COLUMN nama_kolom tipe_data;

/*Example*/
ALTER TABLE nama_tabel 
ALTER COLUMN alamat_mhs varchar(30);
```

##### Hapus Column
```sql
/*Template*/
ALTER TABLE nama_tabel
DROP COLUMN nama_kolom;

/*Example*/
ALTER TABLE Mahasiswa
DROP COLUMN alamat_mhs;
```

##### Tambah Foreign Key
Perintah ini digunakan ketika column sudah dibuat tetapi lupa membuat foreign key saat **CREATE TABLE**.
```sql
/*Template*/
ALTER TABLE nama_tabel1
ADD FOREIGN KEY(nama_kolom1) REFERENCES nama_tabel2(nama_kolom2)

/*Example*/
ALTER TABLE Mahsiswa
ADD FOREIGN KEY(kode_jur) REFERENCES Jurusan(kode_jur)
```

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### DROP
##### Hapus Database
```sql
/*Template*/
DROP DATABASE nama_database;

/*Example*/
DROP DATABASE kampus;
```

##### Hapus Table
```sql
/*Template*/
DROP TABLE nama_table;

/*Example*/
DROP TABLE Mahasiswa;
```

## Refrensi
- https://www.sqlservertutorial.net/sql-server-basics/sql-server-data-types/
- https://www.w3schools.com/sql/default.asp
- https://www.nesabamedia.com/pengertian-ddl/
- https://www.apacara.com/tutorial/mariadb/alter-table-merubah-menambahkan.html
