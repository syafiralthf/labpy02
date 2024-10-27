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

# LATIHAN 3

# Pemesanan Tiket Bioskop

Kasus 1: Program Pemesanan Tiket Bioskop Buat program yang menghitung harga tiket bioskop. Tiket reguler berharga Rp50.000, sedangkan tiket VIP berharga Rp100.000. Jika user memiliki kartu member, mereka mendapatkan diskon 20% dari harga tiket. Program ini harus meminta tipe tiket dan status member dari user, lalu menghitung total harga yang harus dibayar.

Petunjuk:

```Gunakan if else dan operator ternary.```

```python
harga_reguler = 50000
harga_vip = 100000

tipe_tiket = (input("Masukkan tipe tiket (reguler/VIP): "))
status_member = (input("Apakah Anda memiliki kartu member? (ya/tidak): "))

 Menghitung total harga
if tipe_tiket == "reguler":
    total_harga = harga_reguler
elif tipe_tiket == "vip":
    total_harga = harga_vip
else:
    print("Tipe tiket tidak valid.")
    exit()

 Menghitung diskon jika pengguna memiliki kartu member


if status_member == "ya":
        total_harga *= 0.8  # Diskon 20%
    
        print(f"Total harga yang harus dibayar: Rp{total_harga:.2f}")
elif status_member == "tidak":
            total_harga
            print(f"total harga yang harua dibayar: Rp{total_harga:.2f}")
else:
    print("Harga tidak dapat dihitung.")
```

Program ini akan menentukan harga pesanan tiket bioskop, Yang reguler/Vip, dan jika Vip harga 100.000, dan jika reguler 80.0000, dan jika memiliki kartu member pelanggan tersebut akan mendapatkan diskon 20%

```python
harga_reguler = 50000
harga_vip = 100000
```

variable ini menentukan harga tiket bioskop

```python
tipe_tiket = (input("Masukkan tipe tiket (reguler/VIP): "))
status_member = (input("Apakah Anda memiliki kartu member? (ya/tidak): "))
```

memasukan inputan sesuai Output Program (Reguler/Vip) di variable (Tipe_Tiket), dan Memasukan inputan yang output tersebut Bertanya memiliki kartu member atau tidak.

```python
if tipe_tiket == "reguler":
    total_harga = harga_reguler
elif tipe_tiket == "vip":
    total_harga = harga_vip
else:
    print("Tipe tiket tidak valid.")
    exit()
```

Jika tipe tiket reguler total harga proses ke Harga reguler, dan jika tiket vip Total harga proses keharga vip dan jika Selain memasukan inputan reguler/vip Output yang keluar "Tipe tiket tidak valid" dan berproses ke fungsi ```exit()``` yang artinya program dihentikan.

```python
if status_member == "ya":
        total_harga *= 0.8  # Diskon 20%
    
        print(f"Total harga yang harus dibayar: Rp{total_harga:.2f}")
elif status_member == "tidak":
            total_harga
            print(f"total harga yang harua dibayar: Rp{total_harga:.2f}")
else:
    print("Harga tidak dapat dihitung.")
```

desision ini menentukan mempunyai kartu member atau tidak, Jika Inputan status member menjawab "ya", maka total harga akan di kalikan dengan operator * 0,8 yang disebut diskon 20% dan jika inputan status member "tidak", maka total harga normal jika menginputkan selain (ya/tidak) output yang keluar "Harga tidak dapat dihitung"

Hasil Output

