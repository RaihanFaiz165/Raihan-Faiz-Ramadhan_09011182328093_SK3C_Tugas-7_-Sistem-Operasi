## Tugas 6 Sistem Operasi

Nama: Raihan Faiz Ramadhan

NIM: 09011182328093

Kelas: SK3C

MK: Sistem Operasi (Praktikum)

# Praktikum SSH (Secure Shell)
Pada praktikum ini,kita akan mencoba untuk menghubungkan virtual machine pada perangkat kita ke virtual machine pada perangkat lain

1.  Sebelum melakukan percobaan,kita gunakan perintah “sudo apt update && upgrade”,perintah ini berfungsi untuk memperbarui paket agar paket dari repositori berada di versi terbaru.
Setelah itu gunakan perintah “sudo apt install openssh-server”,perintah ini berfungsi untuk mengunduh paket openssh-server karena secara default paket ini belum diunduh,paket ini dibutuhkan untuk meremote virtual machine pada perangkat lain. 
![1](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-7_-Sistem-Operasi/blob/main/Sistem%20operasi%20tugas%207/7.1.png)

2. Setelah itu jalankan perintah “sudo systemctl enable ssh”,perintah tersebut berfungsi untuk mengaktifkan layanan ssh dan perintah “sudo systemctl status ssh” berfungsi untuk menampilkan status aktif atau tidak layanan ssh. Output “active [running]” menandakan ssh sedang dijalankan 
![2](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-7_-Sistem-Operasi/blob/main/Sistem%20operasi%20tugas%207/7.2.png)

3. Sebelum kita mencoba masuk ke virtual machine pada perangkat lain, kita ganti konfigurasi jaringan pada perangkat kita menjadi bridged adapter. Bridged adapter berfungsi untuk menghubungkan virtual machine ke jaringan fisik host. Lakukan hal yang sama pada perangkat yang akan kita uji coba dan pastikan kedua perangkat terhubung ke jaringan yang sama.
![3](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-7_-Sistem-Operasi/blob/main/Sistem%20operasi%20tugas%207/7.3.png)

4. Cek ip address pada perangkat lain menggunakan perintah “ip addr show”
![4](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-7_-Sistem-Operasi/blob/main/Sistem%20operasi%20tugas%207/7.4.png)

5. Gunakan perintah ssh untuk meremote dan tambahkan username beserta ip address dari perangkat yang dituju,namun sebelum kita berhasil menghubungkan ke virtual machine pada perangkat yang dituju kita perlu memasukkan kata sandi dari perangkat tersebut.
![5](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-7_-Sistem-Operasi/blob/main/Sistem%20operasi%20tugas%207/7.5.png)
6. Setelah berhasil login kita coba untuk menjalankan perintah “neofetch” yang akan menampilkan informasi.Sebelumnya saya telah mengunduh paket neofetch sehingga saya dapat menggunakan perintah tersebut.
![6](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-7_-Sistem-Operasi/blob/main/Sistem%20operasi%20tugas%207/7.6.png)

7. Setelah berhasil login dan menjalankan perintah menggunakan di perangkat lain,kita dapat menggunakan perintah “exit” untuk logout dari perangkat tersebut.
![7](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-7_-Sistem-Operasi/blob/main/Sistem%20operasi%20tugas%207/7.7.png)

8. Berhasil logout dari perangkat yang sebelumnya diremote.
![8](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-7_-Sistem-Operasi/blob/main/Sistem%20operasi%20tugas%207/7.8.png)

