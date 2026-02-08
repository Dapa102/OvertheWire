Task
# Level Goal
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

    human-readable
    1033 bytes in size
    not executable

# Commands you may need to solve this level
ls , cd , cat , file , du , find

# Penjelasan
Password untuk level selanjutnya berada dalam sebuah direktori inhere, untuk menemukan password tersebut, user harus memenuhi ketentuan yang telah disiapkan.

# Solusi
Gunakan command find . -type f -size 1033c ! -executable | xargs file
1033c menunjukkan bahwa ingin menemukan file yang memiliki ukuran 1033 bytes dan ! -executable maksudnya file yang tidak bisa di execute.

# Hasil
bandit5@bandit:~/inhere$ ls

maybehere00  maybehere02  maybehere04  maybehere06  maybehere08  maybehere10  maybehere12  maybehere14  maybehere16  maybehere18

maybehere01  maybehere03  maybehere05  maybehere07  maybehere09  maybehere11  maybehere13  maybehere15  maybehere17  maybehere19

bandit5@bandit:~/inhere$ find . -type f -size 1033c ! -executable | xargs file

./maybehere07/.file2: ASCII text, with very long lines (1000)

bandit5@bandit:~/inhere$ cat ./maybehere07/.file2

HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

# Langkah selanjutnya
exit dan ssh bandit6@bandit.labs.overthewire.org -p 2220

# Password
Password for this level = HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
Gunakan password ini untuk masuk kedalam game berikutnya