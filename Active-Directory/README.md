# 👥 Ticket #008 – Restrict User Access to Windows Settings Using Group Policy

## 📋 Ticket Information

| Field              | Value                           |
| ------------------ | ------------------------------- |
| **Reported By**    | IT Operations Manager           |
| **Department**     | Information Technology          |
| **Location**       | Head Office                     |
| **Issue Category** | Active Directory / Group Policy |
| **Priority**       | Medium                          |
| **Status**         | Resolved                        |

---

# 📝 Issue Summary

The IT department requested that standard users be prevented from modifying Windows settings to reduce unauthorized system changes and ensure compliance with company security policies.

The requested restrictions included:

- Prevent access to Windows Settings.
- Prevent changes to Control Panel settings.
- Prevent changes to security-related settings.
- Prevent unauthorized configuration changes.

---

# 🎯 Objective

Create and apply a Group Policy Object (GPO) that restricts standard users from accessing Windows configuration settings while allowing administrators to retain full access.

---

# 🛠️ Environment

- Windows Server 2022
- Active Directory Domain Services (AD DS)
- Group Policy Management Console (GPMC)
- Windows 11 Client

---

# 🔍 Implementation Process

## Step 1 – Open Group Policy Management

Opened:

**Server Manager → Tools → Group Policy Management**

---

## Step 2 – Create a New GPO

Created a new Group Policy Object named:

```text
Workstation Security Policy
```

---

## Step 3 – Edit the GPO

Navigated to:

```text
User Configuration
 └── Administrative Templates
      └── Control Panel
```

Enabled the policy:

- **Prohibit access to Control Panel and PC Settings**

---

## Step 4 – Link the GPO

Linked the Group Policy Object to the Organizational Unit (OU) containing the standard user accounts.

Administrators were excluded from the policy.

---

## Step 5 – Update Group Policy

On the client computer, opened Command Prompt and executed:

```cmd
gpupdate /force
```

Restarted the workstation.

---

## Step 6 – Verify the Policy

Signed in using a standard user account.

Confirmed:

- Access to Windows Settings was blocked.
- Control Panel could not be opened.
- Administrative settings remained protected.

Signed in using an administrator account.

Confirmed:

- Administrative access remained unaffected.

---

# ✅ Resolution

A Group Policy Object was successfully created and applied to restrict standard users from modifying Windows settings while maintaining administrator access.

---

# 📚 Root Cause

Standard users had unrestricted access to Windows configuration settings, increasing the risk of accidental or unauthorized system changes.

---

# 💼 Business Impact

Applying the policy improved workstation security, reduced support incidents caused by user configuration changes, and ensured a consistent desktop environment across the organization.

---

# 💡 Lessons Learned

Group Policy is an effective way to centrally manage Windows security and user permissions in an Active Directory environment. Applying policies to Organizational Units allows administrators to target specific users or devices while preserving administrative access where required.

---

## 🛠️ Skills Demonstrated

- Active Directory Administration
- Group Policy Management
- Organizational Unit (OU) Management
- Windows Security
- Policy Deployment
- System Administration
- Technical Documentation
