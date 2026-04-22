# Linux Permissions & Access Control Lab

## Overview
In this lab, I worked with Linux user accounts, groups, and file permissions to understand how access control is enforced on a system. I created users, assigned group memberships, and tested how permissions affect access to files and directories.

## Objective
- Create and manage Linux users and groups
- Understand how permissions control access
- Test access between different users
- Apply least privilege concepts

## Lab Environment
- Ubuntu Server
- Linux Command Line

## Actions Performed

### 1. User and Group Creation
I created two users (`jenny` and `joe`) and added them to a group called `HR`.

📸 Evidence:
![User Creation](screenshots/linux-permissions-user-creation.png)

---

### 2. Verifying Account Information
I confirmed user and group configuration using system files and commands:
- `/etc/passwd`
- `/etc/group`
- `/etc/shadow`
- `groups`

📸 Evidence:
![Group Verification](screenshots/linux-permissions-group-verification.png)  
![User Group Membership](screenshots/linux-permissions-user-group-membership.png)  
![Passwd Verification](screenshots/linux-permissions-passwd-verification.png)

---

### 3. Testing Directory Access (Before Restriction)
I tested access between users by attempting to view and navigate directories before applying restrictions.

📸 Evidence:
![Directory Access Test](screenshots/linux-permissions-directory-access-test.png)

---

### 4. Restricting Permissions
I removed execute permission for others using `chmod` to prevent unauthorized directory access.

📸 Evidence:
![Permission Change](screenshots/linux-permissions-access-restriction-chmod.png)

---

### 5. Numeric Permissions (chmod 705)
I applied numeric permissions to control access levels and tested allowed actions.

📸 Evidence:
![Numeric Permissions](screenshots/linux-permissions-numeric-permissions-test.png)

---

### 6. Validating Access Control (Access Denied)
I verified that unauthorized users could no longer perform restricted actions.

📸 Evidence:
![Access Denied](screenshots/linux-permissions-access-denied-validation.png)

---

## Key Concepts Demonstrated
- Linux file permissions (read, write, execute)
- User and group management
- Least privilege enforcement
- Access validation testing

## SOC Analyst Relevance
This lab reflects real-world security practices where analysts:
- Verify access controls
- Investigate permission issues
- Ensure least privilege is enforced
- Validate security configurations

## What I Learned
This lab helped me understand how Linux enforces access control and how permissions directly impact system security. I practiced verifying access between users and applying changes to restrict unauthorized activity.
