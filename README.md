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
- *Server Problems**
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
 ## If you want create/generate ssh kyes by using bellow command 
  - `ssh-keygen -f devsecops` :provide *filename what we want* **It will create /generate  ssh keyes (public and pravite)**
  - ssh : Secure shell, this is one protocall
  - Port no **22**
  - Publick Key and Pravite Key locatis is  

  - Absolute Path: from the begining **cd /c/home/vijay**
  - Relative Path: from the current location *cd vijay*
  - How to connect server **ssh -i my pravite kay username@ip address** 
  - How to find user # **whoami**
  - How to find user id information# **id** it shows user nsme and user id , group name group id 
  - How to find which os we are using# **uname** **command it will print system information**
    - **uname -a** : It print all info of Sys info Like versin, which os, kernal 

<<<<<<< HEAD
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
- *syntax* : `scp -r /path/local/foldername user@ip addess:/path/to/remote/destination/`
 - **If you want to copy file with directory we  : `-r` means recursive
 - **If you want cut / rename  the to the file we use `mv` command we use ` mv old file name new file name `mv **source and destination**
 - **cd .. - one step back**
=======
  # CRUD
>>>>>>> c81a34c6f0ddb5b5810b1664242e26671a5fb47d
