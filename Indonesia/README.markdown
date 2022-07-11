# Terminal Cheatsheet untuk Mac (Dasar)

_Huruf ditampilkan dalam huruf kapital agar mudah dibaca saja._ _Capslock harus dimatikan._

### PINTASAN

| Kunci/Perintah | Deskripsi |
| ----------- | ----------- |
| Ctrl + A   | Pergi ke awal baris yang sedang Anda ketik. Ini juga berfungsi untuk sebagian besar sistem bidang input teks. Netbeans menjadi satu pengecualian |
| Ctrl + E   | Pergi ke akhir baris yang sedang Anda ketik. Ini juga berfungsi untuk sebagian besar sistem bidang input teks. Netbeans menjadi satu pengecualian |
| Ctrl + L   | Membersihkan Layar |
| Cmd + K    | Membersihkan Layar |
| Ctrl + U   | Potong semuanya mundur ke awal baris |
| Ctrl + K   | Potong semuanya ke depan hingga akhir baris |
| Ctrl + W   | Potong satu kata ke belakang menggunakan spasi sebagai pembatas |
| Ctrl + Y   | Tempel apa pun yang dipotong oleh perintah potongan terakhir |
| Ctrl + H   | Sama seperti backspace |
| Ctrl + C   | Memberhentikan apa pun yang anda jalankan. Juga menghapus semua yang ada di baris saat ini |
| Ctrl + D   | Keluar dari shell saat ini ketika tidak ada proses yang berjalan, atau kirim EOF ke proses yang sedang berjalan |
| Ctrl + Z   | Menempatkan apa pun yang Anda jalankan ke dalam proses latar belakang yang ditangguhkan. fg memulihkannya |
| Ctrl + _   | Batalkan perintah terakhir. (Garis bawah. Jadi sebenarnya Ctrl + Shift + minus) |
| Ctrl + T   | Tukar dua karakter terakhir sebelum kursor |
| Ctrl + F   | Pindahkan kursor satu karakter ke depan |
| Ctrl + B   | Pindahkan kursor satu karakter ke belakang |
| Option + →  | Pindahkan kursor satu kata ke depan |
| Option + ←  | Pindahkan kursor satu kata ke belakang |
| Esc + T  | Tukar dua kata terakhir sebelum kursor |
| Esc + Backspace | Potong satu kata ke belakang tanpa menggunakan karakter alfabet sebagai pembatas |
| Tab  | Pelengkapan otomatis file dan nama folder |

### PERINTAH INTI

| Kunci/Perintah | Deskripsi |
| ----------- | ----------- |
| cd [folder] | Ubah direktori, misalnya `cd Documents` |
| cd |  Direktori beranda |
| cd ~ |  Direktori beranda |
| cd /  | Sumber dari drive |
| cd -  | Direktori sebelumnya |
| ls | Daftar singkat |
| ls -l | Daftar panjang |
| ls -a | Daftar mencakup file yang tersembunyi |
| ls -lh| Daftar panjang dengan ukuran file yang dapat dibaca manusia |
| ls -R | Seluruh isi folder secara rekursif |
| sudo [command] | Jalankan perintah dengan hak keamanan superuser (Super User DO) |
| open [file] | Membuka file (seolah-olah anda mengklik dua kali) |
| top | Menampilkan proses aktif. Tekan q untuk keluar |
| nano [file] | Buka file menggunakan editor nano |
| vim [file] | Buka file menggunakan editor vim |
| clear |  Membersihkan layar |
| reset |  Mengatur ulang tampilan terminal |

### PERINTAH RANTAI

| Kunci/Perintah | Deskripsi |
| ----------- | ----------- |
| [command-a]; [command-b] | Jalankan perintah A dan kemudian B, terlepas dari keberhasilan A |
| [command-a] && [command-b] | Jalankan perintah B jika A berhasil |
| [command-a] \|\| [command-b] | Jalankan perintah B jika A gagal |
| [command-a] & | Jalankan perintah A di latar belakang |


### PERINTAH PIPA

