# Linux Commands
1) ls
2) cd
3) pwd
4) mkdir
5) rmdir
6) touch
7) cat
8) vi
9) rm
10) cp
11) mv
12) head
13) tail
14) tac
15) more
16) less
17) su
18) 
.........ls...............
ls --> command is used to view the contents of a directory
rajeswarip@DESKTOP-L6IQ400:/$ ls
bin   dev  home  lib    lib64   lost+found  mnt  proc  run   snap  sys  usr
boot  etc  init  lib32  libx32  media       opt  root  sbin  srv   tmp  var

..........cd..............
cd --> change the directory
rajeswarip@DESKTOP-L6IQ400:/$ cd home

...........pwd...............
pwd --> present working directory
rajeswarip@DESKTOP-L6IQ400:/home$ pwd
/home

rajeswarip@DESKTOP-L6IQ400:/home$ ls
rajeswarip

rajeswarip@DESKTOP-L6IQ400:/home$ cd rajeswarip

...........mkdir.................
mkdir --> create a directory
rajeswarip@DESKTOP-L6IQ400:~$ mkdir demo1

rajeswarip@DESKTOP-L6IQ400:~$ ls
demo1

..........rmdir................
rmdir --> remove directory
rajeswarip@DESKTOP-L6IQ400:~$ mkdir demo2

rajeswarip@DESKTOP-L6IQ400:~$ ls
demo1  demo2

rajeswarip@DESKTOP-L6IQ400:~$ cd demo1

............touch..................
touch --> create a empty text file
rajeswarip@DESKTOP-L6IQ400:~/demo1$ touch 1.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
1.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ touch 2.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
1.txt  2.txt

..............cat.................
cat --> to create a file with content
rajeswarip@DESKTOP-L6IQ400:~/demo1$ cat > sample.txt
This is the sample text file

cat --> to view the content in the file
rajeswarip@DESKTOP-L6IQ400:~/demo1$ cat sample.txt
This is the sample text file

.............rm................
rm --> remove file
rajeswarip@DESKTOP-L6IQ400:~/demo1$ rm 1.txt

rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
2.txt  sample.txt

............cp...................
cp --> copy a file or directory
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

..................vi................
vi --> edit the file
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

..................head.............
head --> it displays first 10 lines of data
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

head -->we can also display n number of lines
rajeswarip@DESKTOP-L6IQ400:~/demo1$ head -n 5 sample.txt
1) This is the sample text file
2) This file contains all commands
3) first command is pwd (present working directory)
4) second command is cd (change directory)
5) third command is mkdir (create new directory)

rajeswarip@DESKTOP-L6IQ400:~/demo1$ head -5 sample.txt
1) This is the sample text file
2) This file contains all commands
3) first command is pwd (present working directory)
4) second command is cd (change directory)
5) third command is mkdir (create new directory)

----->display the lines between the 5 to 8
rajeswarip@DESKTOP-L6IQ400:~/demo1$ head -8 sample.txt | tail -4
5) third command is mkdir (create new directory)
6) forth command is rmdir (remove directory)
7) fifth command is ls (list of files)
8) sixth command is touch (creates empty file)
...................tail...............
tail --> it displays last 10 lines of data
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

tail -->we can also display n number of lines
rajeswarip@DESKTOP-L6IQ400:~/demo1$ tail -n 10 sample.txt
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

rajeswarip@DESKTOP-L6IQ400:~/demo1$ tail -10 sample.txt
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

..............tac.................
tac --> reverse of cat commmand
rajeswarip@DESKTOP-L6IQ400:~/demo1$ tac sample.txt

.............mv..............
mv -->move a file or directory
rajeswarip@DESKTOP-L6IQ400:~/demo1$ touch 1.txt
rajeswarip@DESKTOP-L6IQ400:~/demo1$ touch 2.txt
rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
1.txt  2.txt  sample.txt
rajeswarip@DESKTOP-L6IQ400:~/demo1$ mv 1.txt ~/demo2
rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
2.txt  sample.txt
rajeswarip@DESKTOP-L6IQ400:~/demo1$ cd
rajeswarip@DESKTOP-L6IQ400:~$ cd demo2
rajeswarip@DESKTOP-L6IQ400:~/demo2$ ls
1.txt

..................cp....................
cp -->copy a file or directory
rajeswarip@DESKTOP-L6IQ400:~/demo2$ ls
1.txt
rajeswarip@DESKTOP-L6IQ400:~/demo2$ cp 1.txt ~/demo1
rajeswarip@DESKTOP-L6IQ400:~/demo2$ ls
1.txt
rajeswarip@DESKTOP-L6IQ400:~/demo2$ cd
rajeswarip@DESKTOP-L6IQ400:~$ cd demo1
rajeswarip@DESKTOP-L6IQ400:~/demo1$ ls
1.txt  2.txt  sample.txt

