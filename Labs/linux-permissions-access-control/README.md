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
![User Creation](screenshots/user-creation.png)

---

### 2. Verifying Account Information
I reviewed system files to confirm user and group configuration:
- `/etc/passwd`
- `/etc/group`
- `/etc/shadow`

📸 Evidence:
![Account Verification](screenshots/account-verification.png)

---

### 3. Testing Directory Access
I tested access between users by attempting to enter another user’s home directory.

📸 Evidence:
![Directory Access Test](screenshots/access-test-before.png)

---

### 4. Restricting Permissions
I removed execute permissions using `chmod` to prevent unauthorized access.

📸 Evidence:
![Permission Change](screenshots/permission-change.png)

---

### 5. Validating Access Control
After modifying permissions, I tested access again to confirm restrictions were enforced.

📸 Evidence:
![Access Denied](screenshots/access-denied.png)

---

### 6. Numeric Permissions (chmod 705)
I applied numeric permissions and tested what actions were allowed for other users.

📸 Evidence:
![Numeric Permissions](screenshots/numeric-permissions.png)

---

## Key Concepts Demonstrated
- Linux file permissions (read, write, execute)
- User and group management
- Least privilege enforcement
- Access validation testing

## SOC Analyst Relevance
This lab reflects real-world security practices where analysts verify access controls, investigate permission issues, and ensure that users only have the access they need.

## What I Learned
This lab helped me understand how Linux enforces access control and how permissions directly impact system security. I practiced verifying access between users and applying changes to restrict unauthorized activity. 
