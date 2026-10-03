# Git set up 
- `when you created new git repository in git hub we set up in local system
## Follows Steps
- `1` : Create Repository in gitHub, then clone the in to local system
- `2` : git clone <<provide URL> then presee enter
- `3` : create files what we require
## Add into workingrea
- `git status`
- `git add <File Name>`
- `git status`
- `git add <file Name>`
- `git commit -m provide required massage in duble`

**You can stage tracked modified files and commit them in a single command using the**
- git commit -am "Your Commit Massage"
 - `a --all`    :Automatically stages all files that have been **modified** or **deleted**
 - `m Specifies`: the commit message directly inline

**You can create custome command  in your Globle Git  configuration so you only have to type a single short command**

- `git config --global alias.sync '!git pull && push'`

## Please  use git pull before push
## Whenever we use  # git push -u origin main first time we get error  
# How to resolve this error 
  - **Check repository in our system whic repository we are**
  - **git remote -v**

## git remote set-url origin https://YOUR_TOKEN@github.com/gvckai/My-Note-Book.git
- Syntax: # git remote set-url origin https://YOUR_TOKEN@github.com/github-user-name/Repository-name.git

# Who are stakeholders

- Family : Everyone part of the system are stackholders
             Evwryone of us should be happy
- Bank: stackhilder fot bank , customers, employees, management and leadership,        investore, RBI, IT deporment, marketing, sales operation, security team, admin teams, partners, etc.. 

**Schools** : 
         -  Students, Teachers staff, Non teaching Staff, Leadership, Investers, Edication Deportment etc.

**DeoOps**
         - Teammembers, Management, Developers Testing Team, Operation Team, Admin Team,

## SDLC -> Software Develipment Lifecicle
 - client Perspective
 - End user perspective 

# Why we need  Multiple environments?
- DEV Env
- QA Env
- SIT Env
- UAT Env
- PRE-PROD Env
- PERF Env- Porfamence  
- SEC  Env
- PROD Env
** DevOps Team Main Resposibles Only two things**
 - 1 Faster realses 
 - 2 Less defects 
** When we join New organization we should understand their process
    - Understand their process
    - Work with the process
    - Do a simple POC -> Proof of concepts 
    - Impliment in DEV, SIT, UAT
    - Take it PROG
- we should not complain above new organisatio approch based on theit requirement they build up 

# Agail Process

- Sprints
    - Sign-Up and Signin - Authontication and Authoraization
    - Product Calalogue
    - Cart
    - Order Management
    - Payment Module
    - Tracking System
    - Delivery Module

# Agile with DeOps

**One Month sign up and sign in**
- ## First Day
  - **Developers develops Enter Your First Name**
  - **Developers devlops Enter Your Last Name**
## Test the application daily base

**DevOps Team should keep the application highly available , autoscale, and Security, Cost Optimisation**
## What is Computer

**A Device which has cpu RAM, Storage and OS is called Computer we can assigin  IP**
   
- **Laptop --> Personal Use**

- **Server --> To host Application**
    
- **Mobile --> to calling**

- **There two type of distribution/flavours in Linux**
 - *Enterprise* **immediate support**
 - *Community Edition* **Free Edition : No Support** 
 - *RedHat == CentOs == AllmaLinux == AWS Linux*

 - ## Before creating Server in any cloud like AWS AZURE and GCP first Create Create Security Groups
  - **You can call Security groups or Firewall**
   - There are two type of tafics 
    - Ingress *Incoming trafic*
    - Egress *Out going trafic* **We will allow everyone mostly**

- ## Clint Server Architecture : **Dily Doing DevOps**
 - Any how big problem comes in client server: here only solve 
 - if you can not access server are application
   - First check with Intenet
   - Second DNS problem may be
- **Server Problems**
 - 500 error in github outage
 - internal server erro
## How to work internet
 -  - it will work with submerain cable
 ## Who is server , Who is client

 ## Authentication mechanism
 - **What you know** : User Name and Password -less Secure
 - **What you have** : User Name and OTP / Keys
 - **What you are** : Fingurprint, retina plam - Most Secure
 
 - `pwd` : it prints Present working directory `home/vijay$` 
 - `cd` : is is used to change directory `cd /home/vijay` -`/home/vijay$` 
 ## If you want create/generate kyes
  - `ssh-keygen -f devsecops` :provie *filename what we want* **It will create /generate  keyes public and pravite**
  - ssh : Secure shell, this is one protocall port no **22**
  - Publick Key and Pravite Key locatis is  

  - ## Absolute Path: from the begining *cd /c/home/vijay*
  - ## Relative Path: from the current location *cd vijay*
  - ## How to connect server *ssh -i my pravite kay username@ip address* 
  - ## How to find user # *whoami*
  - ## How to find user id information# *id* it shows user nsme and user id , group name group id 
  - ## How to find which os we use# *uname* **command it will print system information**

  # CRUD - 
     - Create 
     - Read 
     - Update 
     - Delete
## in Linux 
 - Creating Files / Folders
 - Read Files / Folders
 - Update File / Folder
 - Deletin Files / Folders 
## How to create empty file 
 - ``touch filename``: it creates empty file 
## if you want to see the files and Folder/ Directories
 - ``ls`` : It isits the file and folders 
 - ``ls -l`` it lists subdirectories in leanthy format
 - ``ls -a` it prits all files including hidden file
 - ``ls -lr` It prints revers alphabitical order
 - ``ls -t` it prints lonlenth wit time
 -``ls -ltr`` 
