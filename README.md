# Praktikum Modul 1 Jaringan Komputer
## Nama kelompok:<br/>
1. Lia Kharisma Putri (5025201034)<br/>
2. Azzura Ferliani Ramadhani (5025201190)<br/>
3. Ingwer Ludwig Nommensen (5025201259)<br/>

## Nomor 1
1. Pilih jaringan (wifi apabila pakai wifi)
2. Di wireshark, lakukan filter dengan command http
3. Pilih salah satu packet, kemudian klik kanan, lalu follow TCP Stream
4. Liat di hasilnya, find kata “server”, jawabannya Server: nginx/1.10.3
5. Hasil:![Dokumentasi soal nomor 1](./dokumentasi/1.png)
## Nomor 2
1. Buka file `soal1-2.pcapng`
2. Cari yang info nya ada alamat “detail topik” dengan command `http contains "detail"`
3. Pilih filename 194 dan save
4. Export object as HTTP dan buka di tempat eksport
5. Jawabannya Evaluasi unjuk kerja User Space Filesystem (FUSE)
6. Hasil:![Dokumentasi soal nomor 2](./dokumentasi/2.png)
## Nomor 3
1. Buka soal `soal3-6.pcapng`
2. Terapkan display filter `tcp.dstport == 80`
3. Hasil: ![Dokumentasi soal nomor 3](./dokumentasi/3.png)
## Nomor 4
1. Buka soal `soal3-6.pcapng`
2. Terapkan display filter `tcp.srcport == 21`
3. Hasil:![Dokumentasi soal nomor 4](./dokumentasi/4.png)
## Nomor 5
1. Buka soal `soal3-6.pcapng`
2. Terapkan display filter `tcp.srcport == 443`
3. Hasil:![Dokumentasi soal nomor 5](./dokumentasi/5.png)
## Nomor 6
1. Buka soal `soal3-6.pcapng`
2. Dikarenakan ip dari lipi.go.id belum diketahui, maka cek terlebih dahulu menggunakan filter `http contains lipi.go.id`
![Pencarian IP lipi.go.id](./dokumentasi/6.1.png)
3. Diketahui ip dari lipi.go.id adalah `203.160.128.158`
4. Terapkan display filter `ip.dst == 203.160.128.158`
5. Hasil:![Dokumentasi soal nomor 6](./dokumentasi/6.2.png)
# Nomor 7
1. Pilih jaringan (wifi apabila pakai wifi)
2. Lakukan ping menggunakan cmd dengan command “ipconfig” untuk mengetahui ip kita
3. Masukkan filter pada wireshark dengan command “ip.src == <ip yang digunakan>” `ip.src==10.8.108.197`
7. Hasil:![Dokumentasi soal nomor 7](./dokumentasi/7.png)
# Nomor 8
1. Buka file `soal8-10.pcapng`
2. Lakukan filter dengan `tcp contains "password"` untuk memfilter konten sensitif seperti password misalnya
3. Lakukan follow tcp stream terhadap paket yang telah ditemukan
4. Hasil:![image](https://user-images.githubusercontent.com/54592376/192100731-70c8e3c4-9dad-4cd9-a28d-b0376258d3f1.png)
# Nomor 9
1. Cari salt yang dimaksud dalam percakapan indikasi kecurangan (ditemukan di stream 29)
2. View as RAW agar bisa di decrypt
3. Save file yang diinginkan dengan format `E09.des3`
4. Hasil:![image](https://user-images.githubusercontent.com/54592376/192100962-640bca44-1a85-4ea6-8692-79f574ff56e4.png)
# Nomor 10
1. Lakukan decrypt sesuai dengan petunjuk indikasi kecurangan
2. Buka terminal dan change directory ke tempat file tersbeut disimpan
3. Ketik command `openssl des3 -d -salt -in E09.des3 -out flag.txt`
4. Dari petunjuk kecurangan yang didapat, masukkan "nakano" (tanpa kutip) sebagai password untuk mendecrypt file
5. Cek File `flag.txt` untuk melihat hasilnya

Hasil Decrypt : JaRkOm2022{8uK4N_CtF_k0k_h3h3h3}
6. Hasil:![image](https://user-images.githubusercontent.com/54592376/192101149-e2e4ac5c-0120-45f0-bfdc-6cd2f71b9742.png)
