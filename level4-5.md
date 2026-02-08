Task
# Level Goal
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

# Commands you may need to solve this level
ls , cd , cat , file , du , find

# Penjelasan
Terdapat banyak file dalam direktori inhere, carilah salah satu password dari banyaknya file tersebut yang berbentuk ascii text.

# Solusi
Gunakan command find . -type f | xargs file
Find . -type f berfungsi untuk mencari semua isi dalam direktori tersebut yang berbentuk file, kemudian | xargs berfungsi sebagai pipeline\pipa untuk mengecek semua tipe dari file tersebut, kemudian tampilkan isi file yang bertipe ASCII text.

# Hasil

bandit4@bandit:~/inhere$ ls

-file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09

bandit4@bandit:~/inhere$ find . -type f | xargs file

./-file02: OpenPGP Public Key

./-file04: data

./-file08: data

./-file00: data

./-file07: ASCII text

./-file06: data

./-file01: OpenPGP Public Key

./-file03: data

./-file05: data

./-file09: data

bandit4@bandit:~/inhere$ cat ./-file07

4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

# Langkah selanjutnya
exit dan ssh bandit6@bandit.labs.overthewire.org -p 2220

# Password
Password for this level = 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
Gunakan password ini untuk masuk kedalam game berikutnya