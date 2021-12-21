# https://overthewire.org/wargames/bandit/

**Bandit
--------


**Bandit Level 0
----------------
Level Goal

The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

Commands you may need to solve this level

ssh
*******************
Solution of level 0

#Execution option 1

~$ ssh bandit.labs.overthewire.org -l bandit0 -p2220

bandit0@bandit.labs.overthewire.org's password:bandit0

#Execution option 2

~$ ssh bandit0@bandit.labs.overthewire.org -p 2220

bandit0@bandit.labs.overthewire.org's password:bandit0
**************************
**Bandit Level 0 → Level 1
--------------------------
Level Goal

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

Commands you may need to solve this level

ls, cd, cat, file, du, find
************************
Solution of level 0 -> 1

~$ ls ->

readme

~$ file readme ->

readme: ASCII text

~$ du readme ->

4 readme

~$ find readme ->

readme

~$ cat readme ->

boJ9jbbUNNfktd78OOpsqOltutMc3MY1 -> this line is also our password to the following level
**************************

**Bandit Level 1 → Level 2
--------------------------
Level Goal

The password for the next level is stored in a file called - located in the home directory

Commands you may need to solve this level

ls, cd, cat, file, du, find
***************************

Solution of level 1 -> 2

login 		- bandit1

password 	- boJ9jbbUNNfktd78OOpsqOltutMc3MY1 

~$ ssh bandit.labs.overthewire.org -l bandit1 -p2220

bandit1@bandit.labs.overthewire.org's password:boJ9jbbUNNfktd78OOpsqOltutMc3MY1

~$ ls

_-

#Execution option 1

~$ cat < - 

CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

#Execution option 2

~$ cat ./-

CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
********************************
**Bandit Level 2 → Level 3
------------------------
Level Goal

The password for the next level is stored in a file called spaces in this filename located in the home directory

Commands you may need to solve this level

ls, cd, cat, file, du, find

Helpful Reading Material

Google Search for “spaces in filename”
**************************************
Solution of leve 2 -> 3

login 		- bandit2

password 	- CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

~$ ssh bandit.labs.overthewire.org -l bandit2 -p2220

bandit2@bandit.labs.overthewire.org's password: CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

~$ ls

spaces in this filename

~$ cat 

.bash_logout             .profile  

.bashrc                  spaces in this filename 

#Execution option 1

~$ cat spaces\ in\ this\ filename 

UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

#Execution option 2

~$ cat 'spaces in this filename'

UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
********************************
**Bandit Level 3 → Level 4
--------------------------
Level Goal

The password for the next level is stored in a hidden file in the inhere directory.

Commands you may need to solve this level

ls, cd, cat, file, du, find

******************************************

Solution of level 3 -> 4

~$ ssh bandit.labs.overthewire.org -l bandit3 -p2220

bandit3@bandit.labs.overthewire.org's password: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

bandit3@bandit:~$ ls -l

total 4

drwxr-xr-x 2 root root 4096 May  7 20:14 inhere

bandit3@bandit:~$ ls -l

total 4

drwxr-xr-x 2 root root 4096 May  7 20:14 inhere

bandit3@bandit:~$ file inhere/

inhere/: directory

bandit3@bandit:~$ cd inhere/

bandit3@bandit:~/inhere$ ls -la

total 12

drwxr-xr-x 2 root    root    4096 May  7 20:14 .

drwxr-xr-x 3 root    root    4096 May  7 20:14 ..

-rw-r----- 1 bandit4 bandit3   33 May  7 20:14 .hidden


bandit3@bandit:~/inhere$ cat .hidden 

pIwrPrtPN36QITSp3EQaw936yaFoFgAB
********************************
**Bandit Level 4 → Level 5
--------------------------
Level Goal

The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

Commands you may need to solve this level

ls, cd, cat, file, du, find
*****************************************

Solution of level 4 -> 5

~$ ssh bandit.labs.overthewire.org -l bandit4 -p2220

bandit4@bandit.labs.overthewire.org's password: pIwrPrtPN36QITSp3EQaw936yaFoFgAB

#Execution option 1

bandit4@bandit:~$ ls

inhere

