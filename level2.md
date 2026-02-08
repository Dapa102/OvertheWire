Task
# Level Goal
The password for the next level is stored in a file called - located in the home directory

# Commands you may need to solve this level
ls , cd , cat , file , du , find

# Penjelasan
Pada level ini, password terdapat dalam sebuah file bernama - pada direktori home, user diminta untuk mencari cara bagaimana menampilkan password tersebut walau hanya bernama -.

# Solusi
Gunakan command ls dan cat. Gunakan command cat ./- untuk menampilkan isi tersebut, fungsi ./ adalah direktori saat ini.

# Hasil
bandit1@bandit:~$ ls

-

bandit1@bandit:~$ cat ./-

263JGJPfgU6LtdEvgfWU1XP5yac29mFx

# Langkah selanjutnya
exit dan ssh bandit2@bandit.labs.overthewire.org -p 2220

# Password
Password for this level = 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
Gunakan password ini untuk masuk kedalam game berikutnya 