![Cuplikan layar 2024-10-27 211059](https://github.com/user-attachments/assets/fbf2547d-9e55-4ebe-8cdd-10847f2eec18)

Code dari program tersebut

![Cuplikan layar 2024-10-27 211227](https://github.com/user-attachments/assets/47095464-b783-4565-9c86-3c41cc6bbdbe)

Berikut flowchartnya

![WhatsApp Image 2024-10-27 at 14 55 29](https://github.com/user-attachments/assets/105563d6-7147-402d-b8e2-bfbe53da8199)


# Kalkulator sedehana

Buat program kalkulator yang menerima dua angka dan satu operator aritmatika dari pengguna (penjumlahan, pengurangan, perkalian, atau pembagian). Program akan menghitung hasil sesuai dengan operator yang dipilih.

```python
# Fungsi untuk kalkulator sederhana
def kalkulator():
    # Meminta input dari pengguna
    angka1 = float(input("Masukkan angka pertama: "))
    angka2 = float(input("Masukkan angka kedua: "))
    operator = input("Masukkan operator (+, -, *, /): ").strip()

    # Menghitung hasil berdasarkan operator yang dipilih
    if operator == "+":
        hasil = angka1 + angka2
    elif operator == "-":
        hasil = angka1 - angka2
    elif operator == "*":
        hasil = angka1 * angka2
    elif operator == "/":
        if angka2 != 0:
            hasil = angka1 / angka2
        else:
            print("Error: Pembagian dengan nol tidak diperbolehkan!")
            return
    else:
        print("Error: Operator tidak valid!")
        return

    # Menampilkan hasil
    print(f"Hasil: {hasil}")

# Memanggil fungsi
kalkulator()
```

Program kalkulator sederhana dalam Python adalah proyek yang baik untuk pemula dan programmer tingkat lanjut. Program ini memungkinkan pengguna untuk melakukan operasi matematika seperti penjumlahan, pengurangan, perkalian, dan pembagian.

```python
angka1 = float(input("Masukkan angka pertama: "))
angka2 = float(input("Masukkan angka kedua: "))
operator = input("Masukkan operator (+, -, *, /): ").strip()
```

Pengguna diminta memasukkan angka pertama dan angka kedua, yang kemudian dikonversi menjadi tipe float agar bisa menerima bilangan desimal, Pengguna diminta memasukkan operator aritmatika, yaitu salah satu dari + (penjumlahan), - (pengurangan), * (perkalian), atau / (pembagian). Fungsi strip() digunakan untuk menghapus spasi yang mungkin tidak sengaja dimasukkan.

```python
if operator == "+":
    hasil = angka1 + angka2
elif operator == "-":
    hasil = angka1 - angka2
elif operator == "*":
    hasil = angka1 * angka2
elif operator == "/":
    if angka2 != 0:
        hasil = angka1 / angka2
    else:
        print("Error: Pembagian dengan nol tidak diperbolehkan!")
        return
```

Jika operator adalah ```+```, maka fungsi akan menjumlahkan kedua angka ```(angka1 + angka2)```, Jika operator adalah ```-```, maka fungsi akan mengurangi angka pertama dengan angka kedua ```(angka1 - angka2)```, Jika operator adalah ```*```, maka fungsi akan mengalikan angka pertama dengan angka kedua ```(angka1 * angka2)```, Jika operator adalah ```/```, maka fungsi akan membagi angka pertama dengan angka kedua ```(angka1 / angka2)```. Namun, sebelum melakukan pembagian, fungsi memastikan bahwa angka kedua ```(angka2)``` tidak bernilai nol, karena pembagian dengan nol tidak valid dan akan menyebabkan error.

```python
else:
    print("Error: Operator tidak valid!")
    return
print(f"Hasil: {hasil}")
kalkulator()
```

Jika pengguna memasukkan operator yang tidak dikenali (bukan +, -, *, atau /), Setelah operasi berhasil dijalankan, hasil perhitungan akan ditampilkan kepada pengguna

Hasil program tersebut:

![Cuplikan layar 2024-10-27 213620](https://github.com/user-attachments/assets/4ede9a88-fb65-495e-b125-15dd6f8c267b)

Code program tersebut

![Cuplikan layar 2024-10-27 213646](https://github.com/user-attachments/assets/eef59b67-da76-448e-aa0b-f4a84306fb60)

Flowchartnya

![flowchart labpy02_page-0001](https://github.com/user-attachments/assets/1db6dcae-1f27-4f86-87f3-2f5233e88ea7)
