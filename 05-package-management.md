# 5Th day 
## Package Management
- 1. Os Server have URLS to connect internet to fech the objects
- 2. dnf install **package Name**
- 3. yum old version of RHEL
- 4. dnf is latest
- 5. yum is softlink to dnf  
- 6.  /etc/yum.repos.d/    
- 7. dnf remove package name : **is used to uninstall packages and their unneeded dependencies**
     `RPM-based Linux distributions like Fedora, RHEL, CentOS Stream, AlmaLinux, and Rocky Linux.`
     - Remove a single package: **sudo dnf remove httpd**
- 8. if you want to update **dnf update pacakage** exm : **sudo dnf update nginx**
        **refreshes repository metadata and updates installed software packages**
- `dnf search package name :` **to help you find relevant software** `exm:` **dnf search nginx**
- `dnf list installed:` **displays all software packages currently installed on your system.**
- `dnf info git`
     **retrieves detailed metadata about the git package, showing version information, repo origin, size, and package summary for both installed and available versions.**
- `dnf repolist`
- `dnf install nginx`
- `dnf list installed | grep nginx`
- `dnf list installed | grep git`
- `dnf remove ngnix -y`

## Service Magament
- sshd is a service continues running
- https is a service
- nginx is web server this is new and papuler powerful
- apach hhp is also webserver this old
- after installing nginx we start the service 
**systemctl start nginx** -It will start nginx server
- Linux is physical server
- nginx is logical server running in side linux server

- sudo systemctl start `<service>`	Starts a stopped service immediately
- udo systemctl stop `<service>`	Stops a running service immediately
- sudo systemctl restart `<service>`	Stops then starts the service (applies new configs)
- sudo systemctl reload `<service>`	Reloads configuration without dropping active connections
- systemctl status `<service>`	Checks current running state, PID, and recent logs
- sudo systemctl enable `<service>`	Sets service to start automatically at boot
- sudo systemctl disable `<service>` Prevents service from starting automatically at boot
- sudo systemctl enable --now <`service>`	Enables and starts the service in a single command
- sudo journalctl -u `<service_name>` -n 50 --no-pager # View recent logs for a specific service
- sudo journalctl -u `<service_name>` -f # Follow logs in real-time

- - systemctl status nginx : **Unit nginx.service could not be found.**
- - dnf install nginx -y :
- - systemctl status nginx : **Active: inactive (dead)**
- - systemctl start nginx : 
- - systemctl status nginx : **Active: active**
- - systemctl enable nginig : **Sets service to start automatically at boot**


# Network Management
 - Howmay ports are the in system 0 to 65535
     - ssh - 22
     - http -80
     - https - 443
     - mysql - 3306
     - backend -8080
     - SMTP - 25
     - jenkin - 8080
     - DNS -53 
- If you want to know whta ports are oppend
 - netstat -lntp : **lists all active TCP listening ports along with the process names and Process IDs (PIDs) bound to  them, using numerical IP addresses and port numbers.**
     - l : **Show only listening sockets (ports waiting for incoming connections).**
     - n: **Print numerical addresses and port numbers (e.g., 80 instead of http, 127.0.0.1 instead of localhost).**
     - t: **Limit results to TCP sockets.**
     - p: **Display the PID and program/process name owning each socket (requires sudo privileges to see all processes).**
# Interview Quation
 - how to find open ports in the linix system
     netstat -lntp --> **by using this command we can find open ports in the linux server**
 - http://32.236.195.242

 # Processmanagement
  - Eveything is process
## how to find which process are running in linux
 -   ps : **Show processes for current shell session:**
 - If you want to all processes in the linux sys
     - ps -ef **: View ALL processes with full details (UNIX style)**
     - pps aux : **View ALL running processes on the system**
     - ps aux | grep nginx : **Filter output for a specific process**
     - ps -u root : **View processes for a specific user**
# There are two types of process 
 - foreground process- it will block terminal we cont do anythin on termina, 
  - If you want to go to background sleep 10 &
 - background process- 
## If any application is not running
-  **We must check**
     - **Check tha service : systemctl status nginx**
          - **netstat -lntp | grep nginx**
          - **ps -ef | grep nginx**
          - **still there is a problem** : then **go and check the logs**
# Session 06

