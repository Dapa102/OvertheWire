Task
# Level Goal
The password for the next level is stored in a hidden file in the inhere directory.

# Commands you may need to solve this level
ls , cd , cat , file , du , find

# Penjelasan
Terdapat sebuah password yang bersembunyi didalam direktori bernama inhere, temukan cara bagaimana menemukan file tersembunyi tersebut dan menampilkan passwordnya.

# Solusi
gunakan command ls -alps dan cd, cat dan ls -alps untuk menampilkan file tersembunyi dan cat untuk menampilkan isinya.

# Hasil
bandit3@bandit:~$ ls

inhere

bandit3@bandit:~$ cd inhere/

bandit3@bandit:~/inhere$ ls -alps

total 12

4 drwxr-xr-x 2 root    root    4096 Oct 14 09:26 ./

4 drwxr-xr-x 3 root    root    4096 Oct 14 09:26 ../

4 -rw-r----- 1 bandit4 bandit3   33 Oct 14 09:26 ...Hiding-From-You

bandit3@bandit:~/inhere$ cat ...Hiding-From-You 

2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

# Langkah selanjutnya
exit dan ssh bandit5@bandit.labs.overthewire.org -p 2220

# Password
Password for this level = 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
Gunakan password ini untuk masuk kedalam game berikutnya