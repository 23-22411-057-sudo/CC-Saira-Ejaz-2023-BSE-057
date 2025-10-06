<<<<<<< HEAD
# Lab1 - Cloud Computing Lab (with Screenshots)

This README file includes **step-by-step instructions** with screenshots extracted directly from the original lab PDF.


## Overview

Lab 1 demonstrates how to install Ubuntu Server in VMware Workstation and connect to it from Windows using SSH.
Steps are in the following order, :

- VMware Installation
- Ubuntu Installation
- Ubuntu Setup & Configuration
- Find IP & Network Commands
- SSH & Commands
- Other

---

## Steps with Screenshots
### Step : Download Vmware Workstation pro 


## VMware Installation

Install VMware Workstation and create a new virtual machine. See exact screenshots below:
![Step 1: Download Ubuntu Server ISO](screenshots/img_p1_2.png)
![Step 1: Download Ubuntu Server ISO](screenshots/img_p2_1.png)
![Step 1: Download Ubuntu Server ISO](screenshots/img_p2_2.png)
![Step 1: Download Ubuntu Server ISO](screenshots/img_p3_1.png)
![Step 1: Download Ubuntu Server ISO](screenshots/img_p3_2.png)

- Installation 

![Step 1: Download Ubuntu Server ISO](screenshots/img_p4_1.png)
![Step 1: Download Ubuntu Server ISO](screenshots/img_p4_2.png)


### Step 1: Download Ubuntu Server ISO

- Download Ubuntu Server ISO from the official Ubuntu website (https://ubuntu.com/download/server).
- Save it somewhere on your computer.

![Step 1: Download Ubuntu Server ISO](screenshots/img_p10_1.png)

![Step 1: Download Ubuntu Server ISO](screenshots/img_p10_2.png)

![Step 1: Download Ubuntu Server ISO](screenshots/img_p11_1.png)

![Step 1: Download Ubuntu Server ISO](screenshots/img_p11_2.png)

![Step 1: Download Ubuntu Server ISO](screenshots/img_p12_1.png)

![Step 1: Download Ubuntu Server ISO](screenshots/img_p12_2.png)

![Step 1: Download Ubuntu Server ISO](screenshots/img_p13_1.png)

![Step 1: Download Ubuntu Server ISO](screenshots/img_p13_2.png)



### Step 2: Create a new virtual machine in VMware Workstation

- Open VMware Workstation Pro.
- Click **Create a New Virtual Machine**.
- Select **Typical (recommended)**.
- Choose **Installer disc image file (ISO)** and browse to the Ubuntu Server ISO.
- Continue through the wizard, selecting defaults unless told otherwise.

![Step 2: Create a new virtual machine in VMware Workstation](screenshots/img_p5_1.png)

![Step 2: Create a new virtual machine in VMware Workstation](screenshots/img_p6_2.png)

![Step 2: Create a new virtual machine in VMware Workstation](screenshots/img_p7_1.png)

![Step 2: Create a new virtual machine in VMware Workstation](screenshots/img_p7_2.png)

![Step 2: Create a new virtual machine in VMware Workstation](screenshots/img_p8_1.png)

![Step 2: Create a new virtual machine in VMware Workstation](screenshots/img_p8_2.png)


### Step 3: Start and install Ubuntu Server

- Click **Power on this virtual machine**.
- Ubuntu Server setup will begin from the ISO.
- Follow the on-screen prompts to complete installation (set username, password, and network).

![Step 3: Start and install Ubuntu Server](screenshots/img_p9_1.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p9_2.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p10_1.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p10_2.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p11_1.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p11_2.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p12_1.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p12_2.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p13_1.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p13_1.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p14_1.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p14_1.png)

![Step 3: Start and install Ubuntu Server](screenshots/img_p15_1.png)


### Step 4: Find the IP address of Ubuntu Server

- After installation, login to Ubuntu Server terminal.
- Run the following command to view IP address:
- ```bash
ip a
```
- Look for the IPv4 address (e.g., 192.168.x.x).

![Step 4: Find the IP address of Ubuntu Server](screenshots/img_15_2.png)

![Step 4: Find the IP address of Ubuntu Server](screenshots/img_16_1.png)

![Step 4: Find the IP address of Ubuntu Server](screenshots/img_16_2.png)

![Step 4: Find the IP address of Ubuntu Server](screenshots/img_16_3.png)



### Step 5: Connect to Ubuntu Server via SSH from Windows

- On Windows (Command Prompt or Git Bash), type:
- ```bash
ssh <username>@<ip-address>
```
- When asked, type `yes` to accept the connection and enter your password.

![Step 5: Connect to Ubuntu Server via SSH from Windows](screenshots/img_p17_1.png)

![Step 5: Connect to Ubuntu Server via SSH from Windows](screenshots/img_p17_2.png)

![Step 5: Connect to Ubuntu Server via SSH from Windows](screenshots/img_p17_3.png)




### Step 6: Enable SSH service (if needed)

- If SSH connection fails, install OpenSSH Server:
- ```bash
sudo apt update && sudo apt install openssh-server
```
- Make sure the service is running:
- ```bash
sudo systemctl status ssh
```

![Step 6: Enable SSH service (if needed)](screenshots/page_12.png)


### Step 7: GitHub upload (optional)

- To upload your Lab1 folder to GitHub, use these commands:
- ```bash
git init
git add .
git commit -m "Add Lab1 with screenshots"
git branch -M main
git remote add origin <repo-url>
git push -u origin main
```

![Step 6: Enable SSH service (if needed)](screenshots/page_18.png)

## End of Lab 1

All screenshots above were extracted automatically from the original lab PDF provided by the student.
=======
# CC-Saira-Ejaz-2023-BSE-057
Cloud Computing Lab 1 &amp; 2 public repository
>>>>>>> ec2fd1138e7e792a055b311a9043400a7903c0e3
