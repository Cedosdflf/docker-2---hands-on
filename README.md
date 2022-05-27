# docker-2---hands-on
Nama : Beni cahyadi
NIM : 119140195

**Program game alien**

**Deskripsi program.**
Program game aliens adalah program game bahasa python. game ini berupa pesawat luar angkasa yang melakukan tembak menembak dengan pesawat asing( pesawat alien).
setiap pesawat luar angkasa berhasil menembak pesawat alien maka player akan mendapatkan poin. jika pesawat alien berhasil menembak atau menabrakan diri ke pesawat luar angkasa, maka nyawa player akan berkurang satu. permainan akan berakhir jika nyawa player telah habis. 

**cara menjalankan container**
1. cari dan download file extract game alien di github. lalu, buka file-file program game aliens itu di visual studio code.
2. buat file bernama "Dockerfile" di visual studio code. letakan file ini dalam satu folder file-file game aliens. 
3. file "Dockerfile" berisikan tulisan sebagai berikut : 

FROM python:3

WORKDIR /examples

COPY ./examples .

CMD ["python", "./aliens.py"]

4. setelah itu, lakukan build image. cara membuild image yaitu klik kanan pada file "Dockerfile". lalu, pilih build image. setelah itu, tulis nama docker container sesuai keinginan anda. kemudian klik enter. selanjutnya, proses building image akan berjalan. tunggu hingga selesai.
5. tahapan selanjutnya yaitu menjalankan docker container. untuk menjalankan docker container anda dapat melakukan dengan cara menulis "docker run <nama_container_anda>" pada jendela terminal di visual studio code.
6. pada percobaan ini file game aliens tidak dapat dijalankan. terdapat eror yang bertuliskan "pygame.eror: vidio system not initialized". untuk permasalan ini saya masih belum mendapat solusi. bagi yang memiliki solusi untuk permasalah ini bisa komen pada kolom komentar.
7. anda dapat menjalankan game aliens ini langsung di visual studio code tanpa melalui docker container. caranya, buka file game aliens.py dan klik tombol play maka game alien akan berjalan.

[![berikut ini adalah link youtube percobaan menjalankan program game alien menggunakan docker](https://youtu.be/Q-TZH3ob2TU)]https://youtu.be/Q-TZH3ob2TU

sekian dan terimakasih. semoga hari mu menyenangkan :)
