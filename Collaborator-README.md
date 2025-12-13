## Tutorial untuk Kolaborator

Untuk memudahkan proses kolaborasi, silakan ikuti langkah berikut:<br>
1. Buat akun Github
2. Sertakan username Github Anda ke [Thread Official AMQ Lokalisasi Bahasa Indonesia](https://discord.com/channels/386089398975856641/1431027276648153098)
3. Download Visual Studio Code dari [sini](https://code.visualstudio.com/download)
4. Download Git dari [link berikut](https://git-scm.com/install/)
5. Buka VSCode
6. Buka folder/directory dimana Anda ingin meletakkan folder repository Github amq-localization-indonesian. (If you're lazy like me, feel free to put it in your Desktop)
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
14. Gunakan command ```git checkout review``` untuk memastikan Anda berada dalam branch ``review``
15. Gunakan command ```git add id.json``` untuk menambahkan file ``id.json`` sebagai bagian dari perubahan yang akan di-push ke Github nantinya
16. Lalu gunakan command ```git commit -m "Revised the most recent translation file from Chris"``` dan ceritakan perubahan apa yang telah Anda lakukan didalam tanda kutip seperti contoh
17. Terakhir, kita bisa menggunakan command ```git push origin review``` untuk meng-push update yang kita lakukan ke Github untuk di-review oleh kawan-kawan tim translasi yang lain

