# Linux

rajeswarip@DESKTOP-L6IQ400:/$ ls
bin   dev  home  lib    lib64   lost+found  mnt  proc  run   snap  sys  usr
boot  etc  init  lib32  libx32  media       opt  root  sbin  srv   tmp  var

rajeswarip@DESKTOP-L6IQ400:/$ cd home

rajeswarip@DESKTOP-L6IQ400:/home$ pwd
/home

rajeswarip@DESKTOP-L6IQ400:/home$ ls
rajeswarip

rajeswarip@DESKTOP-L6IQ400:/home$ cd rajeswarip

rajeswarip@DESKTOP-L6IQ400:~$ mkdir demo1

rajeswarip@DESKTOP-L6IQ400:~$ ls
demo1

rajeswarip@DESKTOP-L6IQ400:~$ mkdir demo2

rajeswarip@DESKTOP-L6IQ400:~$ ls
demo1  demo2

rajeswarip@DESKTOP-L6IQ400:~$ cd demo1

rajeswarip@DESKTOP-L6IQ400:~/demo1$ touch 1.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
1.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ touch 2.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
1.txt  2.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ cat > sample.txt
This is the sample text file

rajeswarip@DESKTOP-L6IQ400:~/demo1$ cat sample.txt
This is the sample text file

rajeswarip@DESKTOP-L6IQ400:~/demo1$ rm 1.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
2.txt  sample.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ cp 2.txt 1.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
1.txt  2.txt  sample.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ cp sample.txt 1.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
1.txt  2.txt  sample.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ cat 1.txt
This is the sample text file

rajeswarip@DESKTOP-L6IQ400:~/demo1$ cat 2.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ rm 1.txt 2.txt sample.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ cat sample.txt


rajeswarip@DESKTOP-L6IQ400:~/demo1$ vi sample.txt
1) This is the sample text file
2) This file contains all commands
3) first command is pwd (present working directory)
4) second command is cd (change directory)
5) third command is mkdir (create new directory)
6) forth command is rmdir (remove directory)
7) fifth command is ls (list of files)
8) sixth command is touch (creates empty file)
9) seventh command is cat (create file, display content and copy the content of one file to another file)
10) eighth command is rm (remove file)
11) ninth command is cp (copy a file or directory)
12) tenth command is mv (move a file or directory)

rajeswarip@DESKTOP-L6IQ400:~/demo1$ head sample.txt
1) This is the sample text file
2) This file contains all commands
3) first command is pwd (present working directory)
4) second command is cd (change directory)
5) third command is mkdir (create new directory)
6) forth command is rmdir (remove directory)
7) fifth command is ls (list of files)
8) sixth command is touch (creates empty file)
9) seventh command is cat (create file, display content and copy the content of one file to another file)
10) eighth command is rm (remove file)

rajeswarip@DESKTOP-L6IQ400:~/demo1$ tail sample.txt
3) first command is pwd (present working directory)
4) second command is cd (change directory)
5) third command is mkdir (create new directory)
6) forth command is rmdir (remove directory)
7) fifth command is ls (list of files)
8) sixth command is touch (creates empty file)
9) seventh command is cat (create file, display content and copy the content of one file to another file)
10) eighth command is rm (remove file)
11) ninth command is cp (copy a file or directory)
12) tenth command is mv (move a file or directory)

rajeswarip@DESKTOP-L6IQ400:~/demo1$ tac sample.txt
