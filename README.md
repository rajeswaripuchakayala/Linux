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
