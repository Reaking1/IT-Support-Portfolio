# 📧 Ticket #007 – User Unable to Send or Receive Emails in Microsoft Outlook

## 📋 Ticket Information

| Field              | Value                   |
| ------------------ | ----------------------- |
| **Reported By**    | Olivia Brown            |
| **Department**     | Human Resources         |
| **Location**       | Floor 3                 |
| **Issue Category** | Microsoft 365 / Outlook |
| **Priority**       | High                    |
| **Status**         | Resolved                |

---

# 📝 Issue Summary

The user reported that Microsoft Outlook was unable to send or receive emails. New emails were not appearing in the inbox, and outgoing messages remained in the Outbox.

The user confirmed:

- Restarting Outlook did not resolve the issue.
- Restarting the computer did not resolve the issue.
- Internet connectivity was working normally.

---

# 🎯 Objective

Restore the user's ability to send and receive emails through Microsoft Outlook.

---

# 🔍 Troubleshooting Process

## Step 1 – Verify the Issue

Confirmed:

- Outlook opened successfully.
- Emails remained in the Outbox.
- Inbox was not updating.
- Internet connection was operational.

---

## Step 2 – Check Outlook Connection Status

Verified Outlook's connection status.

Result:

Outlook was running in **Offline Mode**.

---

## Step 3 – Disable Offline Mode

Navigated to:

**Send/Receive → Work Offline**

Disabled **Work Offline**.

---

## Step 4 – Test Mail Synchronization

Forced a manual Send/Receive.

Result:

- New emails downloaded successfully.
- Emails in the Outbox were sent successfully.

---

## Step 5 – Confirm Resolution

Verified with the user that:

- New emails were received.
- Test email was sent successfully.
- Outlook synchronized normally.

---

# ✅ Resolution

Disabled Outlook's **Work Offline** mode and verified successful synchronization with Microsoft 365.

---

# 📚 Root Cause

Outlook had been placed into **Work Offline** mode, preventing communication with the Microsoft 365 mailbox.

---

# 💼 Business Impact

The user was unable to communicate via email, delaying internal communication and business processes.

Service was restored with no data loss.

---

# 💡 Lessons Learned

When Outlook cannot send or receive emails but the internet connection is functioning normally, checking whether **Work Offline** mode is enabled should be one of the first troubleshooting steps before investigating more complex issues.

---

## 🛠️ Skills Demonstrated

- Microsoft 365 Support
- Outlook Troubleshooting
- Email Synchronization
- User Assistance
- Root Cause Analysis
- Technical Documentation
