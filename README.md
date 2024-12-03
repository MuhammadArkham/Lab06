
## PRAKTIKUM 6

NAMA : Muhammad Arkhamullah Rifai Asshidiq

Mata kuliah : Bahasa pemrograman

NIM : 312410545
## Tugas Praktikum 6
```python
daftar_mahasiswa = []

def tambah():
    nama = input("Masukkan nama mahasiswa: ")
    daftar_mahasiswa.append(nama)
    print(f"{nama} berhasil ditambahkan.")

def tampilkan():
    if not daftar_mahasiswa:
        print("Tidak ada data mahasiswa.")
    else:
        print("Daftar Mahasiswa:")
        for nama in daftar_mahasiswa:
            print(nama)

def hapus(nama):
    if nama in daftar_mahasiswa:
        daftar_mahasiswa.remove(nama)
        print(f"{nama} berhasil dihapus.")
    else:
        print(f"{nama} tidak ditemukan.")

def ubah(nama):
    if nama in daftar_mahasiswa:
        index = daftar_mahasiswa.index(nama)
        nama_baru = input("Masukkan nama baru: ")
        daftar_mahasiswa[index] = nama_baru
        print("Data berhasil diubah.")
    else:
        print(f"{nama} tidak ditemukan.")

def main():
    while True:
        print("\nMenu:")
        print("1. Tambah Data")
        print("2. Tampilkan Data")
        print("3. Hapus Data")
        print("4. Ubah Data")
        print("5. Keluar")

        pilihan = input("Masukkan pilihan (1-5): ")

        if pilihan == '1':
            tambah()
        elif pilihan == '2':
            tampilkan()
        elif pilihan == '3':
            nama = input("Masukkan nama mahasiswa yang akan dihapus: ")
            hapus(nama)
        elif pilihan == '4':
            nama = input("Masukkan nama mahasiswa yang akan diubah: ")
            ubah(nama)
        elif pilihan == '5':
            print("Terima kasih!")
            break
        else:
            print("Pilihan tidak valid. Silakan coba lagi.")

if __name__ == "__main__":
    main()
```
## Hasil kode Program
![Foto](https://github.com/MuhammadArkham/Lab06/blob/main/Screenshot%202024-12-03%20124748.png?raw=true)
![Foto](https://github.com/MuhammadArkham/Lab06/blob/main/Screenshot%202024-12-03%20124757.png?raw=true)

## Penjelasan alur algoritma program
```python
daftar_mahasiswa
```
Untuk membuat list kosong bernama yang akan menampung nama-nama mahasiswa.
```python
Fungsi tambah()
```
 bertugas menambahkan nama baru ke dalam daftar. Pengguna akan diminta untuk menginput nama mahasiswa, dan setelah nama tersebut dimasukkan, program akan menyimpan nama itu ke dalam daftar serta menampilkan pesan sebagai konfirmasi.
```python
Fungsi tampilkan()
```
 bertujuan untuk menampilkan semua nama mahasiswa yang sudah disimpan. Apabila daftar masih kosong, program akan memberikan informasi khusus kepada user bahwa belum ada data yang tersimpan.
```python
Fungsi hapus()
```
 memberikan kemampuan kepada pengguna untuk menghapus nama tertentu dari daftar. Sebelum nama dihapus, program akan memeriksa apakah nama tersebut benar-benar ada dalam daftar untuk menghindari kesalahan.
```python
fungsi ubah()
```
memungkinkan pengguna mengganti nama mahasiswa yang sudah ada. Program akan mencari nama lama yang dimaksud dalam daftar, lalu menggantinya dengan nama baru yang diinputkan pengguna.
```python
fungsi main()
```
Seluruh proses ini dikendalikan oleh fungsi main(), yang menampilkan menu interaktif berisi pilihan untuk menambah, menampilkan, menghapus, mengubah data, atau keluar dari program. user dapat memilih opsi yang sesuai, dan program akan menjalankan fungsi yang relevan.

Program ini menggunakan mekanisme while True untuk memastikan bahwa aplikasi tetap berjalan hingga user memilih opsi keluar. Dengan demikian, aplikasi ini dirancang untuk memberikan pengalaman pengelolaan data mahasiswa yang sederhana tetapi tetap efektif dan mudah digunakan.

## Gambar Flowchart
![Foto]
