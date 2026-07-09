# 🖥️ Ticket #001 – External Monitors Not Detecting After Docking

## 📋 Ticket Information

| Field              | Value              |
| ------------------ | ------------------ |
| **Reported By**    | David Lee          |
| **Department**     | Support            |
| **Location**       | Floor 1            |
| **Issue Category** | Hardware / Display |
| **Priority**       | Medium             |
| **Status**         | Resolved           |

---

# 📝 Issue Summary

The user reported that both external monitors stopped displaying after docking their laptop. The laptop's built-in display continued to function normally.

The user confirmed:

- The issue previously worked without problems.
- Both monitors remained black after docking.
- The laptop screen displayed normally.
- Restarting the laptop did not resolve the issue.
- The laptop was re-docked several times with no success.

---

# 🎯 Objective

Restore functionality to both external monitors while maintaining normal laptop operation.

---

# 🔍 Troubleshooting Process

### Step 1 – Verify the Issue

Confirmed:

- Laptop powered on successfully.
- Internal display functioning correctly.
- Both external monitors remained blank.

---

### Step 2 – Inspect the Docking Station

Checked:

- Dock was securely connected.
- Power cable connected.
- Dock indicator lights operating normally.

---

### Step 3 – Inspect Display Connections

Verified:

- Display cables securely connected.
- Monitor power cables connected.
- Monitors powered on.

---

### Step 4 – Detect Displays

Opened:

**Settings → System → Display**

Selected:

**Detect Displays**

No additional displays were detected.

---

### Step 5 – Restart Dock Connection

Performed the following:

- Undocked laptop
- Waited several seconds
- Reconnected docking station

Displays remained unavailable.

---

### Step 6 – Test Hardware

Connected the laptop directly to one monitor using a display cable.

Result:

- External monitor displayed correctly.

This indicated that:

- Laptop GPU was functioning.
- Monitor was operational.
- Display cable was functional.

The issue appeared to be isolated to the docking station.

---

### Step 7 – Replace Dock

Connected the laptop to a known working docking station.

Result:

- Both monitors detected immediately.
- Extended display functionality restored.

---

# ✅ Resolution

The original docking station had developed a hardware fault and was no longer outputting video to connected displays.

Replacing the docking station restored both external monitors.

---

# 📚 Root Cause

Faulty docking station preventing video output to external monitors.

---

# 💼 Business Impact

The user was limited to the laptop's built-in display, making it difficult to work efficiently across multiple spreadsheets and applications.

Replacing the docking station restored the user's normal multi-monitor workspace.

---

# 💡 Lessons Learned

When a laptop display functions normally but multiple external monitors fail simultaneously, the docking station should be considered as a potential point of failure after verifying monitor power and cable connections. Testing with a known working dock is an effective way to isolate the issue.

---

## 🛠️ Skills Demonstrated

- Hardware troubleshooting
- Docking station diagnostics
- Display configuration
- Root cause analysis
- User support
- Incident documentation
