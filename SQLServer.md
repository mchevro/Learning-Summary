# MS. SQL SERVER Docs
<p align="center">
  <img src="https://user-images.githubusercontent.com/67460437/144825129-7a33d901-6527-41f9-9a7e-502d07bc65d5.png">
</p>

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
#### Membuat Database
```sql
/*Template*/
CREATE DATABASE nama_database;

/*Example*/
CREATE DATABASE kampus;
```

#### Membuat Table
```sql
/*Template*/
CREATE TABLE nama_table(
    column1 data_type,
    column2 data_type
);

/*Example*/
CREATE TABLE Mahasiswa(
    npm_mhs varchar(10),
    nama_mhs varchar(30),
    umur_bhs tinyint
)
```




## Refrensi
- https://www.sqlservertutorial.net/sql-server-basics/sql-server-data-types/
- https://www.w3schools.com/sql/default.asp
- https://www.nesabamedia.com/pengertian-ddl/
