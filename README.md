# Linux Commands
1) ls
    a) ls ..  ---> This .. means, we want to print out one folder back the directory structure
    b) ls ../ ..   --> This means, we want to print out two folders back the directory structure
    c) ls -l   ---> l means long list, this command will show the lond list of the directory
    d) ls -a   ---> this command will show the hidden files in the directory
    e) ls -al  ---> this command will show the hidden files and long list in the directory
    f) ls -lS  ---> this command will sort the list by directory size
    g) ls documents/* .html  ---> this command will show the .hmtl files that are in docuemnts folder
    h) ls documents/* .*     ---> this command will show the .files that are in the documents folder
    i) ls -lS >out.txt   ---> this command will save the result of "ls -lS" command into out.txt file. Here out.txt folder is not exust. So it will create a folder and name it as out.txt and save the results into it.
    j) ls -d */  ---> this command will list out the directories
3) cd
4) pwd
5) mkdir
6) rmdir
7) touch
8) cat
    a) cat -b list1.txt  --> this command will add the line numbers except empyt lines
    For Ex:
        1  list 1 line1
        2  list 1 line2

        3  list 1 line3
     b) cat -n list1.txt  --> this command will add the line numbers to all  
     For Ex:
        1  list 1 line1
        2  list 1 line2
        3
        4  list 1 line3
     c) cat -s list1.txt  --> this command will squeeze the multiple empty lines into one signle line.
     For Ex:
        list 1 line1



        list 1 line2



        list 1 line3
        
      Output:
        list 1 line1

        list 1 line2

        list 1 line3
    d) cat -E list1.txt  --> this command will add the $ symbol at the end of each line
    For Ex:
        list 1 line1$
        $
        list 1 line2$
        list 1 line3$
      
10) vi
11) rm
12) cp
13) mv
14) head
15) tail
16) tac
17) more
18) less
19) su
20) **echo** --> echo command is used to create a file, but we should specify the file content on the command line <br>
**for ex:** <br>
    _echo "this is the sample text file created by echo command" > 1.txt_ <br>
   **cat 1.txt** <br>
          _this is the sample test file created by echo command _ <br>
   ** want to append data**<br>
  _ echo "this is the second line i want to append using echo command" >>1.txt_ <br>
  
 19) **printf**  --> printf command is used to create a file, but we should specify the file content on the command line <br>
 **for ex:** <br>
     _ printf "this is the sample text file created by printf command" > 2.txt_ <br>
     
   ** want to append data**<br>
  _ printf "this is the second line i want to append using printf command" >>2.txt_ <br>
  
  20) **wc**  --> used to count the words, lines, and characters in the file <br>
    **for ex:** <br> 
        _wc sample.txt_ <br>
   ** output:** <br>
       1 10 53 sample.txt --> here 1 defines line, 10 defines words, 53 defines characters <br>
       
       wc -l sample.txt  --> i should get only lines count
       wc -w sample.txt  --> i should get words count
       wc -c sample.txt  --> i should get characters count
  
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

