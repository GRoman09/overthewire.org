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

![image](https://user-images.githubusercontent.com/96256687/147137280-fed919f4-92b5-48cf-97df-dca4ad08cfc3.png)

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

![image](https://user-images.githubusercontent.com/96256687/147136873-85064332-a545-4c32-90b7-c81f35edde9e.png) 

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

![image](https://user-images.githubusercontent.com/96256687/147138841-5a6ba0a8-c0f1-4b03-a2fc-06831d92e58f.png)

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

![image](https://user-images.githubusercontent.com/96256687/147140170-3731cc78-d08e-411c-aac1-07fb6c643221.png)

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

![image](https://user-images.githubusercontent.com/96256687/147141150-98504f3f-a5c9-49bd-8833-33f087a8989a.png)

#Execution option 2

![image](https://user-images.githubusercontent.com/96256687/147141382-ca6441e9-7247-4acf-8aa9-e033165a22ef.png)

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

#Execution option 1

![image](https://user-images.githubusercontent.com/96256687/147389882-bd6cc002-0ac0-4f4d-af71-47525aff8327.png)

#Execution option 2

![image](https://user-images.githubusercontent.com/96256687/147389929-d448d0df-988a-4f52-b466-b55bd947655d.png)

#Execution option 3

![image](https://user-images.githubusercontent.com/96256687/147390002-8bfa3b88-ecfc-4d19-87d8-df281cc7836d.png)

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

bandit6@bandit.labs.overthewire.org's password: DXjZPULLxYr17uwoI01bNLQbtFemEgo7

#Execution option 1

![image](https://user-images.githubusercontent.com/96256687/147390017-46f10e34-0e9f-4b90-9e70-a871d38eec62.png)

#Execution option 2

![image](https://user-images.githubusercontent.com/96256687/147390042-0f9728b5-9703-4c18-bea6-39cbe2599a09.png)

#Execution option 3

![image](https://user-images.githubusercontent.com/96256687/147390269-aa24739a-6222-4da5-b3ed-5320fed818b4.png)

#Execution option 4

![image](https://user-images.githubusercontent.com/96256687/147390326-d61e1e8d-4450-47b4-83d9-4cb4f4792735.png)

HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs 
********************************

**Bandit Level 7 → Level 8
--------------------------
Level Goal

The password for the next level is stored in the file data.txt next to the word millionth

Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
************************************************************
Solution of level 7 -> 8

~$ ssh bandit.labs.overthewire.org -l bandit7 -p2220

bandit7@bandit.labs.overthewire.org's password: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

#Execution option 1

![image](https://user-images.githubusercontent.com/96256687/147390414-340c4aa9-2753-477e-a993-5754ffed7a86.png)

#Execution option 2

![image](https://user-images.githubusercontent.com/96256687/147390436-45b3aaa3-a338-48b3-830d-dc67d08095e2.png)

cvX2JJa4CFALtqS87jk27qwqGhBM9plV
************************************************

**Bandit Level 8 → Level 9
--------------------------
Level Goal

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

Helpful Reading Material

Piping and Redirection
*************************************************************

Solution of level 8 -> 9

~$ ssh bandit.labs.overthewire.org -l bandit8 -p2220

bandit8@bandit.labs.overthewire.org's password: cvX2JJa4CFALtqS87jk27qwqGhBM9plV

#Execution option 1--3

![image](https://user-images.githubusercontent.com/96256687/147390871-032bac38-a4ca-47c1-be13-6d9a73696b55.png) 

UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
********************************

**Bandit Level 9 → Level 10
---------------------------
Level Goal

The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
*************************************************************

Solution of level 9 -> 10

~$ ssh bandit.labs.overthewire.org -l bandit9 -p2220

bandit9@bandit.labs.overthewire.org's password: UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

#Execution option 1

bandit9@bandit:~$ grep -a == data.txt

...===== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

#Execution option 2

bandit9@bandit:~$ strings data.txt | grep -E '=+'

![image](https://user-images.githubusercontent.com/96256687/147391434-042ce6cf-45f3-44ae-96ca-e63b2391821b.png)

truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
********************************

**Bandit Level 10 → Level 11
----------------------------
Level Goal

The password for the next level is stored in the file data.txt, which contains base64 encoded data

Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

Helpful Reading Material

Base64 on Wikipedia
*************************************************************

Solution of level 10 -> 11

~$ ssh bandit.labs.overthewire.org -l bandit10 -p2220

bandit10@bandit.labs.overthewire.org's password: truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

#Execution option 1

![image](https://user-images.githubusercontent.com/96256687/147391539-5238c3c6-78cc-42d2-9b4f-08a1beee0a8c.png)

#Execution option 2-3

![image](https://user-images.githubusercontent.com/96256687/147391576-798ffc3e-8808-4282-a6e8-8b28c92e36b6.png)

IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
********************************

**Bandit Level 11 → Level 12
----------------------------
Level Goal

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

Helpful Reading Material

Rot13 on Wikipedia
************************************************************

Solution of level 11 -> 12

~$ ssh bandit.labs.overthewire.org -l bandit11 -p2220

bandit11@bandit.labs.overthewire.org's password: IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

#Execution option 1

![image](https://user-images.githubusercontent.com/96256687/147414754-822b629c-ab55-477f-984c-4a595bfce112.png)

5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
********************************

**Bandit Level 12 → Level 13
----------------------------
Level Goal

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd, mkdir, cp, mv, file

Helpful Reading Material

Hex dump on Wikipedia
************************************************************************************

Solution of level 12 -> 13 

~$ ssh bandit.labs.overthewire.org -l bandit12 -p2220

bandit12@bandit.labs.overthewire.org's password: 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

#Execution option 1

![image](https://user-images.githubusercontent.com/96256687/147415469-58c1ce7c-334b-47ce-86b5-e1914cc20f0e.png)

#Execution option 2

![image](https://user-images.githubusercontent.com/96256687/147415633-d0ba7fec-136a-4e1b-a85a-fc7f5d20b53d.png)

The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
******************************************************

**Bandit Level 13 → Level 14
----------------------------
Level Goal

The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

Commands you may need to solve this level

ssh, telnet, nc, openssl, s_client, nmap

Helpful Reading Material

SSH/OpenSSH/Keys

******************************************

Solution of level 13 -> 14

~$ ssh bandit.labs.overthewire.org -l bandit13 -p2220

bandit13@bandit.labs.overthewire.org's password: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

![image](https://user-images.githubusercontent.com/96256687/147416394-b8c136eb-f8af-44eb-adab-addbbca31723.png)

![image](https://user-images.githubusercontent.com/96256687/147416425-1d8abd11-5e09-4e2a-bf2b-f10de886454a.png)

4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
********************************

**Bandit Level 14 → Level 15
----------------------------
Level Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

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

bandit14@bandit.labs.overthewire.org's password: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

![image](https://user-images.githubusercontent.com/96256687/147416613-83504220-1b1e-4564-aefc-aed9ee61a5dd.png)

BfMYroe26WYalil77FoDi9qh59eK5xNr
********************************

**Bandit Level 15 → Level 16
----------------------------
Level Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.

Helpful note: 

Getting “HEARTBEATING” and “Read R BLOCK”? 

Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. 

Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command…

Commands you may need to solve this level

ssh, telnet, nc, openssl, s_client, nmap

Helpful Reading Material

Secure Socket Layer/Transport Layer Security on Wikipedia

OpenSSL Cookbook - Testing with OpenSSL
**********************************************************

Solution of level 15 -> 16

~$ ssh bandit.labs.overthewire.org -l bandit15 -p2220

bandit15@bandit.labs.overthewire.org's password: BfMYroe26WYalil77FoDi9qh59eK5xNr

#Execution option 1

![image](https://user-images.githubusercontent.com/96256687/147494832-5d564399-fb99-4e5a-a218-79b79ad73fb6.png)
![image](https://user-images.githubusercontent.com/96256687/147494904-dcd91e5c-831a-4f93-88db-6558b2fbc2e4.png)

#Execution option 2

![image](https://user-images.githubusercontent.com/96256687/147495141-547ebe29-5bdf-45ff-9842-50e9cf77cb28.png)

#Execution option 3

![image](https://user-images.githubusercontent.com/96256687/147495228-55491470-f981-4e40-a7e5-a2c2b443b286.png)

#Execution option 4

![image](https://user-images.githubusercontent.com/96256687/147495292-2ed17b65-9d44-4eb6-9db0-fda6af25052b.png)

#Execution option 5

![image](https://user-images.githubusercontent.com/96256687/147495349-236d788b-8dfa-4d99-92f5-38ba42464d81.png)

#Execution option 6

![image](https://user-images.githubusercontent.com/96256687/147495478-cdba8769-7a94-48a9-bf78-c7b6ad906425.png)
![image](https://user-images.githubusercontent.com/96256687/147495514-35497cec-f7d5-4b81-beee-e5ebc3787b83.png)

cluFn7wTiGryunymYOu4RcffSxQluehd
*********************************

**Bandit Level 16 → Level 17
----------------------------
Level Goal

The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. 

First find out which of these ports have a server listening on them. Then find out which of those speak SSL and which don’t. 

There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

Commands you may need to solve this level

ssh, telnet, nc, openssl, s_client, nmap

Helpful Reading Material

Port scanner on Wikipedia
******************************************

~$ ssh bandit.labs.overthewire.org -l bandit16 -p2220

bandit16@bandit.labs.overthewire.org's password: cluFn7wTiGryunymYOu4RcffSxQluehd

#Execution option 1

bandit16@bandit:~$ nmap localhost 

![image](https://user-images.githubusercontent.com/96256687/147496634-7873ec57-49ce-43b9-a30e-8cb1383a16b0.png)

![image](https://user-images.githubusercontent.com/96256687/147496709-9cf25e2a-0a4f-454e-94dd-1fae12b2b7ad.png)

![image](https://user-images.githubusercontent.com/96256687/147496953-247e884d-3aaf-455c-957d-3dfd417946a8.png)

![image](https://user-images.githubusercontent.com/96256687/147497038-3bd10b07-315f-4c19-ad3a-ede6821a60d7.png)

#Execution option 2

![image](https://user-images.githubusercontent.com/96256687/147497832-006d5676-de33-4c31-a0f5-5832ab5ac55b.png)

![image](https://user-images.githubusercontent.com/96256687/147497875-db192a6a-4b0e-49ca-b9f9-ef3a6af30d0c.png)

xLYVMN9WE5zQ5vHacb0sZEVqbrp7nBTn
************************************************

**Bandit Level 17 → Level 18
----------------------------
Level Goal

There are 2 files in the homedirectory: passwords.old and passwords.new. 

The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19

Commands you may need to solve this level

cat, grep, ls, diff
*****************************************

Solution of level 17 -> 18

~$ ssh bandit.labs.overthewire.org -l bandit17 -p2220

bandit17@bandit.labs.overthewire.org's password: xLYVMN9WE5zQ5vHacb0sZEVqbrp7nBTn

#Execution option 1-2

![image](https://user-images.githubusercontent.com/96256687/147498430-0c65cf39-4472-4b4a-8d09-d302c7252575.png)

kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
********************************

**Bandit Level 18 → Level 19
----------------------------
Level Goal

The password for the next level is stored in a file readme in the homedirectory. 

Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

Commands you may need to solve this level

ssh, ls, cat
*****************************************

Solution of leve 18 -> 19

#Execution optoin 1

![image](https://user-images.githubusercontent.com/96256687/147498726-f471a64c-bb09-43c5-a7bf-e8eb920a497d.png)

bandit18@bandit.labs.overthewire.org's password: kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd

#Execution optoin 2

![image](https://user-images.githubusercontent.com/96256687/147498850-0ae2093f-23cc-4476-98df-0172a9d060f6.png)

#Execution option 3

![image](https://user-images.githubusercontent.com/96256687/147498969-4d97cf40-7016-4dd4-965f-60eafcea7703.png)

IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x
********************************

**Bandit Level 19 → Level 20
----------------------------
Level Goal

To gain access to the next level, you should use the setuid binary in the homedirectory. 

Execute it without arguments to find out how to use it. 

The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

Helpful Reading Material

setuid on Wikipedia
************************

Solution of level 19 -> 20

~$ ssh bandit.labs.overthewire.org -l bandit19 -p2220

bandit19@bandit.labs.overthewire.org's password: IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

![image](https://user-images.githubusercontent.com/96256687/147855987-a7109ce8-0bca-4212-b74c-98eeaaadc60a.png)

GbKksEFF4yrVs6il55v6gwY5aVje5f0j
********************************

**Bandit Level 20 → Level 21
----------------------------
Level Goal

There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. 

It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). 

If the password is correct, it will transmit the password for the next level (bandit21).

NOTE: Try connecting to your own network daemon to see if it works as you think

Commands you may need to solve this level

ssh, nc, cat, bash, screen, tmux, Unix ‘job control’ (bg, fg, jobs, &, CTRL-Z, …)
**********************************************************************************

~$ ssh bandit.labs.overthewire.org -l bandit20 -p2220

bandit20@bandit.labs.overthewire.org's password: GbKksEFF4yrVs6il55v6gwY5aVje5f0j

#Execution option 1

![image](https://user-images.githubusercontent.com/96256687/147856370-1288b517-aefc-4394-81a8-e9ad6bdf5441.png)



#Execution option 2

![image](https://user-images.githubusercontent.com/96256687/147856489-c1ec4c66-21d8-4e22-8db1-eaf24f5850d5.png)

gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr
***************************************

**Bandit Level 21 → Level 22
----------------------------
Level Goal

A program is running automatically at regular intervals from cron, the time-based job scheduler. 

Look in /etc/cron.d/ for the configuration and see what command is being executed.

Commands you may need to solve this level

cron, crontab, crontab(5) (use “man 5 crontab” to access this)
**************************************************************

Solution of level 21 -> 22

~$ ssh bandit.labs.overthewire.org -l bandit21 -p2220

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

**Bandit Level 22 → Level 23
----------------------------
Level Goal

A program is running automatically at regular intervals from cron, the time-based job scheduler. 

Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: Looking at shell scripts written by other people is a very useful skill. 

The script for this level is intentionally made easy to read.

If you are having problems understanding what it does, try executing it to see the debug information it prints.

Commands you may need to solve this level

cron, crontab, crontab(5) (use “man 5 crontab” to access this)
**************************************************************

Solution of level 22 -> 23

~$ ssh bandit.labs.overthewire.org -l bandit22 -p2220

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

**Bandit Level 23 → Level 24
----------------------------
Level Goal

A program is running automatically at regular intervals from cron, the time-based job scheduler. 

Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: This level requires you to create your own first shell-script. 

This is a very big step and you should be proud of yourself when you beat this level!

NOTE 2: Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…

Commands you may need to solve this level

cron, crontab, crontab(5) (use “man 5 crontab” to access this)
**************************************************************

Solution of level 23 -> 24

~$ ssh bandit.labs.overthewire.org -l bandit23 -p2220

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

**Bandit Level 24 → Level 25
----------------------------
Level Goal

A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. 

There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.
***************************************************************************************

Solution of level 24 -> 25

kali@kali:~$ ssh bandit.labs.overthewire.org -l bandit24 -p2220

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
