Nama: AFLAH ATHALLAH TAMAM KAPUKONG

Kelas: TI.24.A4

NIM: 312410280

Matkul: Bahasa Pemrograman

# Struktur Kondisi
Penggunaan struktur kondisi menggunakan statement `if`, Konsep pemrograman yang memungkinkan program untuk mengambil keputusan berdasarkan kondisi atau pernyataan tertentu. Struktur seleksi kondisi yang umum digunakan dalam Python

if : Digunakan untuk mengevaluasi suatu kondisi. Jika kondisi tersebut benar (True)

else : Digunakan untuk menentukan apa yang terjadi jika kondisi `if` adalah salah (False)

elif : digunakan untuk mengevaluasi beberapa kondisi. Jika kondisi `if` pertama salah, Python akan mengevaluasi kondisi `elif`. Anda bisa memiliki beberapa `elif`

# Soal latihan
![gambar](https://github.com/Abcdeflahhh/foto-flowchart/blob/a36cc708a3eaf653a49c74a464d8b0e7810fe0bc/uts.jpg)

# Program menentukan nilai akhir
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
````

Untuk menentukan nilai akhir pada Python, Anda bisa menggunakan pernyataan `return` untuk menandai akhir fungsi atau Menggunakan fungsi `print()` dan menentukan nilai yang akan dikembalikan. Pernyataan `return` dapat mengembalikan berbagai jenis data, seperti `integer`, `float`, `string`, `list`, `dictionary`, dan fungsi lainnya.

```python
nama = input("Masukkan nama:")
uts = input("Masukkan nilai UTS:")
uas = input("Masukkan nilai UAS:")
tugas = input("Masukkan nilai Tugas:")
````
Fungsi `input()` adalah fungsi untuk menerima masukan dari pengguna dalam bentuk string, 

```python
akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4)
````
Fungsi `int(tugas)`, `int(uts)`, dan `int(uas)` digunakan untuk mengonversi nilai input (yang masih berupa string) menjadi bilangan bulat (integer).

```python
keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0]
````
Jika nilai `akhir` lebih besar dari 60, maka `keterangan` berisi "LULUS", jika tidak, maka "TIDAK LULUS"

```Python
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
````

Ini adalah Struktur Kondisi Yang Menggunakan `If`, `Elif`, dan `Else`

```Python
print("\nNama :",nama)
print("Nilai UTS :",uts)
print("Nilai UAS :",uas)
print("Nilai Tugas :",tugas)
print("Nilai Akhir :",akhir)
print("\nNilai Huruf :",huruf)
print("Keterangan :",keterangan)
````

Fungsi `Print()` ini akan mencetak Variable-Variable program tersebut

Hasil output

![gambar](https://github.com/Abcdeflahhh/foto-flowchart/blob/6a5b07023b96e8b67b3eaa62138f4823f8d7c039/output%20uts.jpg)

# Program menampilkan status gaji karyawan
```Python
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
````
Struktur Kondisi Ini menggunakan desision `if, `elif`, dan `else`

```Python
gaji = int(input("Masukkan gaji:"))
````
Program meminta pengguna memasukkan gaji dengan fungsi `input()`

```Python
berkeluarga = (False, True)[input("Sudah berkeluarga? (Y/T)") == "Y"]
punya_rumah = (False, True)[input("Punya rumah? (Y/T)") == "Y"]
````
Inputan ini menggunakan fungsi `string` yang dimasukan berupa Huruf, dan `(False, True)` ini adalah fungsi pemilihan Y atau T, supaya tidak menggunakan if dilanjutan program tersbut

```Python
if berkeluarga:
        print("Wajib ikutan asuransi dan menabung untuk pensiun")
    else:
        print("Tidak perlu ikutan asuransi")
````
Jika angka gaji lebih dari 3 juta maka Output yang akan keluar "Gaji sudah diatas UMR", dan jika tidak `Output` yang keluar "Tidak perlu ikutan asuransi"

```Python
if punya_rumah:
        print ("wajib bayar pajak rumah")

    else:
        print ("tidak wajib bayar pajak rumah")
````
Jika Memiliki rumah `Output` yang keluar "Wajib bayar Pajak", jika tidak `output` yang keluar "Tidak wajib bayar pajak"

```Python
else:
    print ("Gaji belum UMR")
````
Jika gaji pengguna tidak lebih dari 3 juta, program akan mencetak "Gaji belum UMR".

Hasil output

![gambar](https://github.com/Abcdeflahhh/foto-flowchart/blob/eb66051aa9192574a8065c05581c1e46c4a1207d/gaji.jpg)

# Menggunakan kondisi or dengan menginputkan 3 bilangan
```Python
a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))

if a+b == c or b+c == a or c+a == b:
    print("BENAR")
else:
    print("SALAH")
````
Dalam Python mengevaluasi beberapa kondisi dan mengembalikan True jika salah satu kondisinya benar.

```Python
a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))
````
Program meminta pengguna untuk memasukkan tiga bilangan `(a, b, dan c)`.

