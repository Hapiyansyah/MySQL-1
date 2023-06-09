# PRAKTIKUM 1

1. Buat sebuah database dengan nama latihan2!
```
CREATE DATABASE latihan2;
```
![foto1](foto/Ss1.png)

2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan2!
```
CREATE TABLE biodata (nama varchar(15), alamat TEXT);
```
![foto2](foto/ss2.png)

3. Tambahkan sebuah kolom keterangan (varchar(15), sebagai kolom terakhir!
```
ALTER TABLE biodata ADD COLUMN phone VARCHAR(15) AFTER alamat;
```
![foto3](foto/ss3.png)

4. Tambahkan kolom id (int11) diawal (sebagai kolom pertama)!
```
ALTER TABLE biodata ADD COLUMN id int(11) FIRST;
```
![foto4](foto/ss4.png)

5. Sisipkan sebuah kolom dengan nama phone (varchar(15) setelah kolom alamat!
```
ALTER TABLE biodata ADD COLUMN keterangan  VARCHAR(15) AFTER phone;
```
![foto5](foto/ss5.png)

6. Ubah tipe data kolom id menjadi char(11)!
```
ALTER TABLE biodata MODIFY id char(11);
```
![foto6](foto/ss6.png)

7. Ubah nama kolom phone menjadi hp (varchar(20)!
```
ALTER TABLE biodata CHANGE phone hp VARCHAR(20);
```
![foto7](foto/ss7.png)

8. Tambahkan kolom email setelam kolom hp!
```
ALTER TABLE biodata ADD COLUMN email VARCHAR(15) AFTER hp;
```
![foto8](foto/ss8.png)

9. Hapus kolom keterangan dari tabel!
```
ALTER TABLE biodata DROP COLUMN keterangan;
```
![foto9](foto/ss9.png)

10. Ganti nama tabel menjadi data_mahasiswa!
```
ALTER TABLE biodata RENAME data_mahasiswa;
```
![foto10](foto/ss10.png)

11. Ganti nama field id menjadi nim!
```
ALTER TABLE data_mahasiswa CHANGE id nim VARCHAR(10);
```
![foto11](foto/ss11.png)

12. Jadikan nim sebagai PRIMARY KEY!
```
ALTER TABLE data_mahasiswa ADD PRIMARY KEY(nim);
```
![foto12](foto/ss12.png)

13. Jadikan kolom email sebagai UNIQUE KEY!
```
ALTER TABLE data_mahasiswa ADD UNIQUE KEY(email);
```
![foto13](foto/ss13.png)
 
# Evaluasi dan Pertanyaan

1. Apa yang dimaksud dengan int(11)?

Yang dimaksud int(11) artinya suatu data yang dipakai atau digunakan menggunakan tipe data int atau integer dengan length atau panjang karakter 11.

2. Ketika kita melihat struktur tabel denga perintah desc, ada kolom Null berisi YES dan NO. apa maksudnya?

Apabila Null berisi no, maka data tersebut nantinya akan dilakukan pengisian atau penginputan. Sedangkan apabila Null berisi yes, maka artinya data tersebut akan dikosongkan atau tidak dilakukan penginputan.
