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
     - Check tha service : systemctl status nginx
     - netstat -lntp | grep nginx
     - ps -ef | grep nginx
      - still there is a proble : then **go and check the logs**