# Biodata

Nama = Syafira Luthfi

Kelas = TI.24.A.4

NIM = 321410353

# Struktur Kondisi
Penggunaan struktur kondisi menggunakan statement if, Konsep pemrograman yang memungkinkan program untuk mengambil keputusan berdasarkan kondisi atau pernyataan tertentu. Struktur seleksi kondisi yang umum digunakan dalam Python

if : Digunakan untuk mengevaluasi suatu kondisi. Jika kondisi tersebut benar (True)

else : Digunakan untuk menentukan apa yang terjadi jika kondisi if adalah salah (False)

elif : digunakan untuk mengevaluasi beberapa kondisi. Jika kondisi if pertama salah, Python akan mengevaluasi kondisi elif. Anda bisa memiliki beberapa elif

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
