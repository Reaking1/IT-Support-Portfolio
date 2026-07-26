# 📧 Ticket #010 – Assign Microsoft 365 License to a New User

## 📋 Ticket Information

| Field              | Value                        |
| ------------------ | ---------------------------- |
| **Requested By**   | Human Resources              |
| **Department**     | Human Resources              |
| **Location**       | Head Office                  |
| **Issue Category** | Microsoft 365 Administration |
| **Priority**       | Medium                       |
| **Status**         | Resolved                     |

---

# 📝 Issue Summary

Human Resources submitted a request for a new employee to receive access to Microsoft 365 services. The user account had already been created in Microsoft Entra ID but did not have a Microsoft 365 license assigned.

As a result, the user could not access Outlook, Microsoft Teams, OneDrive, or other Microsoft 365 applications.

---

# 🎯 Objective

Assign the appropriate Microsoft 365 license to the user and verify access to Microsoft 365 services.

---

# 🛠️ Environment

- Microsoft 365 Admin Center
- Microsoft Entra ID
- Windows 11
- Microsoft Outlook
- Microsoft Teams

---

# 🔍 Implementation Process

## Step 1 – Verify the User Account

Opened the **Microsoft 365 Admin Center**.

Navigated to:

**Users → Active Users**

Verified that the user's account existed and was active.

---

## Step 2 – Check License Status

Selected the user account.

Reviewed the **Licenses and Apps** section.

Confirmed that no Microsoft 365 license had been assigned.

---

## Step 3 – Assign a License

Selected **Manage Licenses**.

Assigned the appropriate Microsoft 365 license for the user's role.

Saved the changes.

---

## Step 4 – Verify License Assignment

Confirmed that:

- The license appeared under the user's assigned products.
- The account status updated successfully.

---

## Step 5 – Test User Access

Requested that the user sign in using their Microsoft 365 credentials.

Verified successful access to:

- Microsoft Outlook
- Microsoft Teams
- OneDrive
- Microsoft 365 Portal

The user confirmed all services were available.

---

# ✅ Resolution

Assigned the required Microsoft 365 license to the user account.

The user successfully accessed Microsoft 365 services without further issues.

---

# 📚 Root Cause

The user account had been created successfully but no Microsoft 365 license had been assigned, preventing access to cloud services.

---

# 💼 Business Impact

The employee was unable to use email, collaboration tools, or cloud storage, delaying onboarding and daily work activities.

Assigning the appropriate license restored full productivity.

---

# 💡 Lessons Learned

Creating a Microsoft Entra ID account does not automatically grant access to Microsoft 365 services. A suitable Microsoft 365 license must also be assigned. Verifying license assignments should be part of every new user onboarding process.

---

## 🛠️ Skills Demonstrated

- Microsoft 365 Administration
- Microsoft Entra ID
- User Provisioning
- License Management
- Identity and Access Management
- Technical Documentation
- End-User Support
