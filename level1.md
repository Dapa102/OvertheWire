task
# Level Goal
The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

# Commands you may need to solve this level
ls , cd , cat , file , du , find

# Penjelasan
Password untuk level 1 ada didalam file bernama readme yang berada dalam direktori home.

# Solusi
Command = ls dan cat

Gunakan command ls untuk melihat file apa saja yang terdapat dalam direktori tersebut, kemudian commnad cat untuk menampilkan isi dari file tersebut.

# Langkah selanjutnya
exit dan ssh bandit1@bandit.labs.overthewire.org -p 2220

Untuk keluar dari level 0 dan masuk ke level1 menggunakan password yang didapatkan.

# Hasil
bandit0@bandit:~$ ls

readme

bandit0@bandit:~$ cat readme

# Password
The password you are looking for is: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

Dalam file tersebut terdapat sebuah password untuk level 1