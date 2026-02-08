Task 
# Level Goal
The password for the next level is stored in a file called --spaces in this filename-- located in the home directory

# Commands you may need to solve this level
ls , cd , cat , file , du , find

# Penjelasan 
Password terdapat dalam file yang bernama --spaces in this filename--, kita diminta untuk menampilkan password tersebut.

# Solusi
Gunakan command ls dan cat. 
Gunakan command cat ./"--spaces in this filename--"
fungsi ./ adalah direktori saat ini, dengan menggunakan tanda "" kita dapat menampilkan isi dari file tersebut.

atau bisa gunakan command berikut.
cat "./--spaces in this filename--"

# Hasil
bandit2@bandit:~$ ls

--spaces in this filename--

bandit2@bandit:~$ cat ./"--spaces in this filename--"

MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

# Langkah selanjutnya
exit dan ssh bandit4@bandit.labs.overthewire.org -p 2220

# Password
Password for this level = MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
Gunakan password ini untuk masuk kedalam game berikutnya 
