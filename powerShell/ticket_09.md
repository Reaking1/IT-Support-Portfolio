# 🖥️ Ticket #009 – Gather System Information Using PowerShell

## 📋 Ticket Information

| Field              | Value                |
| ------------------ | -------------------- |
| **Reported By**    | Michael Evans        |
| **Department**     | Marketing            |
| **Location**       | Floor 2              |
| **Issue Category** | Windows / PowerShell |
| **Priority**       | Medium               |
| **Status**         | Resolved             |

---

# 📝 Issue Summary

The user reported that their workstation had become noticeably slower over the past week. Before escalating the issue for hardware replacement, system information was collected to determine whether the workstation met the organization's hardware requirements and to identify any potential resource limitations.

---

# 🎯 Objective

Collect system information using PowerShell to assist with troubleshooting and determine whether the workstation's hardware contributed to the reported performance issues.

---

# 🛠️ Environment

- Windows 11
- Windows PowerShell 5.1
- Administrator Access

---

# 🔍 Troubleshooting Process

## Step 1 – Launch PowerShell

Opened **Windows PowerShell** with administrative privileges.

---

## Step 2 – Collect System Information

Executed the following command:

```powershell
Get-ComputerInfo
```

This command returned detailed information including:

- Operating System
- Computer Name
- Windows Version
- Processor Information
- Installed Memory (RAM)
- BIOS Information
- Windows Installation Date

---

## Step 3 – Verify Memory

Executed:

```powershell
Get-CimInstance Win32_ComputerSystem | Select-Object TotalPhysicalMemory
```

Confirmed the installed physical memory.

---

## Step 4 – Verify Processor

Executed:

```powershell
Get-CimInstance Win32_Processor | Select-Object Name, NumberOfCores, NumberOfLogicalProcessors
```

Reviewed CPU model, core count, and logical processors.

---

## Step 5 – Verify Disk Capacity

Executed:

```powershell
Get-PSDrive -PSProvider FileSystem
```

Reviewed available disk space on the system drive.

---

## Step 6 – Analyze Results

Collected information indicated:

- Operating system installed correctly.
- Processor functioning normally.
- Sufficient available disk space.
- Hardware met the organization's minimum requirements.

No hardware-related issues were identified during the assessment.

---

# ✅ Resolution

System information was successfully collected using PowerShell and used to assist in troubleshooting. Hardware specifications met the required standards, allowing further investigation into software-related causes of the reported performance issue.

---

# 📚 PowerShell Commands Used

### Display Detailed System Information

```powershell
Get-ComputerInfo
```

### Display Installed Memory

```powershell
Get-CimInstance Win32_ComputerSystem | Select-Object TotalPhysicalMemory
```

### Display Processor Information

```powershell
Get-CimInstance Win32_Processor | Select-Object Name, NumberOfCores, NumberOfLogicalProcessors
```

### Display Available Disk Space

```powershell
Get-PSDrive -PSProvider FileSystem
```

---

# 💼 Business Impact

Gathering accurate system information reduced troubleshooting time and helped determine that the issue was not caused by insufficient hardware resources, allowing support efforts to focus on software diagnostics.

---

# 💡 Lessons Learned

PowerShell provides a fast and reliable way to gather detailed system information without navigating multiple Windows settings pages. Using built-in cmdlets improves troubleshooting efficiency and supports informed decision-making during incident resolution.

---

## 🛠️ Skills Demonstrated

- PowerShell Administration
- Windows Troubleshooting
- System Diagnostics
- Hardware Assessment
- Technical Documentation
- Root Cause Analysis
- End-User Support
