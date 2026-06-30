# Network Monitoring using ManageEngine OpManager


## 🎯 Task Overview

![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/af269e244648de0acd39223ab4f1dd0f1583f333/imgs/OpManager.jpg)

- **This project entails Monitoring Networks, Servers, Virtualization, Storage, Applications**
-  _The tool in use here is ManageEngine OpManager running on a Linux Environment_
-  _Project Requirements : Linux Environment either running as a VM or a guest Os, ManageEngine installer and working networking environment_ 


## 📝 Background check

1. Environment Setup
- Host Machine: Oracle VirtualBox running Kali Linux VM

- Networking: Two subnets configured for monitoring (e.g., 192.168.1.0/24 and 192.168.2.0/24)

Requirements:

- ManageEngine OpManager installer (.bin file)

- Root or sudo privileges

- Working network connectivity between VM and monitored subnets
 
_Kali Linux - Linux is running as a virtual machine as shown below_
  ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/810389816d1be622b00d06af49e4d3fa957af3e6/imgs/Kali-Linux.jpg)
  
_Manage Engine Installer bin file in the default downloads folder_
  ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/810389816d1be622b00d06af49e4d3fa957af3e6/imgs/bin%20install.jpg)
 

 
## 📝 Installation Steps

1.  **Open Terminal**
   - Open and run the terminal with root privilege
   - Traverse to the folder with the bin installer and open the terminal,
   - Make installer executable - (chmod +x ManageEngine_OpManager_Free_64bit_GA.bin)
   - Run installer - (./ManageEngine_OpManager_Free_64bit_GA.bin)
   - 
     _Installation is now underway as seen below_
  ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/810389816d1be622b00d06af49e4d3fa957af3e6/imgs/Engine02.jpg)


   _Choose your preferred installation directory_
 ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/2081e6589eb12afecba68e12481488706d0ad3e2/imgs/Engine03.jpg)
 
 ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/2081e6589eb12afecba68e12481488706d0ad3e2/imgs/Engine04.jpg)   

 **Installation complete**
 ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/2081e6589eb12afecba68e12481488706d0ad3e2/imgs/Engine05.jpg)
 


 2.  **Starting the service**
   - Navigate to the bin directory: cd /opt/ManageEngine/OpManager/bin
   - Start OpManager: sudo ./StartOpManagerServer.sh

 ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/2081e6589eb12afecba68e12481488706d0ad3e2/imgs/Engine07.jpg)

 ManageEngine is now running and can be seen with the relevant services loaded and running concurrently as seen below :
   Web Client - 8060 & 8061
   Postgres - 13306
   SSHD -     22
   TFTP - 69 
   Syslog - 514

  
   
