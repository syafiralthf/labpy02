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
