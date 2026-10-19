# User Management
- **$** Narmal User /home/ec2-user

- **#** /root user or super user
- user -> a human
- group -> a list of humans a group have one or more user
- authentication (Prove yourself) and authorization ( do you have access to this resource)

**Authorization**

| Role | Permissions |
|---|---|
| Trainee | Read only access |
| Junior | Write and Update Access |
| Senior | Read, Write, and Update Access |
| TL | Read, Write, Update and Delete Access |

A group will have role -> permission
- ramesh > devops-traineesseniors
- devops-juniors
- devops-seniors
- devops-lead
1. Create user
2. add him to devops group
**if you want to create we must have admin access.**
- sudo su - : you will be landed root folder
- useradd ramesh
- groupadd devops

 - when you create usre linux will create a group also on the same user name
 - a user in linux will have 1 primary group and 0 or more secondary group
 - user id = 0 it means root user
 - if you want add ramesh in to devops group
  - usermod  -g group name username  adding user to primary group
  - usermod -g devops ramesh 
- if you add sre secondry group to ramesh
 - usermod -aG sre ramesh
- if you want to give the access temperary you will add as a secondary group
- set password for ramesh
 - passwd ramesh