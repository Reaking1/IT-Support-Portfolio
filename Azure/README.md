# ☁️ Azure Windows Server 2025 Virtual Machine Lab

## 📖 Overview

This lab demonstrates how to deploy a **Windows Server 2025 Azure Edition** virtual machine in Microsoft Azure. The objective is to build a Windows Server environment that can be used to practice system administration, Active Directory, networking, PowerShell, and other IT support tasks.

---

## 🎯 Objectives

* Deploy a Windows Server 2025 virtual machine
* Create and organize Azure resources using a Resource Group
* Configure networking using a Virtual Network (VNet)
* Connect to the server using Remote Desktop (RDP)
* Learn best practices for managing Azure virtual machines

---

## 🛠️ Prerequisites

Before starting, ensure you have:

* An Azure account
* An active Azure subscription (Free Trial or Pay-As-You-Go)
* A stable internet connection
* Remote Desktop Connection (Windows)

---

## 📍 Step 1 – Select a Region

When deploying the virtual machine, choose one of the following regions:

**Preferred Region**

* East US

**Alternative Region**

* South Africa North

> **Note:** Choose the region closest to you whenever possible to reduce latency and improve performance.

---

## 📁 Step 2 – Create a Resource Group

Create a dedicated Resource Group to keep all resources related to this lab organized.

**Example**

```text
WindowsServerLab-RG
```

Using a Resource Group makes it easier to manage and remove all lab resources when you are finished.

---

## 🖥️ Step 3 – Select the Virtual Machine Image

Under **Image**, choose:

**Windows Server 2025 Azure Edition**

This image includes Microsoft's latest Windows Server features optimized for Azure.

---

## 🌐 Step 4 – Configure Networking

During deployment, Azure will prompt you to either:

* Create a new Virtual Network (VNet), or
* Select an existing VNet.

A Virtual Network allows Azure resources to communicate securely with one another.

This becomes especially important when adding future services such as:

* Active Directory Domain Services
* Additional Virtual Machines
* Azure Bastion
* Storage Accounts
* Network Security Groups (NSGs)

For this lab, allowing Azure to create a new VNet is perfectly acceptable.

---

## 📊 Step 5 – Configure Monitoring

Navigate to the **Monitoring** tab.

Locate the following option:

* Enable OS Diagnostics

Disable this setting before continuing.

Once complete, proceed through the remaining configuration pages until you reach **Review + Create**.

---

## 🚀 Step 6 – Deploy the Virtual Machine

Review your configuration.

If everything looks correct, select:

**Create**

Azure will begin deploying the virtual machine.

Deployment usually takes several minutes.

---

# 🔗 Connecting to the Virtual Machine

After deployment completes:

1. Open the Virtual Machine resource.
2. Select **Connect**.
3. Choose **RDP**.
4. Download the Remote Desktop (.rdp) file.
5. Open the downloaded file.
6. Enter the administrator username and password created during deployment.

After authentication, you should successfully connect to your Windows Server 2025 virtual machine.

---

# ⚠️ Important: Stop the Virtual Machine After Each Lab

Azure charges for compute resources while a virtual machine is running.

When you finish working:

1. Open the Virtual Machine.
2. Select **Stop**.
3. Wait until the status changes to **Stopped (Deallocated)**.

This is an important Azure best practice because it prevents unnecessary compute usage while the server is not in use.

When you're ready to continue your lab, simply select **Start** to power the virtual machine back on.

---

## 📚 Skills Practiced

* Azure Virtual Machines
* Azure Resource Groups
* Virtual Networking (VNet)
* Remote Desktop (RDP)
* Azure Resource Management
* Windows Server Administration

---

## 💡 Lessons Learned

This lab provided practical experience deploying and managing a Windows Server virtual machine in Azure. It reinforced the importance of organizing resources with Resource Groups, understanding Virtual Networks, connecting securely via RDP, and following cost-saving best practices by deallocating virtual machines when they are no longer needed.
