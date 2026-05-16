# Active Directory Help Desk Troubleshooting Lab

## Objective
This lab demonstrates common help desk account management tasks performed in Active Directory, including password resets, unlocking accounts, disabling accounts, and managing account expiration policies.

---

## Tools & Requirements
- Windows Server 2022 Virtual Machine
- Windows 11 Virtual Machine
- Active Directory
- VirtualBox
- VirtualBox Extension Pack

---
  
# Common Help Desk Troubleshooting Tasks
- Resetting passwords
- Unlocking locked accounts
- Disabling accounts
- Managing expired accounts

---

# Scenario A — Password Reset / Expired Password

## Situation
A user forgot their password or their password has expired.

---

## Steps
1. Open:
```text
Active Directory Users and Computers
```

2. Right-click the domain and select:
```text
Find Objects in Active Directory Domain Services
```

3. Search using:
- First Name
- Last Name

4. Locate the user account
5. Right-click the account and select:
```text
Reset Password
```

6. Create a temporary password
7. Enable:
```text
User must change password at next logon
```

8. Apply changes

---

## Screenshot — Password Reset

<p align="center">
  INSERT SCREENSHOT HERE
</p>

---

# Scenario B — Locked Account

## Situation
A user entered the wrong password too many times and their account became locked.

---

## Steps
1. Locate the user account using:
```text
Find Objects in Active Directory Domain Services
```

2. Double-click the user account
3. Open:
```text
Account
```

4. Locate the lockout section
5. Enable:
```text
Unlock Account
```

6. Click:
```text
Apply
```

> If the user does not remember their password, offer a password reset.

---

## Screenshot — Unlocking Account

<p align="center">
  INSERT SCREENSHOT HERE
</p>

---

# Scenario C — Disabling User Accounts

## Situation
A user is leaving the company and access must be removed.

---

## Steps
1. Locate the user account
2. Double-click the account
3. Open:
```text
Account
```

4. Under Account Options enable:
```text
Account is disabled
```

5. Click:
```text
Apply
```

> To re-enable the account, uncheck "Account is disabled."

---

## Screenshot — Disabled Account

<p align="center">
  INSERT SCREENSHOT HERE
</p>

---

# Why Disable Instead of Delete?

User accounts are typically disabled instead of deleted because organizations may need:
- Audit history
- Legal records
- File ownership tracking
- Compliance documentation

Disabling the account preserves organizational records while preventing access.

---

# Re-Enabling Accounts

## Important Policy
Help desk staff should not independently re-enable accounts for terminated users.

If a user requests account access restoration:
- Contact Human Resources (HR)
- Obtain authorization before re-enabling access

This ensures access decisions are approved by management and company policy.

---

# Scenario D — Expired Contract / Account Expiration

## Situation
A contractor or temporary employee can no longer sign in because their account expiration date has passed.

---

## Important Procedure
Never extend account expiration dates without approval.

Authorization must come from:
- Human Resources
- Manager approval
- Official company request

---

## Steps
1. Locate the user account
2. Double-click the account
3. Open:
```text
Account
```

4. Locate:
```text
Account Expires
```

5. Set the updated expiration date
6. Click:
```text
Apply
```

---

## Screenshot — Account Expiration Settings

<p align="center">
  INSERT SCREENSHOT HERE
</p>

---

# Skills Practiced
- Active Directory administration
- Password management
- Account lockout troubleshooting
- Account lifecycle management
- User account security
- Help desk procedures
- Administrative policy awareness

---

# What I Learned
This lab provided hands-on experience performing common help desk account management tasks in Active Directory while reinforcing security procedures, administrative policies, and user access management practices.