## Three Tier Architecture
 Raw : Data 
  - Chef : Backend application : (Java, .Net, python, Groovi php etc)
         - **backend applicatins connect with database and do CRUD Operation** *This is Developer Job*
  - Waiter : frontend applications (**HTML, CSS, Java Script, ReactJS, NodeJS**)
          - there are all UI Experiance
  - Captain : Loadbalencer 

  - 1 tier Architecture is every thing is in single server (**Frontend+backend and database**)
   - One Linux Server
# Two tier Architecture
 - 2 linux Servers
# Three Tier Architecture
 - 3 linux Servers
  First we take Lodad balancer go to Fronted go to backend got Database
   - some pleple called web/frontend/HTTP tier (Loadbalancer + frontend)
   - Some people called App/backend / middle ware tier (backend)
   - Somple people called database tier      

# Database Technolagies 
 - MS-SQL
 - MySQL
 - Postgress
 - Oricale
 - Kafka
 - MagoDB 
**Data Base Admin --> Install Data Base, Upgrade, backup, restore, create schema, monitor, scall them Clustring them**
- Install- mysql serve
     - **Install the MySQL 8.0 Community Repository**
     -     sudo dnf install -y https://dev.mysql.com/get/mysql80-community-release-el9-1.noarch.rpm
     - **Import the Official GPG Key (to prevent GPG verification errors):**
          - sudo rpm --import https://repo.mysql.com/RPM-GPG-KEY-mysql-2023
     - **Install the MySQL Server Package:**
          - sudo dnf install -y mysql-community-server
          - systemctl status mysql
          - systemctl start mysqld
          - systemctl status mysqld
          - systemctl enable mysqld
          - netstat -lntp : ****MySql Pot : 3306**
          - ps -ef | grep mysqld
          - sudo grep 'temporary password' /var/log/mysqld.log
            - Copy the passwod safeside
            - mysql -u root -p
             - provide temporary password
             - **change default password** : 
             ```
             mysql> ALTER USER 'root'@'localhost' IDENTIFIED BY 'V@jay*123*';
             ```

             SHOW DATABASES;



# Session07
## Backend Procezer
1. we need to install programming ganduage runtime
2. Create one directory to download the code
3. Download the code 
4. install dependies or libraries

# Install Node.JS
 - by default Node.Js 16 is available on the system enable install version 24
 - dnf module lit nodejs - **list the nodejs version available**
 - dnf list nodejs* 
   - **see which Node.js versions are available in the Amazon Linux 2023 repositories, run:**
- dnf install nodejs -y - `If we install, we dont know which version is installed so`
**Conform the version from the developers** then We should install particuler version
- developer conformed 24 version
## First desible the default version
 - dnf module disable nodejs -y
 - dnf module enable nodejs:24 -y
 - dnf install nodejs -y 
 - My self iI install **dnf install nodejs24.x86_64 -y**
 - Check the version : **node -v**
 ## Set up Application directory
```
   mkdir /app
```
# Create Application User
- **Add a system user to run the application**
- - If we run human or root user to run the application
 1. they may have more access in linux, if one server is compromised, their credentails are leaked
  - once credentials are leaked they can accedd all files and curruped the files
  - here there are more priveleges issues
2. if hacked blast radius is more
3. more files and folder are on human names   
4. what if the human resigns the company - if the application will be runned on his name 
5. if we want to chande the name so here there will be downtime 
6. auditing and accountablity  for this purpus
## instade of running applications or services on human name credentials 
 - **we use system users to limit blast radious and least priveleges**
     - **System user will not have intaractive logins so no credentials, no login, no shell/terminal access also**
# How to create system users:
```
useradd --system --home -d /app --shell /sbin/nologin --comment "expense system user" expense
```
   
```
useradd --system -m -d /app -s /sbin/nologin -c "expense system use" expense
```
  - Check whether expense user is created or no : 
    ```
    cat /etc/passwd |grep  expense
    # expense:x:993:993:expense system use:/app:/sbin/nologin
    ```
     - **--system**       :Creates a system user (UID under 1000) reserved for background processes and services.
     - **-m**	          :Creates the home directory (/app) if it does not already exist.
     - **-d /app**	     : Specifies /app as the custom home directory path.
     - **s /sbin/nologin**: Restricts interactive shell login for safety (standard on Amazon Linux).
     - **-c "expense system user"**	
                         : Adds a comment/description string to the /etc/passwd record.
     - **expense**	     : The username to create.
