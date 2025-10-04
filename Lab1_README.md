# Cloud Computing Lab 1  
**Name:** Saira Ejaz  
**Roll No:** 2023-BSE-057  
**Section:** 5-B  

---

## 💻 Lab Task
**Installation of Ubuntu in VMware Workstation**

---

### 🧩 Step 1: VMware Installation

![VMware Installation](images/vmware_installation.png)

---

### 🧩 Step 2: Download Ubuntu Server ISO

![Download Ubuntu ISO](images/download_ubuntu_iso.png)

---

### 🧩 Step 3: Create a New Virtual Machine in VMware

1. Open **VMware Workstation Pro**  
2. Click **Create a New Virtual Machine**  
3. Select **Typical (recommended)**  
4. When asked for installation media, choose  
   **Installer disc image file (ISO)** and browse to the Ubuntu Server ISO you downloaded.  
5. Continue through the wizard, selecting the defaults unless otherwise instructed.  

![Create VM](images/create_new_vm.png)

---

### 🧩 Step 4: Start the Virtual Machine

1. Once the VM is created, click **Power on this virtual machine**.  
2. The Ubuntu Server installer will boot using the ISO file.  

![Start VM](images/start_vm.png)

---

### 🧩 Step 5: Accessing Ubuntu Server from Windows

Before moving further, make sure you can connect to your Ubuntu Server from your Windows host system.

#### 1️⃣ Find the IP Address of Ubuntu Server

Inside your Ubuntu Server VM, run the following command:
```bash
ip a
```

![Find IP](images/find_ip.png)

---

#### 2️⃣ Connect via SSH from Windows

On your Windows host, open **Command Prompt** or **PowerShell** and run:
```bash
ssh <username>@<ip-address>
```
*(Replace `<username>` with your Ubuntu user and `<ip-address>` with the one you just found.)*

![SSH Connection](images/ssh_connect.png)

---

#### 3️⃣ Accept the Fingerprint

When prompted, type:
```bash
yes
```

![Accept Fingerprint](images/accept_fingerprint.png)

---

#### 4️⃣ Enter Your Password

Use the same password you set during the Ubuntu Server installation.

![Enter Password](images/enter_password.png)

---

### ✅ Result
You have successfully installed **Ubuntu Server on VMware Workstation** and connected via **SSH** from Windows.

---

### 🏫 University Information
**Fatima Jinnah Women University, Rawalpindi**  
**Department of Software Engineering**

---
