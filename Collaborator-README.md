## Panduan untuk Kolaborator

Untuk memudahkan proses kolaborasi, silakan ikuti langkah berikut:<br>
1. Buat akun Github
2. Sertakan username Github Anda ke [Thread Official AMQ Lokalisasi Bahasa Indonesia](https://discord.com/channels/386089398975856641/1431027276648153098)
3. Download Visual Studio Code dari [sini](https://code.visualstudio.com/download)
4. Download Git dari [link berikut](https://git-scm.com/install/)
5. Buka VSCode
6. Buka folder/directory dimana Anda ingin meletakkan folder repository Github amq-localization-indonesian. (If you're lazy like me, feel free to put it on your Desktop)
7. Buka Tab View → Terminal seperti contoh dibawah
   <img width="708" height="731" alt="image" src="https://github.com/user-attachments/assets/7700c23e-a0a8-4dec-b4c6-cad9c4d365a2" />
8. Gunakan command berikut
   ```git clone https://github.com/ChrisLefko/amq-localization-indonesian.git```
9. Lalu gunakan command
    ```cd amq-localization-indonesian```
   untuk mengarahkan Terminal ke folder repositori
10. Anda dapat mengedit file ``id.json`` untuk keperluan translasi berdasarkan diskusi pada [Thread Official AMQ Lokalisasi Bahasa Indonesia](https://discord.com/channels/386089398975856641/1431027276648153098)
11. Setelah selesai mengedit, jangan lupa untuk menyimpan perubahan menggunakan ``Ctrl + S`` atau ``⌘ + S``
12. Buka kembali Terminal pada VSCode
13. Gunakan command ```git status``` untuk mengecek perubahan lokal apa saja yang perlu di-push ke server
14. Selanjutnya, gunakan command ```git checkout -b review``` untuk memastikan Anda berada dalam branch ``review``
15. Setelah itu, gunakan command ```git add id.json``` untuk menambahkan file ``id.json`` sebagai bagian dari perubahan yang akan di-push ke Github nantinya
16. Lalu, gunakan command ```git commit -m "Revised the most recent translation file from Chris"``` dan ceritakan perubahan apa yang telah Anda lakukan didalam tanda kutip seperti contoh
17. Kita bisa menggunakan command ```git push origin review``` untuk meng-push update yang kita lakukan ke Github untuk di-review oleh kawan-kawan tim translasi yang lain
18. Setelahnya, kunjungi laman [Pull Request](https://github.com/ChrisLefko/amq-localization-indonesian/pulls)
19. Klik tombol hijau "Create Pull Request"
20. Klik branch review
21. Buat Pull Request
22. Ketika Pull Request sudah dibuat, Anda dapat mengabari kolaborator lain di [Thread Official AMQ Lokalisasi Bahasa Indonesia](https://discord.com/channels/386089398975856641/1431027276648153098) untuk di-review bersama
23. Setelah proses review selesai, hasil TL Anda akan di-merge ke branch utama (main) untuk diserahkan ke Egerod

## Panduan Menerjemahkan Variabel TL Baru dari Egerod

1. Ikuti langkah 1-9 dari tutorial diatas
2. Download Template terbaru dari Egerod. Biasanya dikirim oleh Egerod sendiri ke [Thread Official AMQ Lokalisasi Bahasa Indonesia](https://discord.com/channels/386089398975856641/1431027276648153098) seperti contoh dibawah
   <img width="622" height="303" alt="image" src="https://github.com/user-attachments/assets/2957d530-5401-478f-812d-adb3008d3a47" />
3. Download file id.json dari Egerod, lalu paste ke folder/direktori amq-localization-indonesian di mesin lokal Anda
4. Paste dan Replace id.json sebelumnya
5. Buka VSCode
6. Buka Terminal
7. Gunakan command ```git branch``` untuk memastikan Anda berada pada branch ``review``
8. Selanjutnya, gunakan command ```git add id.json``` supaya template baru Egerod yang telah di-paste ke direktori lokal Anda bisa ikut terbawa ke repositori Github ini
9. Lalu, jalankan command ```git commit -m "Updated the April Fools 2026 Template by Egerod"``` kalimat setelah -m bisa diganti dengan topik update (misal: Update Lore Nexus untuk Karakter x atau Menu untuk mode baru NGMC)
10. Setelah itu, kita bisa menggunakan command ```git push origin review``` untuk "mendorong" template dari mesin lokal Anda ke repositori ini
11. Ketika git push berhasil dilakukan, buat pull request pada branch review (biasanya GitHub akan merekomendasikan Anda untuk membuat Pull Request setelah Anda berhasil melakukan proses git push, Anda bisa mengikuti guide tersebut yang biasa terletak di bagian atas laman)
12. Mention @ChrisLefko (John Pepper) atau @rafaelm64 (Rafa-kun) di [Thread Official AMQ Lokalisasi Bahasa Indonesia](https://discord.com/channels/386089398975856641/1431027276648153098) karena GitHub membutuhkan setidaknya 1 orang untuk me-review setiap git push yang dilakukan oleh kolaborator
13. Setelah pull request di-review, Anda bisa mulai mengerjakan proses translasi/terjemahan pada template yang baru Anda push ke GitHub
14. Anda bisa mengerjakan dengan membuka VSCode, File → Open Folder → Cari folder/direktori amq-localization-indonesian di mesin Anda
15. Selanjutnya, Anda dapat menggunakan shortcut ``Ctrl + F`` atau ``⌘ + F`` dan cari kata kunci ```MISSING-```
16. Variabel baru yang belum diterjemahkan akan berada di baris yang sama dengan kata kunci MISSING- (mis: MISSING-title: "Tiny Video")
17. Terjemahkan variabel yang masih terlihat dalam Bahasa Inggris seperti yang terdapat pada contoh di langkah 16
18. Hasil terjemahan akan menjadi seperti ini (MISSING-title: "Video Kecil")
19. Lalu, hapus kata kunci ``MISSING-`` (jangan lupa tanda "-") dari variabel. Hasil akhir akan menjadi seperti ini (title: "Video Kecil")
20. Lakukan langkah 15-19 hingga ``Ctrl + F`` atau ``⌘ + F`` tidak dapat menemukan kata kunci MISSING- dalam script
21. Selanjutnya, lakukan langkah 7-12 dengan pesan commit yang berbeda (mis: "Translated the April Fools 2026 Template")
22. Setelah pull request di-review dan di-merge ke branch utama, Anda bisa menggunakan link berikut ```https://raw.githubusercontent.com/ChrisLefko/amq-localization-indonesian/refs/heads/main/id.json``` untuk menyerahkan file json terjemahan terbaru ke Egerod

