
# Watch Me Build The Lab HERE
https://www.loom.com/share/5879d781f5224b6b97fdfffd6f20b4b4?sid=fc7f42a2-cc56-42ae-a680-db72ec3f279d

# AWS Lab: Connecting to a Windows Server 2022 EC2 Instance via RDP

This lab walks you through connecting to your Windows Server 2022 EC2 instance using Remote Desktop Protocol (RDP), incorporating steps mentioned in your transcript.

---

## 1. Introduction  
In this lab, we're connecting to the Windows Server 2022 EC2 instance created in the previous lab **Launch-AWS-EC2-Instance**. We'll use the AWS Console and RDP to establish the connection.

---

## 2. Navigate to Your EC2 Instance  
1. Open the **AWS Console** and go to **EC2** → **Instances** → **View Dashboard**.  
2. Locate the EC2 instance you want to connect to (from the previous lab).  
   - Note its **Instance ID** for identification.  
   - Observe both the **Public IP** and **Private IP** addresses.  
   - You can also view its **VPC ID** and **Subnet ID**.  

---

## 3. Initiate RDP Connection  
1. Click **Connect** on your EC2 instance.  
2. Select the **RDP client** (Remote Desktop) tab.  
   - Click **Download remote desktop file** (.rdp file).  
   - Click **Get Password** to retrieve the administrator password.  
     - Upload your **.pem key pair** (downloaded in the previous lab).  
     - Click **Decrypt Password**, then copy and store the decrypted password securely.  

---

## 4. Connect Using RDP Client  
1. Open the downloaded `.rdp` file using your Remote Desktop client (e.g., `Demo-ec2-instance-Lab.rdp` on Windows).  
2. When prompted, paste the decrypted administrator password.  
3. If a certificate warning appears, click **Yes** to proceed.  
4. You should now be logged into your Windows Server 2022 instance.  

---

## 5. Key Security Considerations  
- **Secure Storage of .pem Key**: Treat your key pair like a house key—store it securely and do not leave it unprotected.  
   
- **Certificate Warnings**: Windows instances typically use self-signed certificates. In production environments, configure a proper Certificate Authority to eliminate warning prompts.  
  
- **Licensing Limits**: Windows Server’s license allows only up to **two concurrent RDP sessions** for administrative use.  

---

## 6. What You’ll Do Next  
In the next lab, we'll install Active Directory components and begin configuring users and groups on the Windows Server instance.

---

##  Summary Table

| Step | Action |
|------|--------|
| 1 | Navigate to EC2 dashboard, locate instance, note IDs and IP info |
| 2 | Click Connect → RDP client → download .rdp file + get password via .pem |
| 3 | Open .rdp file, enter password, accept certificate, connect |
| 4 | Store key and password securely; acknowledge session limits |
| 5 | Proceed to Active Directory configuration in the next lab |

---


