# Biodata

Nama = Syafira Luthfi Azzahra

Kelas = TI.24.A.4

NIM = 321410353

# Struktur Kondisi
Penggunaan struktur kondisi menggunakan statement ```if```, Konsep pemrograman yang memungkinkan program untuk mengambil keputusan berdasarkan kondisi atau pernyataan tertentu. Struktur seleksi kondisi yang umum digunakan dalam Python

if : Digunakan untuk mengevaluasi suatu kondisi. Jika kondisi tersebut benar (True)

else : Digunakan untuk menentukan apa yang terjadi jika kondisi ```if``` adalah salah (False)

elif : digunakan untuk mengevaluasi beberapa kondisi jika kondisi ```if``` pertama salah, Python akan mengevaluasi kondisi ```elif``` anda bisa memiliki beberapa ```elif```

```python
nama = input("Masukkan nama:")
uts = input("Masukkan nilai UTS:")
uas = input("Masukkan nilai UAS:")
tugas = input("Masukkan nilai Tugas:")

akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4)
keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0]
if akhir > 80:
    huruf = "A"
elif akhir > 70:
    huruf = "B"
elif akhir > 50:
    huruf = "C"
elif akhir > 40:
    huruf = "D"
else:
    huruf = "E"
print("\nNama :",nama)
print("Nilai UTS :",uts)
print("Nilai UAS :",uas)
print("Nilai Tugas :",tugas)
print("Nilai Akhir :",akhir)
print("\nNilai Huruf :",huruf)
print("Keterangan :",keterangan)
```

Untuk menentukan nilai akhir pada Python, Anda bisa menggunakan pernyataan ```return``` untuk menandai akhir fungsi atau Menggunakan fungsi ```print()``` dan menentukan nilai yang akan dikembalikan. Pernyataan ```return``` dapat mengembalikan berbagai jenis data seperti ```integer```, ```float```, ```string```, ```list```, ```dictionary```, dan fungsi lainnya.

```python
nama = input("Masukkan nama:")
uts = input("Masukkan nilai UTS:")
uas = input("Masukkan nilai UAS:")
tugas = input("Masukkan nilai Tugas:")
```
Fungsi ```input()``` adalah fungsi untuk menerima masukan dari pengguna dalam bentuk string,

```python
akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4)
```

Fungsi ```int(tugas)```, ```int(uts)```, dan ```int(uas)``` digunakan untuk mengonversi nilai input (yang masih berupa string) menjadi bilangan bulat (integer).

```python
keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0]
```
Jika nilai akhir lebih besar dari 60, maka keterangan berisi "LULUS", jika tidak, maka "TIDAK LULUS"

```python
if akhir > 80:
huruf = "A"
elif akhir > 70:
huruf = "B"
elif akhir > 50:
huruf = "C"
elif akhir > 40:
huruf = "D"
else:
huruf = "E"
```
Ini adalah Struktur Kondisi Yang Menggunakan ```If```, ```Elif```, dan ```Else```

```python
print("\nNama :",nama)
print("Nilai UTS :",uts)
print("Nilai UAS :",uas)
print("Nilai Tugas :",tugas)
print("Nilai Akhir :",akhir)
print("\nNilai Huruf :",huruf)
```

Fungsi ```Print()``` ini akan mencetak Variable-Variable program tersebut

Hasil output

![Cuplikan layar 2024-10-27 113045](https://github.com/user-attachments/assets/8b4c7595-7990-47cf-bb9b-8c6de64e12de)

# Menampilkan gaji karyawan

```python
gaji = int(input("Masukkan gaji:"))
berkeluarga = (False, True)[input("Sudah berkeluarga? (Y/T)") == "Y"]
punya_rumah = (False, True)[input("Punya rumah? (Y/T)") == "Y"]


if gaji > 3000000:
    print ("Gaji sudah diatas UMR")
    if berkeluarga:
        print ("Wajib ikutan asuransi dan menabung untuk pensiun")
    else:
        print ("Tidak perlu ikutan asuransi")
    if punya_rumah:
        print ("wajib bayar pajak rumah")

    else:
        print ("tidak wajib bayar pajak rumah")
else:
    print ("Gaji belum UMR")
```

Struktur Kondisi Ini menggunakan desision ```if```, ```elif```, dan ```else```

```python
gaji = int(input("Masukkan gaji:"))
```

Program meminta pengguna memasukkan gaji dengan fungsi ```input()```

```python
berkeluarga = (False, True)[input("Sudah berkeluarga? (Y/T)") == "Y"]
punya_rumah = (False, True)[input("Punya rumah? (Y/T)") == "Y"]
```

Inputan ini menggunakan fungsi ```string``` yang dimasukan berupa Huruf, dan ```(False, True)``` ini adalah fungsi pemilihan Y atau T, supaya tidak menggunakan ```if``` dilanjutan program tersbut

```python
if berkeluarga:
        print("Wajib ikutan asuransi dan menabung untuk pensiun")
    else:
        print("Tidak perlu ikutan asuransi")
```

Jika angka gaji lebih dari 3 juta maka Output yang akan keluar "Gaji sudah diatas UMR", dan jika tidak ```output``` yang keluar "Tidak perlu ikutan asuransi"

```python
if punya_rumah:
        print ("wajib bayar pajak rumah")

    else:
        print ("tidak wajib bayar pajak rumah")
```

Jika Memiliki rumah ```output``` yang keluar "Wajib bayar Pajak", jika tidak ```output``` yang keluar "Tidak wajib bayar pajak"

```python
else:
    print ("Gaji belum UMR")
```

Jika gaji pengguna tidak lebih dari 3 juta, program akan mencetak "Gaji belum UMR".

Hasil output

![Cuplikan layar 2024-10-27 134939](https://github.com/user-attachments/assets/af1612ef-fb07-4292-8978-4a71d6bd8861)

# Menggunakan kondisi OR dengan menginputkan 3 bilangan

```python
a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))
if a+b == c or b+c == a or c+a == b:
    print("BENAR")
else:
    print("SALAH")
```

operator OR dalam python merubah beberapa kondisi dan mengembalikan true jika salah satu benar.

```python
a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))
```

Program ini menginputkan sesuatu ```integer``` yang menggunakan variable a,b,c.

```python
if a+b == c or b+c == a or c+a == b:
    print("BENAR")
else:
    print("SALAH")
```

jika (A) ditambah (B) haslnya (C) atau bahasa pemograman itu ```OR``` ,dan apabila (B) ditambah (C) hasilnya (A),dan (C) ditambah (A) maka hasilnya (B). maka output yang keluar adalah "benar"

Hasil output

![Cuplikan layar 2024-10-27 202914](https://github.com/user-attachments/assets/64941294-426d-4999-b16e-e254cf873a00)
