# 🌐 Ticket #006 – No Network Connectivity Due to Faulty Ethernet Cable

## 📋 Ticket Information

| Field              | Value        |
| ------------------ | ------------ |
| **Reported By**    | Emily Carter |
| **Department**     | Finance      |
| **Location**       | Floor 1      |
| **Issue Category** | Networking   |
| **Priority**       | High         |
| **Status**         | Resolved     |

---

# 📝 Issue Summary

The user reported that their workstation had no wired network connectivity. Windows displayed **"No Internet Access"**, preventing access to shared network resources, email, and internal applications.

---

# 🎯 Objective

Restore the user's wired network connection and identify the source of the network failure.

---

# 🔍 Troubleshooting Process

## Step 1 – Verify the Issue

Confirmed:

- Network icon displayed no connectivity.
- User unable to access internal resources.
- Ethernet connection not detected.

---

## Step 2 – Physical Inspection

Checked:

- Ethernet cable securely connected to the workstation.
- Ethernet cable securely connected to the wall outlet.
- Visible damage to the cable.
- Link/activity LEDs on the network port.

No link lights were present.

---

## Step 3 – Test with a Known Working Ethernet Cable

Disconnected the existing Ethernet cable.

Connected a known working cable.

**Result:**

No change.

---

## Step 4 – Identify the Network Switch Port

Visited the network cabinet.

Used a cable tester and port identification tool to trace the wall outlet back to the corresponding switch port.

Verified:

- Correct patch panel connection.
- Correct switch port assignment.
- Switch port link status.

The switch port showed no active link.

---

## Step 5 – Replace Patch Cable

Replaced the patch cable between the patch panel and the network switch.

Immediately after replacement:

- Link light became active.
- Switch port reported an active connection.

---

## Step 6 – Verify Connectivity

Returned to the user's workstation.

Confirmed:

- Ethernet adapter connected.
- Valid IP address assigned via DHCP.
- Successful ping to the default gateway.
- Internet access restored.
- Access to internal resources confirmed.

---

# ✅ Resolution

Replaced the faulty patch cable connecting the patch panel to the network switch.

Network connectivity was restored successfully.

---

# 📚 Root Cause

Faulty Ethernet patch cable preventing communication between the workstation and the network switch.

---

# 💼 Business Impact

The user was unable to access network resources, preventing them from performing daily work until connectivity was restored.

---

# 💡 Lessons Learned

Physical layer issues should always be investigated before assuming software or configuration problems. Checking cables, link lights, and switch connectivity can quickly identify hardware faults and reduce troubleshooting time.

---

## 🛠️ Tools Used

- Ethernet Cable Tester
- Network Switch
- Patch Panel
- Known Working Ethernet Cable
- Command Prompt (`ipconfig`, `ping`)

---

## 🧠 Skills Demonstrated

- Physical Network Troubleshooting
- Ethernet Diagnostics
- Switch Port Identification
- Cable Replacement
- DHCP Verification
- Network Connectivity Testing
- Root Cause Analysis
