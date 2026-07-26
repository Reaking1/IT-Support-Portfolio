# 🌐 Ticket #013 – Verify Network Connectivity Using PowerShell

## 📋 Ticket Information

| Field              | Value                             |
| ------------------ | --------------------------------- |
| **Reported By**    | Sophia Martinez                   |
| **Department**     | Customer Support                  |
| **Location**       | Floor 1                           |
| **Issue Category** | Windows / Networking / PowerShell |
| **Priority**       | High                              |
| **Status**         | Resolved                          |

---

# 📝 Issue Summary

The user reported that they were unable to access company websites, shared network drives, and internal applications. Internet connectivity appeared to be unavailable.

---

# 🎯 Objective

Determine whether the issue was caused by the user's workstation, the local network, or an external connection.

---

# 🛠️ Environment

- Windows 11
- Windows PowerShell
- Ethernet Connection

---

# 🔍 Troubleshooting Process

## Step 1 – Verify the Issue

Confirmed:

- User could not access internal company resources.
- Web pages failed to load.
- Network icon indicated limited connectivity.

---

## Step 2 – Check IP Configuration

Opened **PowerShell** as Administrator.

Executed:

```powershell
Get-NetIPAddress
```

Reviewed the assigned IPv4 address and confirmed the network adapter configuration.

---

## Step 3 – Test Connection to the Default Gateway

Executed:

```powershell
Test-NetConnection 192.168.1.1
```

**Result:**

The connection test failed, indicating the workstation could not communicate with the local network gateway.

---

## Step 4 – Inspect Network Adapter

Executed:

```powershell
Get-NetAdapter
```

Confirmed the Ethernet adapter was connected and operational.

---

## Step 5 – Renew the IP Address

Executed:

```powershell
ipconfig /release
ipconfig /renew
```

The workstation successfully obtained a new IP address from the DHCP server.

---

## Step 6 – Verify Connectivity

Executed:

```powershell
Test-NetConnection www.microsoft.com
```

The connection test completed successfully.

Verified:

- Internet access restored.
- Internal company resources accessible.
- User confirmed normal operation.

---

# ✅ Resolution

The network connection was restored after renewing the workstation's IP address. PowerShell confirmed successful communication with both the local gateway and external resources.

---

# 📚 Root Cause

The workstation had an invalid or expired network configuration that prevented communication with the network. Renewing the DHCP lease resolved the issue.

---

# 💼 Business Impact

The user was unable to access business-critical applications and online resources, temporarily interrupting normal work activities.

---

# 💡 Lessons Learned

PowerShell provides powerful networking cmdlets that help quickly determine whether connectivity issues originate from the local workstation, network infrastructure, or external services. Verifying IP configuration and testing connectivity are essential first steps when diagnosing network problems.

---

# 🛠️ PowerShell Commands Used

### View IP Configuration

```powershell
Get-NetIPAddress
```

### Check Network Adapter Status

```powershell
Get-NetAdapter
```

### Test Network Connectivity

```powershell
Test-NetConnection 192.168.1.1
```

### Renew IP Address

```powershell
ipconfig /release
ipconfig /renew
```

---

## 🧠 Skills Demonstrated

- PowerShell Administration
- Windows Networking
- DHCP Troubleshooting
- Network Diagnostics
- Root Cause Analysis
- Technical Documentation
- End-User Support
