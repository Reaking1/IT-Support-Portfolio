# 🔐 Ticket #005 – BitLocker Recovery Key Required After System Restart

## 📋 Ticket Information

| Field              | Value                        |
| ------------------ | ---------------------------- |
| **Reported By**    | James Wilson                 |
| **Department**     | Finance                      |
| **Location**       | Floor 2                      |
| **Issue Category** | Windows Security / BitLocker |
| **Priority**       | High                         |
| **Status**         | Resolved                     |

---

# 📝 Issue Summary

The user reported that after restarting their company laptop, Windows prompted for a **BitLocker Recovery Key** before allowing the operating system to boot.

The user was unable to continue working because they did not know the recovery key.

---

# 🎯 Objective

Verify the user's identity, retrieve the correct BitLocker Recovery Key, and restore access to the device while following company security procedures.

---

# 🔍 Troubleshooting Process

## Step 1 – Verify the Issue

Confirmed:

- Device displayed the BitLocker Recovery screen.
- User was unable to access Windows.
- Recovery Key ID displayed on the screen.

---

## Step 2 – Verify User Identity

Before accessing any recovery information, verified the user's identity according to company security policy.

Verification included:

- Confirming the user's identity using Multi-Factor Authentication (MFA).
- Verifying employee details against company records.
- Confirming device ownership.

> **Security Note:** BitLocker Recovery Keys should never be provided until the user's identity has been successfully verified.

---

## Step 3 – Retrieve the Recovery Key

After successful identity verification:

- Located the device in the organization's management system.
- Matched the Recovery Key ID displayed on the device.
- Retrieved the corresponding BitLocker Recovery Key.

---

## Step 4 – Unlock the Device

Guided the user through entering the BitLocker Recovery Key.

Result:

- Windows booted successfully.
- User regained access to the operating system.

---

## Step 5 – Verify System Functionality

Confirmed:

- User successfully signed into Windows.
- Company applications opened normally.
- No further BitLocker prompts appeared.

---

# ✅ Resolution

The user's identity was verified using company security procedures, the correct BitLocker Recovery Key was retrieved, and access to the device was successfully restored.

---

# 📚 Root Cause

BitLocker requested the recovery key after detecting a change that required additional verification before unlocking the encrypted drive.

---

# 💼 Business Impact

The user was unable to access their workstation until the BitLocker Recovery Key was provided, temporarily preventing them from performing their daily work.

---

# 🔒 Security Considerations

- Verify the user's identity before accessing or disclosing a BitLocker Recovery Key.
- Match the Recovery Key ID displayed on the device with the stored recovery key.
- Never share recovery keys with unverified individuals.
- Record the verification process and actions taken in the support ticket.

---

# 💡 Lessons Learned

BitLocker protects organizational data by preventing unauthorized access to encrypted drives. Following identity verification procedures, including MFA where required, helps ensure recovery keys are released only to authorized users while maintaining compliance with security policies.

---

## 🛠️ Skills Demonstrated

- Windows Security
- BitLocker Administration
- Identity Verification
- Multi-Factor Authentication (MFA)
- Security Best Practices
- End-User Support
- Technical Documentation
