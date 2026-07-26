# 🔐 Ticket #011 – Reset Microsoft 365 User Password and Verify Multi-Factor Authentication

## 📋 Ticket Information

| Field              | Value                               |
| ------------------ | ----------------------------------- |
| **Reported By**    | Emma Davis                          |
| **Department**     | Sales                               |
| **Location**       | Floor 4                             |
| **Issue Category** | Microsoft 365 / Identity Management |
| **Priority**       | High                                |
| **Status**         | Resolved                            |

---

# 📝 Issue Summary

The user contacted the IT Service Desk after being unable to sign in to Microsoft 365. The user reported receiving an "Incorrect password" message despite multiple attempts.

The user was unable to access:

- Outlook
- Microsoft Teams
- OneDrive
- Microsoft 365 Portal

---

# 🎯 Objective

Verify the user's identity, reset the Microsoft 365 password, and confirm successful access to Microsoft 365 services.

---

# 🛠️ Environment

- Microsoft 365 Admin Center
- Microsoft Entra ID
- Microsoft Authenticator
- Windows 11

---

# 🔍 Troubleshooting Process

## Step 1 – Verify User Identity

Before making any account changes, the user's identity was verified in accordance with the organization's security procedures.

Verification included:

- Confirming the employee's identity.
- Verifying contact information on file.
- Completing Multi-Factor Authentication (MFA) verification where required.

---

## Step 2 – Review User Account

Opened the **Microsoft 365 Admin Center**.

Navigated to:

**Users → Active Users**

Confirmed:

- User account was active.
- No account lockout detected.
- Microsoft 365 license assigned.

---

## Step 3 – Reset the Password

Selected **Reset Password**.

Generated a temporary password.

Configured the account to require the user to change the password at the next sign-in.

---

## Step 4 – User Sign-In

Provided the temporary password securely.

The user successfully signed in.

The user created a new password during the first login.

---

## Step 5 – Verify MFA

Confirmed that:

- Microsoft Authenticator approval worked correctly.
- Multi-Factor Authentication completed successfully.
- User successfully accessed Outlook, Teams, and OneDrive.

---

# ✅ Resolution

The user's password was reset after identity verification. The user successfully completed MFA, changed the temporary password, and regained access to Microsoft 365 services.

---

# 📚 Root Cause

The user was unable to authenticate using their previous password. A password reset restored account access.

---

# 💼 Business Impact

The user could not access email, collaboration tools, or cloud services, preventing normal work activities until account access was restored.

---

# 🔒 Security Considerations

- Verify the user's identity before resetting passwords.
- Never communicate passwords through unsecured channels.
- Require the user to change any temporary password upon first sign-in.
- Confirm that MFA remains enabled after the password reset.

---

# 💡 Lessons Learned

Password resets are among the most common Microsoft 365 support tasks. Following identity verification procedures and enforcing MFA helps protect user accounts while minimizing downtime.

---

## 🛠️ Skills Demonstrated

- Microsoft 365 Administration
- Microsoft Entra ID
- Password Management
- Multi-Factor Authentication (MFA)
- Identity Verification
- User Account Administration
- Technical Documentation
- End-User Support
