# Praktikum Modul 1 Jaringan Komputer
## Nama kelompok:<br/>
1. Lia Kharisma Putri (5025201034)<br/>
2. Azzura Ferliani Ramadhani (5025201190)<br/>
3. Ingwer Ludwig Nommensen (5025201259)<br/>

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
