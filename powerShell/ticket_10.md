# 🖥️ Ticket #012 – Identify and Restart a Stopped Windows Service Using PowerShell

## 📋 Ticket Information

| Field              | Value                |
| ------------------ | -------------------- |
| **Reported By**    | Daniel Smith         |
| **Department**     | Finance              |
| **Location**       | Floor 3              |
| **Issue Category** | Windows / PowerShell |
| **Priority**       | High                 |
| **Status**         | Resolved             |

---

# 📝 Issue Summary

The user reported that a business application would not open. The application displayed a connection error during startup.

Initial investigation suggested that the required Windows service was not running.

---

# 🎯 Objective

Identify the status of the required Windows service and restore application functionality.

---

# 🛠️ Environment

- Windows 11
- Windows PowerShell
- Administrator Privileges

---

# 🔍 Troubleshooting Process

## Step 1 – Verify the Issue

Confirmed:

- Application failed to connect.
- User received a service connection error.
- Internet connectivity was working normally.

---

## Step 2 – Check Service Status

Opened **PowerShell** as Administrator.

Executed:

```powershell
Get-Service
```

Reviewed the list of services and identified that the required service was in the **Stopped** state.

---

## Step 3 – Verify the Specific Service

Executed:

```powershell
Get-Service -Name "Spooler"
```

Result:

```text
Status   Name      DisplayName
------   ----      -----------
Stopped  Spooler   Print Spooler
```

---

## Step 4 – Restart the Service

Executed:

```powershell
Start-Service -Name "Spooler"
```

---

## Step 5 – Confirm Service Status

Executed:

```powershell
Get-Service -Name "Spooler"
```

Result:

```text
Status   Name      DisplayName
------   ----      -----------
Running  Spooler   Print Spooler
```

---

## Step 6 – Verify Resolution

Requested the user to reopen the application.

Confirmed:

- Application launched successfully.
- No further connection errors occurred.

---

# ✅ Resolution

Restarted the stopped Windows service using PowerShell.

The application resumed normal operation.

---

# 📚 Root Cause

The required Windows service had stopped unexpectedly, preventing the application from functioning correctly.

---

# 💼 Business Impact

The user could not access a business-critical application, interrupting normal work activities.

---

# 💡 Lessons Learned

PowerShell provides a fast and efficient way to check, start, and manage Windows services without navigating the Services console. This reduces troubleshooting time and improves administrative efficiency.

---

# 🛠️ PowerShell Commands Used

### View All Services

```powershell
Get-Service
```

### Check a Specific Service

```powershell
Get-Service -Name "Spooler"
```

### Start a Service

```powershell
Start-Service -Name "Spooler"
```

### Restart a Service

```powershell
Restart-Service -Name "Spooler"
```

---

## 🧠 Skills Demonstrated

- Windows Administration
- PowerShell
- Windows Services
- Application Troubleshooting
- Root Cause Analysis
- Technical Documentation
- End-User Support