## How to create directory
 - ``mkdir`` it command is used to create directory
## How to enter data in to file 
 - **cat > filename > enter > enter the text in the file > enter > ctrl+d-save and  the text in to file**
 - **cat >> filename | press Enter | Provide / Enter the text in existing file |press Enter | Ctrl + d** 
  - Cat commend is used to read the file
 - ``cp`` copy the file 
 - **scp** This command is used to copy files directly two Linex server
  - `scp` : **Secure Copy Protocol**
- **scp -r** : copy the entire directory with files securely 
    - rsync is faster than scp for large transfers because it compresses data and can resume interrupted downloads/uploads
- `If you used custom ssh  port use **scp -p 2222 /path/to/file username@server name /destination IP address**
- *syntax* : `scp -r /path/local/foldername user@ip addess:/path/to/remote/destination/`
 - **If you want to copy file with directory we  : `-r` means recursive**
 - **If you want cut / rename  the to the file we use `mv` command we use ` mv old file name new file name `mv** **source and destination**
 - **cd .. - one step back**

 ## How to downlode file / folder 
 - if you want to download files and folder by using `wget provide URL`
 - If you use `cutl` command it will show on the screen itself fron the internet
   - curl command is used in scripting and api
   - if you wan to see the content in the spot we use `cutl`
- **If you want to search the perticuler ward in the file**
    - `grep word name file name`
    - `cat filename | grep word name`
- If you want to search content in the file , we use **grep** command
    - *Syntax: cat password | grep linux*
    - *Syntax: cat /etc/passwd | grep -i Ramesh* # -i forgot case insensitive, It prints all wheater is is upper case and lower case
       **i = K in-senstive**
    - *Syntax: cat /etc/passwd | grep -in ramesh*# -n it prints line number in which line the word we search, if you want to line number 
    - *Syntax: cat /etc/passwd | grep -inc ramesh* **it prints word , how many time it comes `C - Count the word in the file`cat /
    - *Syntax: cat README.md | grep -iv* : It print verbose , it is used to print oposit word 
## head command
 - $head file name
      - **$ head README.md** : It prints 10 lines of the top by default 
      - **$ tail README.md** : It prints 10  lines of bottem  by default
**If you want to see particular lines like top 4 lines**
  - **-I** case insencitive 
  - **-v** : It will display whole words instead of selecting word 
  - cat /etc/passwd | grep ramesh -in : It prints with line number
  **-i : case insensitive**
  **cat README.md | grep -in Linux**
  **-n : It prints line numbe  whic line it is** *where linux word is not there*
  **-c : Count of finds**
  # Head Command 
   - head command it print top 10 lines bydefault
   - $ head -n3 : it prints top 3 lines 
    # session-6
## Backed Applications
 - Youthink Chef 
   - Java
   - .Net
   - Python
   - Groovi
   - Php
   All these conneted to database, i will do the CRUD Oparation
## Frontend Application
 - Waiter
   - HTML
   - CSS
   - JS
   - ReactJS
   - NodeJS
## Database 
- MS SQL
- MY SQL
- Postgress
- Oracle
- Kafka
## How to Seee How many user 
- **$ cat /etc/passwd** - It prints all users 
## Interview Qation How to prnt users name?
- ** First we shoud cut and 
   - Cut -d ":" f1 and file name
     - cut -d ":" -f1 /etc/passwd
       - d is dilimiter
       - f fragmentcut 
   - $cut -d ":" -f1,2 /etc/passwd
   - $cut -d ":" -f1 /etc/group-It prints group only
**For Example is URL :https://github.com/daws-92s/concepts/blob/main/04-linux.md
  - $ echo "https://github.com/daws-92s/concepts/blob/main/04-linux.md"-: **What ever we give, it print on terminal**
  - $ echo $ echo "https://github.com/daws-92s/concepts/blob/main/04-linux.md" | cut -d "/" -f8
## awk command very importent in shell scripting
 - here F is delimiter 
  - $ `echo "https://github.com/daws-92s/concepts/blob/main/04-linux.md" |awk -F "/" '{print $NF}'`
    - **04-linux.md**
 - `awk -F ":" '{print $1F}' /etc/passwd` ** It prints user names in passwd file
 - `id ramesh | awk -F " " '{print $1F}'`
 **0-999 call it as System Users,** It is not humen users
 **from 1000, there are manually created user**
## Interview Quation
   **We need manually created user, how to fech them please write it**
    - `$ awk -F ":" '$3 <= 999 {print $1,$3F}' /etc/passwd`
## Print manually created users
 - `awk -F ":" '$3 >= 1000 {print $1,$3F}' /etc/passw`
 **Group**
 - `$ awk -F ":" '$3 >= 1000 {print $1,$3F}' /etc/group`
 - `$ awk -F ":" '$3 <= 999 {print $1,$3F}' /etc/grou`
## By using aws command, we process the text what we like
## .tar.gz
 - tar -czf
  - c for creating
  - z for zip formating
  - f for file
## Never use rm -rf *
**tar -czf zipfilename with .gz and give filevame**
- `$ tar -czf backup-02-10-2026.gz 04-linux.md dir`
**Extact the filer from zip format**
 `tar -xzf backup-02-10-2026.gz` : **x means extract**
**If you want to see the files in zip without zipping"**
 - `$ tar -tzvf backup-02-10-2026.gz`
 -  **-t, --list                 list the contents of an archive**
 -  **-v, --verbose              verbosely list files processed**
 # Editors vim - Visually improved editor
 ## VIM Editor
  - command mod 
   - **:wq** - write and quit
   - **:q** - quit
   - **:q!** - fource quit- without saving

   - 
  - There are three more vim edito
   - Esc mode
   - Command mode
   - insert mode
**when you create file wit vim, it is open in Esc mode defaultly**
 - if you want to go command mode - press **:** 
 - if you want to go insert mode - press **i** if it is Esc mode, if it is command mod press **Esc** and **i**
 ## if you want to delete wntair content in vi edito 
 - **:%d**
 # importent things
## User Management
**There are two types of users in Linux**
-  $-dinots Narmal user
-  #-de=dinots super/root user 
- Super user home directory is **root**
-  If you want admin access **sudo su -**
**If you want to uper power $ sudo su - you can enter into root user**
 - /root : root user home directory
 - /home/user-name
 - /home/ec2-user
 - user means one human
 - group a list of human / have one or more user
 ## Authantication and Autherization 
  - **Authenticati means prove your self**?
  - **Autherization means, do you have access to the resource?**
  - **Role      ->   Permission**
  - **Ttainee   -> Read only permission**
  - **Junior    -> write access**
  - **Senior    -> Read, Write, Update**
  - **TL        -> Read, write, update and Delete**

  ## I will create some groups
    - **devops-trainee**
    - **devops-Junior**
    - **devops-senior**
    - **devops-leam lead*
**why is group : for the fxibility**
- A group will have role 
  - **Create User** `
  - **add him into devops group**
  **If you want to create we need admin access**
    - `useradd user-name
      - where is user information **etc/passwd** this is user information location
## When you create user, Linux will create a group also ont he same user name
 - **A user in Linux will have one primary group and 0 or more secondary groups**
  - `#: useradd remesh` - it is used to create user - **root user has permission to create users**
  - `id ramesh` - uid=1001(ramesh) gid=1001(ramesh) groups=1001(ramesh): **it print user id group id others id**
  - **user must have, one primary group** 
    - **If user id is zero, that meaning root user**
   - #id - **It prints root user or current user**
     - `uid=0(root) gid=0(root) groups=0(root) context=unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023`
        - Narmal user home folder is **/home/ramesh**
         - **cat /etc/passwd | grep  ramesh** - ramesh:x:1001:1001::**/home/ramesh:**/bin/bash
             
