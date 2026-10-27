# ansible 
## Shell disadvantages
 - No idempotency
 - No error handling
 - shell is imperative, commands should be order
 - cant not handle at a scale
 - Homogenous -> works only for specific destro
 - can not store secrets securely
 **ssh ec2-user@172.31.31.45 -C "touch /tmp/devops.txt"
 - non interactive login

 ## Ansible ->  Configuration Manage Ment
  - plain server -> ready to host application

  **each and every thing is configuring the server like**

  1. installing programing language
  2. createing system user
  3. creating app directory
  4. downloading code
  5. unzipping code
  6. installing dependencies
  7. creating systemctl service files 
  8. loading data if necessary
  9. starting the server
  
  **Above these are all Configuration**
    

| Ansible | Chef | Salt Stack |
|---|---|---|
| **The No-Agent & Easy** | **Strict Enterprise** | **The "Lightning-Fast"** |
| **Agentless and Push-based** | **Agent-based and Pull-based.**| **Master-Minion (Agent-based) with Ultra-Fast Messaging**|