```python
if a+b == c or b+c == a or c+a == b:
    print("BENAR")
else:
    print("SALAH")
````
Bagian ini memeriksa tiga kondisi menggunakan operator logika `or`, jika salah satu dari kondisi di atas terpenuhi, program akan mencetak "BENAR", 
 Jika tidak ada satu pun dari kondisi yang terpenuhi, maka blok `else` akan dijalankan, dan program akan mencetak "SALAH".

Hasil output

![gambar](https://github.com/Abcdeflahhh/foto-flowchart/blob/eb66051aa9192574a8065c05581c1e46c4a1207d/3%20bil.jpg)

# Latihan3
# Program tiket bioskop

![gambar](https://github.com/Abcdeflahhh/foto-flowchart/blob/eb66051aa9192574a8065c05581c1e46c4a1207d/soal%20bioskop.jpg)

```python
# Fungsi untuk menghitung harga tiket
def hitung_harga_tiket():
    # Harga tiket
    harga_reguler = 50000
    harga_vip = 100000
    diskon_member = 0.20  # Diskon 20%

    # Meminta input dari pengguna
    tipe_tiket = input("Masukkan tipe tiket (reguler/VIP): ").strip().lower()
    status_member = input("Apakah Anda memiliki kartu member? (ya/tidak): ").strip().lower()

    # Menentukan harga berdasarkan tipe tiket
    if tipe_tiket == "reguler":
        harga_tiket = harga_reguler
    elif tipe_tiket == "vip":
        harga_tiket = harga_vip
    else:
        print("Tipe tiket tidak valid!")
        return

    # Menghitung total harga dengan diskon jika berlaku
    if status_member == "ya":
        total_harga = harga_tiket * (1 - diskon_member)
    elif status_member == "tidak":
        total_harga = harga_tiket
    else:
        print("Status member tidak valid!")
        return

    # Menampilkan total harga
    print(f"Total harga yang harus dibayar: Rp{total_harga:.2f}")

# Memanggil fungsi
hitung_harga_tiket()
````
Program ini akan menentukan harga pesanan tiket bioskop, Yang reguler/Vip, dan jika Vip harga 100.000, dan jika reguler 80.0000, dan jika memiliki kartu member pelanggan tersebut akan mendapatkan diskon 20%

```python
harga_reguler = 50000
harga_vip = 100000
````
Untuk menentukan harga tiket tersebut

```python
tipe_tiket = input("Masukkan tipe tiket (reguler/VIP): ").strip().lower()
status_member = input("Apakah Anda memiliki kartu member? (ya/tidak): ").strip().lower()
````
Pengguna diminta untuk memasukkan tipe tiket yang mereka inginkan, bisa "reguler" atau "VIP", Pengguna juga diminta untuk menjawab apakah mereka memiliki kartu member, dengan pilihan "ya" atau "tidak"

```python
if tipe_tiket == "reguler":
    harga_tiket = harga_reguler
elif tipe_tiket == "vip":
    harga_tiket = harga_vip
else:
    print("Tipe tiket tidak valid!")
    return
````
Jika tipe tiket adalah "reguler", harga tiket akan diatur menjadi harga_reguler (Rp50.000), Jika tipe tiket adalah "VIP", harga tiket akan diatur menjadi harga_vip (Rp100.000), Jika tipe tiket yang dimasukkan tidak valid, fungsi akan menampilkan pesan error dan menghentikan proses

```python
if status_member == "ya":
    total_harga = harga_tiket * (1 - diskon_member)
elif status_member == "tidak":
    total_harga = harga_tiket
else:
    print("Status member tidak valid!")
    return
````
Jika pengguna adalah member `(status_member == "ya")`, harga tiket akan dikurangi diskon 20%, Jika pengguna bukan member `(status_member == "tidak")`, harga tiket tetap sama tanpa pengurangan, Jika input untuk status member tidak valid, misalnya selain "ya" atau "tidak", fungsi akan menampilkan pesan error dan menghentikan eksekusi

```python
print(f"Total harga yang harus dibayar: Rp{total_harga:.2f}")
hitung_harga_tiket()
````
Setelah menghitung total harga, anda dapat langsung menjalankan fungsinya

Hasil program tersebut:

![gambar](https://github.com/Abcdeflahhh/foto-flowchart/blob/eb66051aa9192574a8065c05581c1e46c4a1207d/hasil%20bioskop.jpg)

Code program tersebut:

![gambar](https://github.com/Abcdeflahhh/foto-flowchart/blob/b6408239d33252d85b2b23e4d16ef7ee162eb310/codingan%20bioskop.jpg)

Flowchart Program Tersebut:

![gambar](https://github.com/Abcdeflahhh/foto-flowchart/blob/cb3b595e12cb13ed750694c02635de6fc3f1e136/tiket%20biskop.png) 