- **If you want to create group**
 - `groupadd devops` - **It is used to create group**
 - `groupdell devops` - **It is used to delete group**
  - how to to see the group user information
    - **cat /etc/group** - it prints group names
- **I want to add devops group to ramesh user**
  - usermod -g <groupname> <username> **adding user to primary group**
   - usermod -g  devops ramesh
    - `id ramesh` - uid=1001(ramesh) gid=1002(devops) groups=1002(devops)
   - small **-g** means primary group
- **If you want to add secondary group devops-trainee to the ramesh**
 - `usermod -aG secondary group name and username
  - **-a** append
  - **G** Secondary group
**if you want to give primery access, you can add secondary group**
**How to assign passwor to the user**
 - **passwd username** - It is user to asign password to the user
  - `passwd ramesh` provide the password to set the password
   - if you want to connect to the server we required password to user
  - we should do small configaration on configaration file **vim /etc/ssh/sshd_config**
   - PasswordAuthentication no **you need cahnge in to yes** then only it will allow password authentication 
     `PasswordAuthentication yes`
   - PermitEmptyPasswords no
   **while i am modifing vim /etc/ssh/sshd_config**
   `E325: ATTENTION` Found a swap file by the name "/etc/ssh/.sshd_config.swp"
          owned by: root   dated: Sat Oct 03 01:39:54 2026
         file name: /etc/ssh/sshd_config
          modified: no
         user name: root   host name: ip-172-31-45-226.ap-southeast-2.compute
        process ID: 31345 (STILL RUNNING)
While opening file "/etc/ssh/sshd_config"
             dated: Sat Oct 03 01:44:45 2026
      NEWER than swap file!

(1) Another program may be editing the same file.  If this is the case,
    be careful not to end up with two different instances of the same
    file when making changes.  Quit, or continue with caution.
(2) An edit session for this file crashed.
    If this is the case, use ":recover" or "vim -r /etc/ssh/sshd_config"
    to recover the changes (see ":help recovery").
    If you did this already, delete the swap file "/etc/ssh/.sshd_config.swp"
    to avoid this message.`
  **It is showing error li process ID: 31345 (STILL RUNNING)**
  **I solved like This by using Kill command**
  **check if another terminal session or user is currently editing the file:**
  
  - ps -aud process ID
  - `sudo ps aux | grep 31345` find the process and kill process
  **If the process is active in another session: Switch to that terminal or exit Vim safely there**
  - `sudo kill -9 31345`
## Step 2: Compare the swap file with the current file
 - Before recovering or deleting anything, check if the swap file contains changes you care about:
  - sudo vim -r /etc/ssh/sshd_config
   - if you want the swap file's changes: Save and exit (:wq).
   - if you don't need the swap file's changes: Quit without saving (:q!).

