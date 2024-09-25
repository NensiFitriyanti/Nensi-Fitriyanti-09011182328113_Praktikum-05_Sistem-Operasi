# Nensi-Fitriyanti-09011182328113_Sistem-Operasi
Praktikum 5 Job Control
Nama : Nensi Fitriyanti
Kelas : SK3B
NIM : 09011182328113

Tugas
1. Eksekusi seluruh profile yang ada :
   a. Edit file /etc/profile dan tampilkan pesan sebagai berikut : echo "Profile dari /etc/profile"
   
   ![Screenshot from 2024-09-25 19-21-50](https://github.com/user-attachments/assets/4624eab4-01db-4f92-9c37-685329f74e61)

   ![Screenshot from 2024-09-25 19-31-38](https://github.com/user-attachments/assets/7f76ed2d-bc22-4c81-b1c3-c179a1c86274)

   b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :
   /home/stD02001/.bash_profile
   /home/stD02001/.bash_login
   /home/stD02001/.profile
   /home/stD02001/.bashrc
   Ganti nama/home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo, misalnya pada
   /home/mahasiswa/.bash_profile : echo "Profile dari .bash_profile" Lakukan hal yang sama untuk file lainnya, sesuaikan
   tampilan dengan nama file yang bersangkutan.

   /home/stD02001/.bash
   
   ![Screenshot from 2024-09-25 20-06-53](https://github.com/user-attachments/assets/39ff6d2c-559d-41ed-8dcc-ecf3cba3ba42)

   ![Screenshot from 2024-09-25 20-08-53](https://github.com/user-attachments/assets/1d84f73a-5e61-474c-b93f-adc62e851090)

**/home/. stD02001/.bash_login**

   ![Screenshot from 2024-09-25 20-12-07](https://github.com/user-attachments/assets/ed20c220-54d6-4563-a121-bf6815556c00)

   ![Screenshot from 2024-09-25 19-45-38](https://github.com/user-attachments/assets/4503f08f-62da-48d9-b133-0a22ab501cd7)

**/home/mahasiswa/.profile**

   ![Screenshot from 2024-09-25 20-14-13](https://github.com/user-attachments/assets/8750d3c0-1c3e-4538-890c-363d3afdaa48)

  ![Screenshot from 2024-09-25 20-38-13](https://github.com/user-attachments/assets/461203e1-c58c-4593-9710-bfa8c25dccb9)

**/home/mahasiswa/.bashrc** 

   ![Screenshot from 2024-09-25 20-40-05](https://github.com/user-attachments/assets/d2377855-14d1-4f5b-85f0-39e21b2560c6)

  ![Screenshot from 2024-09-25 20-49-06](https://github.com/user-attachments/assets/fdaedb1f-72a8-4d7d-a072-841cf5fa9ca5)


c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:
   **$ su mahasiswa**

**$ exit**

   ![Screenshot from 2024-09-25 20-46-16](https://github.com/user-attachments/assets/c7c9b122-b185-4050-bd9a-3065eec3d59a)

kemudian gunakan opsi – sebagai berikut :

**$ su – mahasiswa**

**$ exit**

   ![Screenshot from 2024-09-25 20-49-06](https://github.com/user-attachments/assets/fdaedb1f-72a8-4d7d-a072-841cf5fa9ca5)

Jelaskan perbedaan kedua utilitas tersebut.

= Perbedaannya adalah jika menggunakan perintah su mahasiswa, hanya identitas pengguna yang berubah sementara lingkungan (environment) dari pengguna sebelumnya tetap dipertahankan. Sebaliknya, perintah su - mahasiswa melakukan login baru sepenuhnya, termasuk memuat ulang seluruh lingkungan pengguna baru dari awal.

## **2. Prompt String (PS)**

a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan
parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell
PS1=‟> „
export PS1

![Screenshot from 2024-09-25 21-23-47](https://github.com/user-attachments/assets/5b04eff9-07c8-47f7-905b-f36546b69136)

![Screenshot from 2024-09-25 21-24-56](https://github.com/user-attachments/assets/62dee570-6ab0-407f-9232-0eea6801a414)

b. Eksperimen hasil PS1 :
$ PS1=“\! > “
69 > PS1=”\d > “
Mon Sep 23 > PS1=”\t > “
10:10:20 > PS1=”Saya=\u > “
Saya=mahasiswa > PS1=”\w >”
~ > PS1=\h >”

![Screenshot from 2024-09-25 21-29-00](https://github.com/user-attachments/assets/6e7fbc87-2f91-4086-95f1-6e7ea5556958)

## **3. Logout**

Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout
Echo “Terima kasih atas sesi yang diberikan”
Sleep 5
clear

![Screenshot from 2024-09-25 21-52-02](https://github.com/user-attachments/assets/e6b48bc7-d547-4aee-a294-0d2105dd24e9)

![Screenshot from 2024-09-25 21-51-16](https://github.com/user-attachments/assets/b7261106-9d32-4751-a698-fe5178acc36b)

## **4. Bash script*
a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :

**p1.sh**

#! /bin/bash

echo “Program p1”

ls –l

![Screenshot from 2024-09-25 21-52-47](https://github.com/user-attachments/assets/7c5963ca-5141-430d-b168-d9961c904f96)

![Screenshot from 2024-09-25 21-54-03](https://github.com/user-attachments/assets/3140fecf-6deb-4552-811c-5d2a9c891b78)

**p2.sh**

#! /bin/bash

echo “Program p2”

who

![Screenshot from 2024-09-25 21-56-23](https://github.com/user-attachments/assets/47311091-e40b-4e8a-8350-b21af517ba9a)

![Screenshot from 2024-09-25 21-57-13](https://github.com/user-attachments/assets/8c3d6507-505b-4afe-b3e2-d240d1986e68)

**p3.sh**

#! /bin/bash

echo “Program p3”

ps x

![Screenshot from 2024-09-25 21-57-32](https://github.com/user-attachments/assets/66aa2b51-a3be-4f0c-b957-cf0a09a0c7f4)

![Screenshot from 2024-09-25 21-58-21](https://github.com/user-attachments/assets/17eece15-caff-4c30-84cd-c4e8b332ae0a)

b. Jalankan script tersebut sebagai berikut :
**$ ./p1.sh ; ./p3.sh ; ./p2.sh**

![Screenshot from 2024-09-25 22-13-33](https://github.com/user-attachments/assets/4510e724-abba-43d3-9bf2-0526c2d2f305)

![Screenshot from 2024-09-25 22-13-53](https://github.com/user-attachments/assets/ed24883e-3187-4bf5-86da-98e667047ff0)

![Screenshot from 2024-09-25 22-14-08](https://github.com/user-attachments/assets/ccc3cd9d-311a-4d54-9655-2bcb4af44d7e)

**$ ./p1.sh &**

![Screenshot from 2024-09-25 22-15-25](https://github.com/user-attachments/assets/9133ad7e-7a04-40a6-803d-166297d54dea)

**$ ./p1.sh $ ./p2.sh & ./p3.sh &**

![Screenshot from 2024-09-25 22-22-21](https://github.com/user-attachments/assets/ccd3cfc6-82e7-4f0c-b329-d1a74672d95f)

**$ ( ./p1.sh ; ./p3.sh ) &**

![Screenshot from 2024-09-25 22-25-37](https://github.com/user-attachments/assets/bdbb2cfb-9227-4289-b98a-74f508ff5540)

## **5. Jobs**

**a.** Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.

#!/bin/bash
while [ true ]

do

date >> hasil

sleep 10

done

![Screenshot from 2024-09-25 22-32-54](https://github.com/user-attachments/assets/44fcec45-1dda-481d-ad89-6c0248fd8e3f)

![Screenshot from 2024-09-25 22-32-34](https://github.com/user-attachments/assets/003e55b2-1150-4fdb-ae6d-8ee6d1e72ca9)

**b.** Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :

$ jobs

$ find / -print > files 2>/dev/null &

$ jobs

**c.** Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background

$ fg %1

$ bg

![Screenshot from 2024-09-25 22-37-57](https://github.com/user-attachments/assets/69518561-ab67-4328-a016-f298c0641150)

**d.** Stop program background dengan utilitas kil

$ ps x

$ kill [Nomor PID]

![Screenshot from 2024-09-25 22-39-32](https://github.com/user-attachments/assets/046b1c6b-badb-491d-8aab-4b2ad674b9d7)

![Screenshot from 2024-09-25 22-48-07](https://github.com/user-attachments/assets/21e28cf4-fc9a-421e-9160-79fd5f5cf838)

## **6. History**

**a.** Ganti nilai HISTSIZE dari 1000 menjadi 20

$ HISTSIZE=20

$ h

![Screenshot from 2024-09-25 23-00-27](https://github.com/user-attachments/assets/ab959f04-654a-4a83-899f-0ce464b7751e)

**b.** Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan

$ !-5

![Screenshot from 2024-09-25 23-01-26](https://github.com/user-attachments/assets/a5efe427-b293-4cca-873a-43d06730d18a)

**c.** Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer

$ !!

![Screenshot from 2024-09-25 23-01-42](https://github.com/user-attachments/assets/2d4a985c-dd30-4975-b383-e1ba39fb6ca3)

**d.** Ulangi instruksi pada history bufer nomor 150

$ !150

![Screenshot from 2024-09-25 23-03-06](https://github.com/user-attachments/assets/7b75f28b-a55d-40a4-823d-ff533dd4e72a)

**e.** Ulangi instruksi dengan prefix “ls”

$ !ls

![Screenshot from 2024-09-25 23-06-36](https://github.com/user-attachments/assets/773e266a-9ed3-4026-93c1-81446be7e4e1)
