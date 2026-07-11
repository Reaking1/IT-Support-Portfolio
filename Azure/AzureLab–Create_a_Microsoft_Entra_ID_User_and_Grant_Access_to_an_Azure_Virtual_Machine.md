# ☁️ Azure Lab – Create a Microsoft Entra ID User and Grant Access to an Azure Virtual Machine

## 📋 Lab Information

| Field          | Value                          |
| -------------- | ------------------------------ |
| **Platform**   | Microsoft Azure                |
| **Service**    | Microsoft Entra ID             |
| **Category**   | Identity and Access Management |
| **Difficulty** | Beginner                       |
| **Status**     | Completed                      |

---

# 📝 Overview

This lab demonstrates how to create a new user in Microsoft Entra ID and grant them permission to sign in to an Azure Virtual Machine using Azure Role-Based Access Control (RBAC).

This is a common administrative task performed by IT Support and Cloud Administrators when onboarding new employees.

---

# 🎯 Objectives

- Create a new user in Microsoft Entra ID.
- Configure the user's account.
- Grant the user access to an Azure Virtual Machine.
- Verify successful sign-in permissions.

---

# 🛠️ Environment

- Microsoft Azure Portal
- Microsoft Entra ID
- Azure Virtual Machine
- Windows Server 2025

---

# 🔍 Implementation Steps

## Step 1 – Create a User

In the Azure portal:

1. Navigate to **Microsoft Entra ID**.
2. Select **Users**.
3. Click **New User**.
4. Choose **Create New User**.
5. Enter the user's details, including:
   - Name
   - Username
   - Password (or auto-generate one)

6. Create the account.

---

## Step 2 – Verify the User

Confirmed that the new user appeared in the Entra ID user list.

Verified:

- Account enabled
- Username created successfully
- Password generated

---

## Step 3 – Grant VM Login Permissions

1. Open the Azure Virtual Machine.
2. Select **Access Control (IAM)**.
3. Choose **Add Role Assignment**.
4. Select one of the following roles:
   - Virtual Machine User Login
   - Virtual Machine Administrator Login (if administrative access is required)

5. Assign the role to the newly created Entra ID user.
6. Save the changes.

---

## Step 4 – Verify Access

Confirmed that the role assignment was successful.

The user was now authorized to sign in to the Azure Virtual Machine using their Microsoft Entra ID credentials (provided Entra ID authentication had been configured on the VM).

---

# ✅ Result

Successfully created a Microsoft Entra ID user and granted the appropriate permissions to access an Azure Virtual Machine.

---

# 📚 Key Concepts Learned

- Microsoft Entra ID user management
- Azure Role-Based Access Control (RBAC)
- Virtual Machine access management
- Identity and Access Management (IAM)
- User provisioning

---

# 💼 Business Value

Centralized identity management allows organizations to securely control user access to cloud resources. Using Azure RBAC ensures users receive only the permissions required for their role, supporting the principle of least privilege.

---

# 💡 Lessons Learned

Microsoft Entra ID provides centralized user management, while Azure RBAC controls what those users are allowed to do. Separating identity from permissions makes administration more secure and scalable.

---

## 🛠️ Skills Demonstrated

- Microsoft Entra ID Administration
- Azure Virtual Machines
- Azure RBAC
- Identity and Access Management (IAM)
- User Provisioning
- Access Management
- Technical Documentation
