# Network Monitoring using ManageEngine OpManager


## 🎯 Task Overview

![image](https://github.com/FRANCOJUMAH/Network-Monitoring/blob/af269e244648de0acd39223ab4f1dd0f1583f333/imgs/OpManager.jpg)

- **This project entails Monitoring Networks, Servers, Virtualization, Storage, Applications**
-  _The tool in use here is ManageEngine OpManager running on a Linux Environment_
-  _Project Requirements : Linux Environment either running as a VM or a guest Os, ManageEngine installer and working networking environment_ 




## 📝 Project Steps

1. **Created the EC2 Instance (Windows)**
   - Log in to the AWS Management Console (https://signin.aws.amazon.com/), 
   ![image](https://github.com/FRANCOJUMAH/Creating-an-AWS-EC2-Instance-/blob/2efa99f82ef7d9d4d59a3921a3ef55a47846d58a/resources/Console.png)
   - Go to the EC2 Dashboard in the AWS Management Console and click "Launch Instance".
   - Name the instance ("tuko-kadi") and selected a Windows AMI (Microsoft Windows Server 2025 Base).
   - Choose an instance type, such as t2.micro (Free Tier eligible).
   - Create a new key pair, download the .pem file, and store it securely.
   - Under Network Settings, ensure "Auto-assign public IP" is enabled
