# 🖥️ Ticket #004 – PowerShell Used to Identify Low Disk Space

## 📋 Ticket Information

| Field              | Value             |
| ------------------ | ----------------- |
| **Reported By**    | Sarah Johnson     |
| **Department**     | Finance           |
| **Location**       | Floor 3           |
| **Issue Category** | Windows / Storage |
| **Priority**       | Medium            |
| **Status**         | Resolved          |

---

# 📝 Issue Summary

The user reported receiving repeated "Low Disk Space" notifications and experienced slow system performance when opening files and applications.

---

# 🎯 Objective

Determine the cause of the low disk space warning and restore sufficient free storage for normal system performance.

---

# 🔍 Troubleshooting Process

## Step 1 – Verify the Issue

Confirmed:

- Low disk space notification displayed.
- Windows operating system functioning normally.
- User reported slower than usual performance.

---

## Step 2 – Check Disk Usage

Opened **PowerShell** as Administrator.

Executed the following command:

```powershell
Get-PSDrive -PSProvider FileSystem
```

### Result

```text
Name Used (GB) Free (GB)
C      236.8      4.2
```

The system drive (C:) had less than 5 GB of free space remaining.

---

## Step 3 – Identify Large Files

Used File Explorer and built-in Windows storage tools to identify large files and unnecessary temporary data.

Found:

- Temporary files
- Downloads folder containing unused installers
- Windows temporary cache files

---

## Step 4 – Clean Up Disk Space

Performed the following actions:

- Removed temporary files
- Deleted unnecessary installation files
- Emptied the Recycle Bin
- Ran Disk Cleanup

---

## Step 5 – Verify Resolution

Executed the PowerShell command again:

```powershell
Get-PSDrive -PSProvider FileSystem
```

### Result

```text
Name Used (GB) Free (GB)
C      214.3     26.7
```

Disk space had increased significantly.

System performance returned to normal.

---

# ✅ Resolution

Removed unnecessary files and verified available storage using PowerShell.

The user confirmed that the low disk space warning no longer appeared and system performance improved.

---

# 📚 Root Cause

The system drive was nearly full due to accumulated temporary files and unused downloads.

---

# 💼 Business Impact

Low available storage caused reduced system performance and disrupted the user's ability to work efficiently.

Cleaning the drive restored normal performance and prevented potential application issues.

---

# 💡 Lessons Learned

PowerShell provides a quick and reliable way to verify disk usage during troubleshooting. Combining PowerShell with Windows cleanup tools allows IT support technicians to identify storage issues efficiently and confirm that corrective actions have resolved the problem.

---

# 🛠️ PowerShell Commands Used

```powershell
Get-PSDrive -PSProvider FileSystem
```

---

## 🧠 Skills Demonstrated

- Windows Troubleshooting
- PowerShell Administration
- Storage Management
- Root Cause Analysis
- End-User Support
- Technical Documentation
