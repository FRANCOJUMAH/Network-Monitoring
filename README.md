# Network Monitoring using ManageEngine OpManager


## 🎯 Task Overview

![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/af269e244648de0acd39223ab4f1dd0f1583f333/imgs/OpManager.jpg)

- **This lab entails Monitoring Networks, Servers, Virtualization, Storage, Applications**
-  _The tool in use here is ManageEngine OpManager running on a Linux Environment_
-  _Project Requirements : Linux Environment either running as a VM or a guest Os, ManageEngine installer and working networking environment_ 


## 📝 Background check

1. Environment Setup
- Host Machine: Oracle VirtualBox running Kali Linux VM

- Networking: Two subnets configured for monitoring (e.g., 192.168.1.0/24 and 192.168.2.0/24)

Requirements:

- ManageEngine OpManager installer (.bin file)
  Here you can get the installation files for different platforms - https://www.manageengine.com/download.html

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
   _Web Client - 8060 & 8061,
   Postgres - 13306,
   SSHD -     22,
   TFTP - 69, 
   Syslog - 514_

 ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/b4aa96d2af82b25ad91e05fa1938e6c2ce5696d0/imgs/Engine08.jpg)
 
 ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/b4aa96d2af82b25ad91e05fa1938e6c2ce5696d0/imgs/Engine09.jpg)

 ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/b4aa96d2af82b25ad91e05fa1938e6c2ce5696d0/imgs/Engine10.jpg)

3. **Accessing the Web Console**

- OpManager is now running and is accessible using the web client service running on port 8060 for http and port 8061 for https.
       _https://kali:8061  /    http://kali:8060_
       
 ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/b4aa96d2af82b25ad91e05fa1938e6c2ce5696d0/imgs/Engine11.jpg)
 
- Login with the default credentials after which you will be prompted to change as a security requirement 
 ![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/2f1eda3db2879a20a784e1108a3fa015494c94fc/imgs/Engine12.jpg)

- View Dashboard 
![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/2f1eda3db2879a20a784e1108a3fa015494c94fc/imgs/Engine14.jpg)

- Performance Monitors - below are some metrics you could set in your dashboard to monitor your network infrastructure
![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/2f1eda3db2879a20a784e1108a3fa015494c94fc/imgs/Engine15.jpg) 

- Add Devices : You could add devices using network discovery by setting the subnet correctly and let the system detect available devices
![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/e098ca3eae40178c40da057cd8218a225ac1db0a/imgs/network%20discovery.jpg)

- Added devices (45) , 1 Subnet 
![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/e098ca3eae40178c40da057cd8218a225ac1db0a/imgs/subnet.jpg)

- OpManager Dashboard : You can monitor your infrastructure. Any Alarms either critical or normal can also be previewed here.
- Depending on your preference, you can also go ahead and configure Mail Server to get email notifications incase of an alarm. 

![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/e098ca3eae40178c40da057cd8218a225ac1db0a/imgs/dashboard.jpg)

     _ N/B - This is not the end. There are so many functionalities to unwind in this lab. I hope this doc was instrumental and off help as you go on to set up your lab environment that would go along to help in learning and monitoring your network environments. _
  
                                                                      **Keep Building and Keep Learning**