| Kunci/Perintah | Deskripsi |
| ----------- | ----------- |
| [command-a] \| [command-b] | Jalankan perintah A dan kemudian berikan hasilnya ke perintah B misalnya ps auxwww \| grep google |


### RIWAYAT PERINTAH

| Kunci/Perintah | Deskripsi |
| ----------- | ----------- |
| history n |  Menunjukkan hal-hal yang diketik – tambahkan nomor untuk membatasi item n terakhir |
| Ctrl + r  | Cari secara interaktif melalui perintah yang diketik sebelumnya |
| ![value] |  Jalankan perintah terakhir yang diketik yang dimulai dengan 'value' |
| ![value]:p |  Cetak ke konsol perintah terakhir yang diketik yang dimulai dengan ‘value’ |
| !! |  Jalankan perintah terakhir yang diketik |
| !!:p |  Cetak ke konsol perintah terakhir yang diketik |

### MANAJEMEN FILE

| Kunci/Perintah | Deskripsi |
| ----------- | ----------- |
| touch [file] |   Buat file baru |
| pwd | Jalur lengkap ke direktori kerja |
| . |  Folder saat ini, misalnya `ls .` |
| .. | Direktori induk/penutup, misalnya `ls ..` |
| ls -l .. | Daftar panjang direktori induk |
| cd ../../ | Naik 2 level |
| cat | Gabungkan ke layar |
| rm [file] |  Hapus file, misalnya `rm data.tmp` |
| rm -i [file] | Hapus dengan konfirmasi |
| rm -r [dir] | Hapus direktori dan konten |
| rm -f [file] | Penghapusan paksa tanpa konfirmasi |
| cp [file] [newfile] | Salin file ke file |
| cp [file] [dir] | Salin file ke direktori |
| mv [file] [new filename] |  Pindahkan/Ganti nama, misalnya `mv file1.ad /tmp` |
| pbcopy < [file] | Salin konten file ke clipboard |
| pbpaste | Tempel konten papan klip |
| pbpaste > [file] | Tempel konten clipboard ke dalam file, `pbpaste > paste-test.txt` |

### MANAJEMEN DIREKTORI

| Kunci/Perintah | Deskripsi |
| ----------- | ----------- |
| mkdir [dir] | Buat direktori baru |
| mkdir -p [dir]/[dir] |  Buat direktori bersarang |
| rmdir [dir] | Hapus direktori ( hanya beroperasi pada direktori kosong ) |
| rm -R [dir] | Hapus direktori dan konten |
| less [file]|  Konten file keluaran dikirimkan dalam potongan ukuran layar |
| [command] > [file] |  Dorong output ke file, perlu diingat itu akan ditimpa |
| [command] >> [file] | Tambahkan output ke file yang ada |
| [command] < [file] |  Beri tahu perintah untuk membaca konten dari file |

### PENCARIAN

| Kunci/Perintah | Deskripsi |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | Cari file, misalnya `find /Users -name "file.txt"` |
| grep [search_pattern] [file] | Cari semua baris yang berisi pola, misalnya `grep "Tom" file.txt` |
| grep -r [search_pattern] [dir] | Cari secara rekursif di semua file di direktori yang ditentukan untuk semua baris yang berisi pola |
| grep -v [search_pattern] [file] | Cari semua baris yang TIDAK mengandung pola |
| grep -i [search_pattern] [file] | Cari semua baris yang berisi pola case-insensitive |
| mdfind [search_pattern] | Pencarian sorotan untuk file (nama, konten, metadata lainnya), misalnya `mdfind skateboard` |
| mdfind -onlyin [dir] -name [pattern] | Pencarian sorotan untuk file bernama seperti pola di direktori yang diberikan |

### PERTOLONGAN

| Kunci/Perintah | Deskripsi |
| ----------- | ----------- |
| [command] -h |  Menawarkan bantuan |
| [command] --help | Menawarkan bantuan |
| info [command] | Menawarkan bantuan |
| man [command] |  Tampilkan bantuan manual untuk [perintah] |
| whatis [command] | Memberikan deskripsi satu baris dari [perintah] |
| apropos [search-pattern] | Mencari perintah dengan kata kunci dalam deskripsi |