# Ajira Cloud Computing Project


## 🎯 Task Overview

![image](https://github.com/FRANCOJUMAH/EC2-Instance-RDP-Project/blob/a28a5e4d5e8199f5405c1114de3e82c93bcb1a18/images/ec2%20rdp.png)

- **This project entails launching a Windows EC2 instance, enabling Remote Desktop Protocol (RDP) access via security groups, and configuring Amazon Cloudwatch for Monitoring & Amazon SNS to send notifications.**
-  _Create an RDP server, configure network security, and use Cloudwatch & SNS to monitor or alert on instance state changes (e.g., stopping/starting) for a complete, managed remote environment_

## 📝 Project Steps

1. **Created the EC2 Instance (Windows)**
   - Log in to the AWS Management Console (https://signin.aws.amazon.com/), 
   ![image](https://github.com/FRANCOJUMAH/Creating-an-AWS-EC2-Instance-/blob/2efa99f82ef7d9d4d59a3921a3ef55a47846d58a/resources/Console.png)
   - Go to the EC2 Dashboard in the AWS Management Console and click "Launch Instance".
   - Name the instance ("tuko-kadi") and selected a Windows AMI (Microsoft Windows Server 2025 Base).
   - Choose an instance type, such as t2.micro (Free Tier eligible).
   - Create a new key pair, download the .pem file, and store it securely.
   - Under Network Settings, ensure "Auto-assign public IP" is enabled
