
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
