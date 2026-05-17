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
 <img width="1115" height="834" alt="Screenshot 2026-05-16 182741" src="https://github.com/user-attachments/assets/60e19da6-6bf7-4d27-9716-1379d78f714f" />
<img width="1111" height="837" alt="Screenshot 2026-05-16 182720" src="https://github.com/user-attachments/assets/84e9ac00-9855-4cb5-ac82-46dceaf4dc3c" />

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
 <img width="1109" height="837" alt="Screenshot 2026-05-16 182912" src="https://github.com/user-attachments/assets/f85cfd55-4871-4fed-9024-9732e304f2fb" />
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
  <img width="1113" height="834" alt="Screenshot 2026-05-16 183118" src="https://github.com/user-attachments/assets/29b8eafd-d1f8-44b2-9f23-6a152bd72c36" />
<img width="1114" height="836" alt="Screenshot 2026-05-16 183305" src="https://github.com/user-attachments/assets/91dda626-6de3-46d9-9c69-356313656469" />

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
<img width="1114" height="838" alt="Screenshot 2026-05-16 183414" src="https://github.com/user-attachments/assets/a8b59844-6e01-4d67-b647-3a85c6c1b26e" />
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