andit4@bandit:~$ file inhere/*

inhere/-file00: data

inhere/-file01: data

inhere/-file02: data

inhere/-file03: data

inhere/-file04: data

inhere/-file05: data

inhere/-file06: data

inhere/-file07: ASCII text

inhere/-file08: data

inhere/-file09: data

bandit4@bandit:~$ cat inhere/-file07

koReBOKuIDDepwhWk7jZC0RTdopnAYKh

#Execution option 2

bandit4@bandit:~/inhere$ file ./*

./-file00: data

./-file01: data

./-file02: data

./-file03: data

./-file04: data

./-file05: data

./-file06: data

./-file07: ASCII text

./-file08: data

./-file09: data

bandit4@bandit:~/inhere$ cat ./-file07

koReBOKuIDDepwhWk7jZC0RTdopnAYKh
********************************
**Bandit Level 5 → Level 6
--------------------------
Level Goal

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable

1033 bytes in size

not executable

Commands you may need to solve this level

ls, cd, cat, file, du, find
*****************************************

Solution of level 5 -> 6

~$ ssh bandit.labs.overthewire.org -l bandit5 -p2220

bandit5@bandit.labs.overthewire.org's password: koReBOKuIDDepwhWk7jZC0RTdopnAYKh

andit5@bandit:~$ ls

inhere

bandit5@bandit:~$ cd inhere/

#Execution option 1

bandit5@bandit:~/inhere$ find -readable -size 1033c

./maybehere07/.file2

bandit5@bandit:~/inhere$ cat maybehere07/.file2

DXjZPULLxYr17uwoI01bNLQbtFemEgo7

#Execution option 2

bandit5@bandit:~/inhere$ find . -type f -size 1033c -exec cat {} \;

DXjZPULLxYr17uwoI01bNLQbtFemEgo7
********************************
**Bandit Level 6 → Level 7
--------------------------
Level Goal

The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size
Commands you may need to solve this level
ls, cd, cat, file, du, find, grep

******************************************

Solution of level 6 -> 7

~$ ssh bandit.labs.overthewire.org -l bandit6 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit6@bandit.labs.overthewire.org's password: DXjZPULLxYr17uwoI01bNLQbtFemEgo7

#Execution option 1

bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password

bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

#Execution option 2

bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null -exec cat {} \;
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

#Execution option 3

bandit6@bandit:~$ find / -group bandit6 -user bandit7 -size 33c -exec cat {} \;
...
find: ‘/var/lib/polkit-1’: Permission denied
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
find: ‘/var/log’: Permission denied
...

#Execution option 4

bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>&1 | grep -F -v Permission
...
find: ‘/proc/16675/fdinfo/5’: No such file or directory
/var/lib/dpkg/info/bandit7.password

#Execution option 5

bandit6@bandit:~$ cd /                                                               
bandit6@bandit:/$ cat `find . -size 33c -group bandit6 -user bandit7 2>/dev/null`
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs 

bandit6@bandit:~$ cd / && cat `find . -size 33c -group bandit6 -user bandit7 2>/dev/null`      
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs 
********************************
Bandit Level 7 → Level 8
Level Goal
The password for the next level is stored in the file data.txt next to the word millionth

Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

************************************************************

Solution of level 7 -> 8

~$ ssh bandit.labs.overthewire.org -l bandit7 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit7@bandit.labs.overthewire.org's password: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

#Execution option 1

bandit7@bandit:~$ ls
data.txt
bandit7@bandit:~$ cat data.txt | grep "millionth"
millionth       cvX2JJa4CFALtqS87jk27qwqGhBM9plV

#Execution option 2

bandit7@bandit:~$ grep "millionth" data.txt
millionth       cvX2JJa4CFALtqS87jk27qwqGhBM9plV
************************************************
Bandit Level 8 → Level 9
Level Goal
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

Helpful Reading Material
Piping and Redirection

*************************************************************

Solution of level 8 -> 9

~$ ssh bandit.labs.overthewire.org -l bandit8 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit8@bandit.labs.overthewire.org's password: cvX2JJa4CFALtqS87jk27qwqGhBM9plV

#Execution option 1

bandit8@bandit:~$ sort data.txt | uniq --unique 
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

#Execution option 2

bandit8@bandit:~$ sort data.txt | uniq -c | grep '^ *1 '
	1 UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

#Execution option 3

andit8@bandit:~$ cat data.txt | sort | uniq --unique 
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
********************************
Bandit Level 9 → Level 10
Level Goal
The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

*************************************************************

Solution of level 9 -> 10

~$ ssh bandit.labs.overthewire.org -l bandit9 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit9@bandit.labs.overthewire.org's password: UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

#Execution option 1

bandit9@bandit:~$ grep -a == data.txt
...===== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

#Execution option 2

bandit9@bandit:~$ strings data.txt | grep -E '=+'
========== the*2i"4
=:G e
========== password
<I=zsGi
Z)========== is
A=|t&E
Zdb=
c^ LAh=3G
*SF=s
&========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
S=A.H&^
********************************************
Bandit Level 10 → Level 11
Level Goal
The password for the next level is stored in the file data.txt, which contains base64 encoded data

Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

Helpful Reading Material
Base64 on Wikipedia

*************************************************************

Solution of level 10 -> 11

~$ ssh bandit.labs.overthewire.org -l bandit10 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit10@bandit.labs.overthewire.org's password: truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

#Execution option 1

bandit10@bandit:~$ ls
data.txt
bandit10@bandit:~$ cat data.txt 
VGhlIHBhc3N3b3JkIGlzIElGdWt3S0dzRlc4TU9xM0lSRnFyeEUxaHhUTkViVVBSCg==
bandit10@bandit:~$ base64 --decode data.txt 
The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

#Execution option 2

bandit10@bandit:~$ cat data.txt | base64 --decode 
The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

#Execution option 3

bandit10@bandit:~$ base64 -d data.txt | cut -d" " -f4
IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
********************************
Bandit Level 11 → Level 12
Level Goal
The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

Helpful Reading Material
Rot13 on Wikipedia

************************************************************

Solution of level 11 -> 12

~$ ssh bandit.labs.overthewire.org -l bandit11 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit11@bandit.labs.overthewire.org's password: IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

#Execution option 1

bandit11@bandit:~$ ls
data.txt
bandit11@bandit:~$ cat data.txt 
Gur cnffjbeq vf 5Gr8L4qetPEsPk8htqjhRK8XSP6x2RHh
>>https://rot13.com -> copy/paste "Gur cnffjbeq vf 5Gr8L4qetPEsPk8htqjhRK8XSP6x2RHh" -> "The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu"

#Execution option 2

bandit11@bandit:~$ cat data.txt | tr a-zA-Z n-za-mN-ZA-M
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

#Execution option 3

bandit11@bandit:~$ cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

#Execution option 4

bandit11@bandit:~$ cat data.txt | tr “[a-zA-Z]” “[n-za-mN-ZA-M]”
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

#Execution option 5

bandit11@bandit:~$ cat data.txt | tr “n-za-mN-ZA-M” “a-zA-Z”
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

#Execution option 6

bandit11@bandit:~$ cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m' | cut -d" " -f4
5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
********************************
Bandit Level 12 → Level 13
Level Goal
The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd, mkdir, cp, mv, file

Helpful Reading Material
Hex dump on Wikipedia

************************************************************************************

Solution of level 12 -> 13 

~$ ssh bandit.labs.overthewire.org -l bandit12 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit12@bandit.labs.overthewire.org's password: 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

#Execution option 1

bandit12@bandit:~$ ls
data.txt
bandit12@bandit:~$ mkdir /tmp/myname123
mkdir: cannot create directory ‘/tmp/myname123’: File exists
bandit12@bandit:/tmp/myname123$ cp ~bandit12/data.txt /tmp/myname123 && mv data.txt data_test.txt
bandit12@bandit:/tmp/myname123$ ls
data_test.txt
bandit12@bandit:/tmp/myname123$ file data_test.txt 
data_test.txt: ASCII 
bandit12@bandit:/tmp/myname123$ xxd -r data_test.txt data
bandit12@bandit:/tmp/myname123$ ls
data  data_test.txt
bandit12@bandit:/tmp/myname123$ file data
data: gzip compressed data, was "data2.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix

bandit12@bandit:/tmp/myname123$ mv data data.gz
bandit12@bandit:/tmp/myname123$ gzip -d data.gz
bandit12@bandit:/tmp/myname123$ file data
data: bzip2 compressed data, block size = 900k

bandit12@bandit:/tmp/myname123$ mv data data.bz2
bandit12@bandit:/tmp/myname123$ bzip2 -d data.bz2
bandit12@bandit:/tmp/myname123$ file data
data: gzip compressed data, was "data4.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix

bandit12@bandit:/tmp/myname123$ mv data data.gz
bandit12@bandit:/tmp/myname123$ gzip -d data.gz
bandit12@bandit:/tmp/myname123$ file data
data: POSIX tar archive (GNU)

bandit12@bandit:/tmp/myname123$ mv data data.tar
bandit12@bandit:/tmp/myname123$ tar xvf data.tar
data5.bin
bandit12@bandit:/tmp/myname123$ file data5.bin
data5.bin: POSIX tar archive (GNU)

bandit12@bandit:/tmp/myname123$ mv data5.bin data5.tar
bandit12@bandit:/tmp/myname123$ tar xvf data5.tar
data6.bin
bandit12@bandit:/tmp/myname123$ file data6.bin
data6.bin: bzip2 compressed data, block size = 900k

bandit12@bandit:/tmp/myname123$ mv data6.bin data6.tar
bandit12@bandit:/tmp/myname123$ tar xvf data6.tar
data8.bin
bandit12@bandit:/tmp/myname123$ file data8.bin
data8.bin: gzip compressed data, was "data9.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix

bandit12@bandit:/tmp/myname123$ mv data8.bin data8.gz
bandit12@bandit:/tmp/myname123$ gzip -d data8.gz
bandit12@bandit:/tmp/myname123$ file data8
data8: ASCII text

bandit12@bandit:/tmp/myname123$ cat data8
The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

bandit12@bandit:/tmp/myname123$ ls
data5.tar  data6.tar  data8  data.tar  data_test.txt

bandit12@bandit:/tmp/myname123$ rm -rf /tmp/myname123 -v
removed '/tmp/myname123/data6.tar'
removed '/tmp/myname123/data.tar'
removed '/tmp/myname123/data8'
removed '/tmp/myname123/data5.tar'
removed '/tmp/myname123/data_test.txt'
removed directory '/tmp/myname123'


#Execution option 2

bandit12@bandit:~$ mkdir /tmp/myname123
bandit12@bandit:~$ cp data.txt /tmp/myname123
bandit12@bandit:~$ cd /tmp/myname123
bandit12@bandit:/tmp/myname123$ ls
data.txt

bandit12@bandit:/tmp/myname123$ xxd -r data.txt > data.bin
bandit12@bandit:/tmp/myname123$ ls
data.bin  data.txt

andit12@bandit:/tmp/myname123$ zcat data.bin > data1
bandit12@bandit:/tmp/myname123$ ls
data1  data.bin  data.txt

bandit12@bandit:/tmp/myname123$ file data1 data.bin data.txt 
data1:    bzip2 compressed data, block size = 900k
data.bin: gzip compressed data, was "data2.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix
data.txt: ASCII text

bandit12@bandit:/tmp/myname123$ bzcat data1 > data2
bandit12@bandit:/tmp/myname123$ file data2
data2: gzip compressed data, was "data4.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix

bandit12@bandit:/tmp/myname123$ tar -xvf data2
data5.bin
bandit12@bandit:/tmp/myname123$ file data5.bin 
data5.bin: POSIX tar archive (GNU)

andit12@bandit:/tmp/myname123$ tar -xvf data5.bin
data6.bin
bandit12@bandit:/tmp/myname123$ file data6.bin 
data6.bin: bzip2 compressed data, block size = 900k

bandit12@bandit:/tmp/myname123$ bzcat data6.bin > data7
bandit12@bandit:/tmp/myname123$ file data7
data7: POSIX tar archive (GNU)

bandit12@bandit:/tmp/myname123$ tar -xvf data7
data8.bin
bandit12@bandit:/tmp/myname123$ file data8.bin 
data8.bin: gzip compressed data, was "data9.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix

bandit12@bandit:/tmp/myname123$ zcat data8.bin > data9
bandit12@bandit:/tmp/myname123$ file data9
data9: ASCII text

bandit12@bandit:/tmp/myname123$ cat data9
The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

bandit12@bandit:/tmp/myname123$ ls -l
total 52
-rw-r--r-- 1 bandit12 root   573 Jul 29 12:28 data1
-rw-r--r-- 1 bandit12 root   431 Jul 29 12:32 data2
-rw-r--r-- 1 bandit12 root 10240 May  7 20:14 data5.bin
-rw-r--r-- 1 bandit12 root   222 May  7 20:14 data6.bin
-rw-r--r-- 1 bandit12 root 10240 Jul 29 12:38 data7
-rw-r--r-- 1 bandit12 root    79 May  7 20:14 data8.bin
-rw-r--r-- 1 bandit12 root    49 Jul 29 12:41 data9
-rw-r--r-- 1 bandit12 root   606 Jul 29 12:26 data.bin
-rw-r----- 1 bandit12 root  2582 Jul 29 12:24 data.txt
******************************************************
Bandit Level 13 → Level 14
Level Goal
The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

Commands you may need to solve this level
ssh, telnet, nc, openssl, s_client, nmap

Helpful Reading Material
SSH/OpenSSH/Keys

******************************************

Solution of level 13 -> 14

~$ ssh bandit.labs.overthewire.org -l bandit13 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit13@bandit.labs.overthewire.org's password: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

bandit13@bandit:~$ ls
sshkey.private
bandit13@bandit:~$ ssh bandit14@localhost -i sshkey.private 
Could not create directory '/home/bandit13/.ssh'.
The authenticity of host 'localhost (127.0.0.1)' can't be established.
ECDSA key fingerprint is SHA256:98UL0ZWr85496EtCRkKlo20X3OPnyPSB5tB5RPbhczc.
Are you sure you want to continue connecting (yes/no)? yes

bandit14@bandit:/etc/bandit_pass$ cat /etc/bandit_pass/bandit14
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

bandit13@bandit:~$ ssh -i ./sskey.private bandit14@localhost
Warning: Identity file ./sskey.private not accessible: No such file or directory.
Could not create directory '/home/bandit13/.ssh'.
The authenticity of host 'localhost (127.0.0.1)' can't be established.
ECDSA key fingerprint is SHA256:98UL0ZWr85496EtCRkKlo20X3OPnyPSB5tB5RPbhczc.
Are you sure you want to continue connecting (yes/no)? yes
Failed to add the host to the list of known hosts (/home/bandit13/.ssh/known_hosts).
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit14@localhost's password: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

bandit14@bandit:~$ whoami
bandit14
*************************
Bandit Level 14 → Level 15
Level Goal
The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost. [Пароль для следующего уровня можно получить, отправив пароль текущего уровня на порт 30000 на локальном хосте.]
Commands you may need to solve this level
ssh, telnet, nc, openssl, s_client, nmap

Helpful Reading Material
How the Internet works in 5 minutes (YouTube) (Not completely accurate, but good enough for beginners)
IP Addresses
IP Address on Wikipedia
Localhost on Wikipedia
Ports
Port (computer networking) on Wikipedia

****************************************

Solution of level 14 -> 15

~$ ssh bandit.labs.overthewire.org -l bandit14 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit14@bandit.labs.overthewire.org's password: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

bandit14@bandit:~$ nc localhost  30000
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr
********************************
Bandit Level 15 → Level 16
Level Goal
The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.

Helpful note: Getting “HEARTBEATING” and “Read R BLOCK”? Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command…

Commands you may need to solve this level
ssh, telnet, nc, openssl, s_client, nmap

Helpful Reading Material
Secure Socket Layer/Transport Layer Security on Wikipedia
OpenSSL Cookbook - Testing with OpenSSL

**********************************************************

Solution of level 15 -> 16

~$ ssh bandit.labs.overthewire.org -l bandit15 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit15@bandit.labs.overthewire.org's password: BfMYroe26WYalil77FoDi9qh59eK5xNr

#Execution option 1

bandit15@bandit:~$ openssl s_client -connect localhost:30001
CONNECTED(00000003)
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
---
Certificate chain
 0 s:/CN=localhost
   i:/CN=localhost
---
Server certificate
-----BEGIN CERTIFICATE-----
MIICBjCCAW+gAwIBAgIEDU18oTANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDDAls
b2NhbGhvc3QwHhcNMjAwNTA3MTgxNTQzWhcNMjEwNTA3MTgxNTQzWjAUMRIwEAYD
VQQDDAlsb2NhbGhvc3QwgZ8wDQYJKoZIhvcNAQEBBQADgY0AMIGJAoGBAK3CPNFR
FEypcqUa8NslmIMWl9xq53Cwhs/fvYHAvauyfE3uDVyyX79Z34Tkot6YflAoufnS
+puh2Kgq7aDaF+xhE+FPcz1JE0C2bflGfEtx4l3qy79SRpLiZ7eio8NPasvduG5e
pkuHefwI4c7GS6Y7OTz/6IpxqXBzv3c+x93TAgMBAAGjZTBjMBQGA1UdEQQNMAuC
CWxvY2FsaG9zdDBLBglghkgBhvhCAQ0EPhY8QXV0b21hdGljYWxseSBnZW5lcmF0
ZWQgYnkgTmNhdC4gU2VlIGh0dHBzOi8vbm1hcC5vcmcvbmNhdC8uMA0GCSqGSIb3
DQEBBQUAA4GBAC9uy1rF2U/OSBXbQJYuPuzT5mYwcjEEV0XwyiX1MFZbKUlyFZUw
rq+P1HfFp+BSODtk6tHM9bTz+p2OJRXuELG0ly8+Nf/hO/mYS1i5Ekzv4PL9hO8q
PfmDXTHs23Tc7ctLqPRj4/4qxw6RF4SM+uxkAuHgT/NDW1LphxkJlKGn
-----END CERTIFICATE-----
subject=/CN=localhost
issuer=/CN=localhost
---
No client certificate CA names sent
Peer signing digest: SHA512
Server Temp Key: X25519, 253 bits
---
SSL handshake has read 1019 bytes and written 269 bytes
Verification error: self signed certificate
---
New, TLSv1.2, Cipher is ECDHE-RSA-AES256-GCM-SHA384
Server public key is 1024 bit
Secure Renegotiation IS supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
SSL-Session:
    Protocol  : TLSv1.2
    Cipher    : ECDHE-RSA-AES256-GCM-SHA384
    Session-ID: 1193DFF01A55845B11DB75667AF8CC93F2CA944167D1FD003EFC26416CE83169
    Session-ID-ctx: 
    Master-Key: 57291BD42F3B3AD4F7D9AEB7875EB3404ED5E436F080B9A455EE09A66F6FE7A48EB828C203FAC81F7C2AAA863276B5BA
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - aa 02 e6 3a 2e 0b c8 5d-6f 54 4a 1b 5a e0 2c 0e   ...:...]oTJ.Z.,.
    0010 - 90 88 b6 5b 82 4a a0 69-ea d7 59 48 29 a4 57 b7   ...[.J.i..YH).W.
    0020 - ec 43 df b8 12 b6 8c 0c-44 59 00 f5 c2 d1 33 fe   .C......DY....3.
    0030 - b5 bc b2 b1 ad 67 e9 1f-84 12 66 16 52 ec d3 dc   .....g....f.R...
    0040 - cf d1 86 ee fe a9 15 b0-56 57 66 43 3c 36 fe 12   ........VWfC<6..
    0050 - d2 3e 89 90 62 8a 6b e4-7b ce ea 78 a0 96 69 bd   .>..b.k.{..x..i.
    0060 - e7 a9 5e c1 5c ab fc 41-e3 0d 97 8e 0f 35 f0 5f   ..^.\..A.....5._
    0070 - 3d 73 03 4a 6e 09 b8 6b-b3 71 60 06 3d 32 b7 b4   =s.Jn..k.q`.=2..
    0080 - 72 11 b6 37 d3 cb 5c 73-2b b2 5a cd 6f 4d 3b 0e   r..7..\s+.Z.oM;.
    0090 - 4c 0e 82 26 92 f4 ba 54-bb 32 0f 43 c7 8a fa b5   L..&...T.2.C....

    Start Time: 1596046156
    Timeout   : 7200 (sec)
    Verify return code: 18 (self signed certificate)
    Extended master secret: yes
---
BfMYroe26WYalil77FoDi9qh59eK5xNr
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd

closed

#Execution option 2

bandit15@bandit:~$ openssl s_client -connect localhost:30001 -quiet
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
BfMYroe26WYalil77FoDi9qh59eK5xNr
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd

#Execution option 3

bandit15@bandit:~$ cat /etc/bandit_pass/bandit15 | openssl s_client -connect localhost:30001 -quiet
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd

#Execution option 4

bandit15@bandit:~$ echo BfMYroe26WYalil77FoDi9qh59eK5xNr | openssl s_client -quiet -connect localhost:30001
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd

#Execution option 5

bandit15@bandit:~$ openssl s_client -connect localhost:30001 -quiet < /etc/bandit_pass/bandit15
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd

#Execution option 6

bandit15@bandit:~$ openssl s_client -ign_eof -connect localhost:30001
CONNECTED(00000003)
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
---
Certificate chain
 0 s:/CN=localhost
   i:/CN=localhost
---
Server certificate
-----BEGIN CERTIFICATE-----
MIICBjCCAW+gAwIBAgIEDU18oTANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDDAls
b2NhbGhvc3QwHhcNMjAwNTA3MTgxNTQzWhcNMjEwNTA3MTgxNTQzWjAUMRIwEAYD
VQQDDAlsb2NhbGhvc3QwgZ8wDQYJKoZIhvcNAQEBBQADgY0AMIGJAoGBAK3CPNFR
FEypcqUa8NslmIMWl9xq53Cwhs/fvYHAvauyfE3uDVyyX79Z34Tkot6YflAoufnS
+puh2Kgq7aDaF+xhE+FPcz1JE0C2bflGfEtx4l3qy79SRpLiZ7eio8NPasvduG5e
pkuHefwI4c7GS6Y7OTz/6IpxqXBzv3c+x93TAgMBAAGjZTBjMBQGA1UdEQQNMAuC
CWxvY2FsaG9zdDBLBglghkgBhvhCAQ0EPhY8QXV0b21hdGljYWxseSBnZW5lcmF0
ZWQgYnkgTmNhdC4gU2VlIGh0dHBzOi8vbm1hcC5vcmcvbmNhdC8uMA0GCSqGSIb3
DQEBBQUAA4GBAC9uy1rF2U/OSBXbQJYuPuzT5mYwcjEEV0XwyiX1MFZbKUlyFZUw
rq+P1HfFp+BSODtk6tHM9bTz+p2OJRXuELG0ly8+Nf/hO/mYS1i5Ekzv4PL9hO8q
PfmDXTHs23Tc7ctLqPRj4/4qxw6RF4SM+uxkAuHgT/NDW1LphxkJlKGn
-----END CERTIFICATE-----
subject=/CN=localhost
issuer=/CN=localhost
---
No client certificate CA names sent
Peer signing digest: SHA512
Server Temp Key: X25519, 253 bits
---
SSL handshake has read 1019 bytes and written 269 bytes
Verification error: self signed certificate
---
New, TLSv1.2, Cipher is ECDHE-RSA-AES256-GCM-SHA384
Server public key is 1024 bit
Secure Renegotiation IS supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
SSL-Session:
    Protocol  : TLSv1.2
    Cipher    : ECDHE-RSA-AES256-GCM-SHA384
    Session-ID: A045B0172FE570D9C9CFB8CAD1B177BE2E172C5E0ED53F191C7529F6D9E76960
    Session-ID-ctx: 
    Master-Key: AA0A89D7377B7AFE611FC9B5531BAE757D30E1EC7EFD36148882DBBBC9772AF030DFEAB6B208242A38DD934E3A257CDE
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - aa 02 e6 3a 2e 0b c8 5d-6f 54 4a 1b 5a e0 2c 0e   ...:...]oTJ.Z.,.
    0010 - 6e b4 28 f1 be 5e 39 c9-61 f3 d8 aa 16 99 78 81   n.(..^9.a.....x.
    0020 - de 7e 5f 85 38 34 95 bc-fa 1c cc 6f 28 42 f0 0f   .~_.84.....o(B..
    0030 - e8 87 16 dd d8 46 39 52-ba fa a7 a5 cc cf 8d 78   .....F9R.......x
    0040 - cd f6 e1 19 a7 3a dc 41-38 55 c3 ba b5 fa 16 09   .....:.A8U......
    0050 - b8 7f e8 b7 a2 81 fb 7c-d5 50 3b df 42 f2 b9 ab   .......|.P;.B...
    0060 - a3 54 c7 06 a7 b8 43 3e-63 e8 bb 1d 66 8a 1b 34   .T....C>c...f..4
    0070 - 35 ca 45 22 77 40 d3 94-54 3a 23 49 a7 b0 6b 84   5.E"w@..T:#I..k.
    0080 - f6 3c d4 44 2d e7 99 ad-78 10 a1 a7 f2 50 90 14   .<.D-...x....P..
    0090 - 56 b1 85 5e e8 59 d9 99-e2 04 54 50 48 e1 67 67   V..^.Y....TPH.gg

    Start Time: 1596046981
    Timeout   : 7200 (sec)
    Verify return code: 18 (self signed certificate)
    Extended master secret: yes
---
BfMYroe26WYalil77FoDi9qh59eK5xNr
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd

closed
********************************
Bandit Level 16 → Level 17
Level Goal
The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

Commands you may need to solve this level
ssh, telnet, nc, openssl, s_client, nmap

Helpful Reading Material
Port scanner on Wikipedia

******************************************

~$ ssh bandit.labs.overthewire.org -l bandit16 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit16@bandit.labs.overthewire.org's password: cluFn7wTiGryunymYOu4RcffSxQluehd

#Execution option 1

bandit16@bandit:~$ nmap localhost 

Starting Nmap 7.40 ( https://nmap.org ) at 2020-07-29 20:55 CEST
Nmap scan report for localhost (127.0.0.1)
Host is up (0.00027s latency).
Not shown: 997 closed ports
PORT      STATE SERVICE
22/tcp    open  ssh
113/tcp   open  ident
30000/tcp open  ndmps

Nmap done: 1 IP address (1 host up) scanned in 0.10 seconds
bandit16@bandit:~$ nmap localhost -p 31000-32000

Starting Nmap 7.40 ( https://nmap.org ) at 2020-07-29 20:56 CEST
Nmap scan report for localhost (127.0.0.1)
Host is up (0.00043s latency).
Not shown: 996 closed ports
PORT      STATE SERVICE
31046/tcp open  unknown
31518/tcp open  unknown
31691/tcp open  unknown
31790/tcp open  unknown
31960/tcp open  unknown

Nmap done: 1 IP address (1 host up) scanned in 0.10 seconds
bandit16@bandit:~$ nmap localhost -p31000-32000 -sV

Starting Nmap 7.40 ( https://nmap.org ) at 2020-07-29 20:58 CEST
Nmap scan report for localhost (127.0.0.1)
Host is up (0.00034s latency).
Not shown: 996 closed ports
PORT      STATE SERVICE     VERSION
31046/tcp open  echo
31518/tcp open  ssl/echo
31691/tcp open  echo
31790/tcp open  ssl/unknown
31960/tcp open  echo
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port31790-TCP:V=7.40%T=SSL%I=7%D=7/29%Time=5F21C6D2%P=x86_64-pc-linux-g
SF:nu%r(GenericLines,31,"Wrong!\x20Please\x20enter\x20the\x20correct\x20cu
SF:rrent\x20password\n")%r(GetRequest,31,"Wrong!\x20Please\x20enter\x20the
SF:\x20correct\x20current\x20password\n")%r(HTTPOptions,31,"Wrong!\x20Plea
SF:se\x20enter\x20the\x20correct\x20current\x20password\n")%r(RTSPRequest,
SF:31,"Wrong!\x20Please\x20enter\x20the\x20correct\x20current\x20password\
SF:n")%r(Help,31,"Wrong!\x20Please\x20enter\x20the\x20correct\x20current\x
SF:20password\n")%r(SSLSessionReq,31,"Wrong!\x20Please\x20enter\x20the\x20
SF:correct\x20current\x20password\n")%r(TLSSessionReq,31,"Wrong!\x20Please
SF:\x20enter\x20the\x20correct\x20current\x20password\n")%r(Kerberos,31,"W
SF:rong!\x20Please\x20enter\x20the\x20correct\x20current\x20password\n")%r
SF:(FourOhFourRequest,31,"Wrong!\x20Please\x20enter\x20the\x20correct\x20c
SF:urrent\x20password\n")%r(LPDString,31,"Wrong!\x20Please\x20enter\x20the
SF:\x20correct\x20current\x20password\n")%r(LDAPSearchReq,31,"Wrong!\x20Pl
SF:ease\x20enter\x20the\x20correct\x20current\x20password\n")%r(SIPOptions
SF:,31,"Wrong!\x20Please\x20enter\x20the\x20correct\x20current\x20password
SF:\n");

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 88.85 seconds

bandit16@bandit:~$ openssl s_client -connect localhost:31790 -quiet
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
cluFn7wTiGryunymYOu4RcffSxQluehd
Correct!
-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
-----END RSA PRIVATE KEY-----

#Execution option 2

bandit16@bandit:~$ cd /tmp/
bandit16@bandit:/tmp$ mkdir bandit17
bandit16@bandit:~$ cat /etc/bandit_pass/bandit16 | openssl s_client -connect localhost:31790 -quiet > /tmp/bandit17/bandit17.key
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
bandit16@bandit:~$ ls /tmp/bandit17/
bandit17.key
bandit16@bandit:~$ chmod 600 /tmp/bandit17/bandit17.key
bandit16@bandit:~$ ssh -i /tmp/bandit17/bandit17.key bandit17@localhost 
Could not create directory '/home/bandit16/.ssh'.
The authenticity of host 'localhost (127.0.0.1)' can't be established.
ECDSA key fingerprint is SHA256:98UL0ZWr85496EtCRkKlo20X3OPnyPSB5tB5RPbhczc.
Are you sure you want to continue connecting (yes/no)? yes

bandit17@bandit:~$ cat /etc/bandit_pass/bandit17 
xLYVMN9WE5zQ5vHacb0sZEVqbrp7nBTn
************************************************
Bandit Level 17 → Level 18
Level Goal
There are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19

Commands you may need to solve this level
cat, grep, ls, diff

*****************************************

Solution of level 17 -> 18

~$ ssh bandit.labs.overthewire.org -l bandit17 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit17@bandit.labs.overthewire.org's password: xLYVMN9WE5zQ5vHacb0sZEVqbrp7nBTn

#Execution option 1

bandit17@bandit:~$ ls
passwords.new  passwords.old
bandit17@bandit:~$ diff passwords.new passwords.old 
42c42
< kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
---
> w0Yfolrc5bwjS4qw5mq1nnQi6mF03bii

#execution option 2

bandit17@bandit:~$ grep -vf passwords.old passwords.new
kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
********************************
Bandit Level 18 → Level 19
Level Goal
The password for the next level is stored in a file readme in the homedirectory. Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

Commands you may need to solve this level
ssh, ls, cat

*****************************************

Solution of leve 18 -> 19

#Execution optoin 1

~$ ssh bandit.labs.overthewire.org -l bandit18 -p2220 "cat readme"
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit18@bandit.labs.overthewire.org's password: kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

#Execution optoin 2

~$ ssh bandit.labs.overthewire.org -l bandit18 -p2220 cat "readme" > password
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit18@bandit.labs.overthewire.org's password: kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
kali@kali:~$ cat password 
IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

#Execution option 3

~$ ssh -t bandit18@bandit.labs.overthewire.org -p2220  /bin/sh
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit18@bandit.labs.overthewire.org's password: 
$ ls
readme
$ cat readme    
IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x
********************************
Bandit Level 19 → Level 20
Level Goal
To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

Helpful Reading Material
setuid on Wikipedia

************************

Solution of level 19 -> 20

~$ ssh bandit.labs.overthewire.org -l bandit19 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit19@bandit.labs.overthewire.org's password: IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

bandit19@bandit:~$ ls -l
total 8
-rwsr-x--- 1 bandit20 bandit19 7296 May  7 20:14 bandit20-do

bandit19@bandit:~$ file bandit20-do 
bandit20-do: setuid ELF 32-bit LSB executable, Intel 80386, version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux.so.2, for GNU/Linux 2.6.32, BuildID[sha1]=8e941f24b8c5cd0af67b22b724c57e1ab92a92a1, not stripped

bandit19@bandit:~$ ./bandit20-do id
uid=11019(bandit19) gid=11019(bandit19) euid=11020(bandit20) groups=11019(bandit19)

bandit19@bandit:~$ ./bandit20-do 
Run a command as another user.
  Example: ./bandit20-do id

bandit19@bandit:~$ ./bandit20-do cat /etc/bandit_pass/bandit20
GbKksEFF4yrVs6il55v6gwY5aVje5f0j
********************************
Bandit Level 20 → Level 21
Level Goal
There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

NOTE: Try connecting to your own network daemon to see if it works as you think

Commands you may need to solve this level
ssh, nc, cat, bash, screen, tmux, Unix ‘job control’ (bg, fg, jobs, &, CTRL-Z, …)

**********************************************************************************

~$ ssh bandit.labs.overthewire.org -l bandit20 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit20@bandit.labs.overthewire.org's password: GbKksEFF4yrVs6il55v6gwY5aVje5f0j

#Execution option 1
bandit20@bandit:~$ ls -la
total 32
drwxr-xr-x  2 root     root      4096 May  7 20:14 .
drwxr-xr-x 41 root     root      4096 May  7 20:14 ..
-rw-r--r--  1 root     root       220 May 15  2017 .bash_logout
-rw-r--r--  1 root     root      3526 May 15  2017 .bashrc
-rw-r--r--  1 root     root       675 May 15  2017 .profile
-rwsr-x---  1 bandit21 bandit20 12088 May  7 20:14 suconnect

bandit20@bandit:~$ file suconnect 
suconnect: setuid ELF 32-bit LSB executable, Intel 80386, version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux.so.2, for GNU/Linux 2.6.32, BuildID[sha1]=74c0f6dc184e0412b6dc52e542782f43807268e1, not stripped

bandit20@bandit:~$ ps aux
USER       PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
bandit20  2899  0.0  0.1  21180  5020 pts/35   Ss   19:33   0:00 -bash
bandit20  3658  0.0  0.0  19328  3004 pts/35   S+   19:35   0:00 tmux
bandit20  3659  0.0  0.1  21188  4952 pts/7    Ss+  19:35   0:00 -bash
bandit20 14041  0.0  0.1  21148  4860 pts/84   Ss   19:55   0:00 -bash
bandit20 14392  0.0  0.1  21148  4860 pts/90   Ss+  19:56   0:00 -bash
bandit20 15566  0.0  0.0  19188  2484 pts/84   R+   19:59   0:00 ps aux
bandit20 18794  0.0  0.1  21148  5048 pts/60   Ss+  18:58   0:00 -bash
bandit20 22445  0.0  0.0  28168  3440 ?        Ss   19:08   0:00 tmux
bandit20 29827  0.0  0.1  21148  5032 pts/67   Ss   19:22   0:00 -bash
bandit20 32263  0.0  0.1  46640  5616 pts/67   S+   19:27   0:00 ssh bandit21@localhost

bandit20@bandit:~$ echo "GbKksEFF4yrVs6il55v6gwY5aVje5f0j" | nc -l localhost -p12345 &
[1] 16857
bandit20@bandit:~$ ./suconnect 12345
Read: GbKksEFF4yrVs6il55v6gwY5aVje5f0j
Password matches, sending next password
gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr
[1]+  Done                    echo "GbKksEFF4yrVs6il55v6gwY5aVje5f0j" | nc -l localhost -p12345



#Execution option 2
> terminal_1
bandit20@bandit:~$ nc -vlp 12345 < /etc/bandit_pass/bandit20
listening on [any] 12345 ...
connect to [127.0.0.1] from localhost [127.0.0.1] 49062
gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr

> terminal_2
bandit20@bandit:~$ ./suconnect 12345
Read: GbKksEFF4yrVs6il55v6gwY5aVje5f0j
Password matches, sending next password
***************************************
Bandit Level 21 → Level 22
Level Goal
A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

Commands you may need to solve this level
cron, crontab, crontab(5) (use “man 5 crontab” to access this)

**************************************************************

Solution of level 21 -> 22

~$ ssh bandit.labs.overthewire.org -l bandit21 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit21@bandit.labs.overthewire.org's password: gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr

bandit21@bandit:~$ cat /etc/cron.d/cronjob_bandit22
@reboot bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null
* * * * * bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null

bandit21@bandit:~$ cd /etc/cron.d/
bandit21@bandit:/etc/cron.d$ ls -l
total 24
-rw-r--r-- 1 root root  62 May 14 13:40 cronjob_bandit15_root
-rw-r--r-- 1 root root  62 Jul 11 15:56 cronjob_bandit17_root
-rw-r--r-- 1 root root 120 May  7 20:14 cronjob_bandit22
-rw-r--r-- 1 root root 122 May  7 20:14 cronjob_bandit23
-rw-r--r-- 1 root root 120 May 14 09:41 cronjob_bandit24
-rw-r--r-- 1 root root  62 May 14 14:04 cronjob_bandit25_root

bandit21@bandit:/etc/cron.d$ cat /usr/bin/cronjob_bandit22.sh 
#!/bin/bash
chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv

bandit21@bandit:/etc/cron.d$ cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI
********************************
Bandit Level 22 → Level 23
Level Goal
A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: Looking at shell scripts written by other people is a very useful skill. The script for this level is intentionally made easy to read. If you are having problems understanding what it does, try executing it to see the debug information it prints.

Commands you may need to solve this level
cron, crontab, crontab(5) (use “man 5 crontab” to access this)

**************************************************************

Solution of level 22 -> 23

~$ ssh bandit.labs.overthewire.org -l bandit22 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit22@bandit.labs.overthewire.org's password: Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI

bandit22@bandit:~$ cat /etc/cron.d/cronjob_bandit23
@reboot bandit23 /usr/bin/cronjob_bandit23.sh  &> /dev/null                                     
* * * * * bandit23 /usr/bin/cronjob_bandit23.sh  &> /dev/null                                   
bandit22@bandit:~$ cat /usr/bin/cronjob_bandit23.sh
#!/bin/bash                                                                                     
                                                                                                
myname=$(whoami)                                                                                
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)                                   
                                                                                                
echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"                          
                                                                                                
cat /etc/bandit_pass/$myname > /tmp/$mytarget 

bandit22@bandit:~$ echo I am user bandit23 | md5sum | cut -d ' ' -f 1
8ca319486bfbbc3663ea0fbe81326349

bandit22@bandit:~$ cat /tmp/8ca319486bfbbc3663ea0fbe81326349
jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n
********************************
Bandit Level 23 → Level 24
Level Goal
A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

NOTE 2: Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…

Commands you may need to solve this level
cron, crontab, crontab(5) (use “man 5 crontab” to access this)

**************************************************************

Solution of level 23 -> 24

~$ ssh bandit.labs.overthewire.org -l bandit23 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit23@bandit.labs.overthewire.org''s password: jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n

bandit23@bandit:~$ cat /etc/cron.d/cronjob_bandit24
@reboot bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
* * * * * bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null

bandit23@bandit:~$ cat /usr/bin/cronjob_bandit24.sh
#!/bin/bash

myname=$(whoami)

cd /var/spool/$myname
echo "Executing and deleting all scripts in /var/spool/$myname:"
for i in * .*;
do
    if [ "$i" != "." -a "$i" != ".." ];
    then
        echo "Handling $i"
        owner="$(stat --format "%U" ./$i)"
        if [ "${owner}" = "bandit23" ]; then
            timeout -s 9 60 ./$i
        fi
        rm -f ./$i
    fi
done


bandit23@bandit:~$ mkdir -p /tmp/secttp
bandit23@bandit:~$ cd /tmp/secttp
bandit23@bandit:/tmp/secttp$ ls -l
total 52
-rw-r--r-- 1 bandit23 root    4 Sep 24 15:03 myname
-rw-rw-rw- 1 bandit23 root    0 Sep 20 22:37 pas
-rw-rw-rw- 1 bandit23 root   33 Sep 20 16:09 passs
-rw-rw-rw- 1 bandit23 root   33 Sep 25 16:20 password
-rw-r--r-- 1 bandit23 root 4435 Sep 19 00:14 pincode.py
-rw-r--r-- 1 bandit23 root 4415 Sep 19 00:15 pinsa.py
-rw-r--r-- 1 bandit23 root    0 Sep 17 12:30 ppassword
-rwxrwxrwx 1 bandit23 root   64 Sep 20 16:06 p.sh
-rw-r--r-- 1 bandit23 root   66 Sep 24 15:09 secctp.sh
-rwxr-xr-x 1 bandit23 root   54 Sep 20 05:13 sectp.sh
-rw-r--r-- 1 bandit23 root    2 Sep 24 15:06 secttp
-rwxrwxrwx 1 bandit23 root   66 Sep 25 13:35 secttp.sh
-rw-r--r-- 1 bandit23 root    2 Sep 24 15:02 whoami

bandit23@bandit:/tmp/secttp$ touch secttp.sh
bandit23@bandit:/tmp/secttp$ chmod 777 secttp.sh
bandit23@bandit:/tmp/secttp$ ls -al secttp.sh
-rwxrwxrwx 1 bandit23 root 66 Sep 26 18:52 secttp.sh

andit23@bandit:/tmp/secttp$ nano secttp.sh 
Unable to create directory /home/bandit23/.nano: Permission denied
It is required for saving/loading search history or cursor positions.

Press Enter to continue

#!/bin/bash

cat /etc/bandit_pass/bandit24 > /tmp/secttp/password


bandit23@bandit:/tmp/secttp$ touch password 
bandit23@bandit:/tmp/secttp$ chmod 666 password 
bandit23@bandit:/tmp/secttp$ ls -la password 
-rw-rw-rw- 1 bandit23 root 33 Sep 26 18:57 password

bandit23@bandit:/tmp/secttp$ cp secttp.sh /var/spool/bandit24/
bandit23@bandit:/tmp/secttp$ ls -al /var/spool/bandit24/secttp.sh
-rwxr-xr-x 1 bandit23 bandit23 66 Sep 26 18:59 /var/spool/bandit24/secttp.sh
bandit23@bandit:/tmp/secttp$ ls -al password
-rw-rw-rw- 1 bandit23 root 33 Sep 26 18:57 password
bandit23@bandit:/tmp/secttp$ cat password
UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ
********************************
Bandit Level 24 → Level 25
Level Goal
A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.

***************************************************************************************

Solution of level 24 -> 25

kali@kali:~$ ssh bandit.labs.overthewire.org -l bandit24 -p2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit24@bandit.labs.overthewire.org''s password: UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ

bandit24@bandit:~$ nc localhost 30002
I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.
Timeout. Exiting.

bandit24@bandit:~$ cd /tmp/
bandit24@bandit:/tmp$ nano basher.sh
Unable to create directory /home/bandit24/.nano: Permission denied
It is required for saving/loading search history or cursor positions.

Press Enter to continue

#!/bin/bash

pass="UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ"
for i in {1000..10000}
do {
if
    echo $pass $i| nc localhost 30002 | grep Wrong > /dev/null
then
    echo $i
else
    echo $pass $i| nc localhost 30002
    exit
fi
}
done

////////////////////////////////////////////////////

#!/bin/bash

password=$(cat /etc/bandit_pass/bandit24)

for i in $(seq -w 9999); 
do
    echo "$password $i" | nc localhost 30002 
done

////////////////////////////////////////////////////

#!/bin/bash
passwd="UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ"

for a in {0..9}{0..9}{0..9}{0..9}
do
    echo $passwd' '$a | nc localhost 30002 >> result &
done

/////////////////////////////////////////////////////


bandit24@bandit:/tmp$ ./basher.sh
**********************************
