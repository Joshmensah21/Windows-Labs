# Lab 02 – User Accounts and Permissions

![Category](https://img.shields.io/badge/Category-Windows%20%2F%20User%20Accounts%20%26%20Permissions-blue)
![Date](https://img.shields.io/badge/Date%20Completed-24th%20July%202026-brightgreen)
![Tool](https://img.shields.io/badge/Tools-Settings%20%2F%20File%20Explorer%20%2F%20NTFS%20%2F%20Netplwiz-orange)

## 📌 1. Objective
The main purpose of this practical was to understand the main differences between administrative and user permissions by testing what different users can access or modify within Windows NTFS (New Technology File System). It also aimed to develop an understanding of how to create and manage multiple user accounts.

## 🛠️ 2. Tools Used
* Windows Settings
* File Explorer
* Windows NTFS Permissions
* Netplwiz to verify the account type

## ⚙️ 3. Procedure
1. Confirmed my existing Windows account had Administrator privileges.
2. Created a new Windows account for testing called ‘TestEmployee’.
3. Used ‘netplwiz’ to confirm ‘TestEmployee’ is a standard user.
4. Created an IT-Support-Test folder on the C: drive and added a text file to it.
5. Opened the folder’s security properties and investigated the permissions assigned to different users and groups.
6. Logged into TestEmployee and tested whether it could open, edit, create and delete files within the IT-Support-Test folder.
7. Investigated the Authenticated Users group to understand why the Standard User was able to modify the folder contents.

## 📊 4. Findings

### Account & Group Configuration
| Setting / Parameter | Detail |
| :--- | :--- |
| **Primary Account** | Administrator |
| **Test Account** | TestEmployee (Standard User) |
| **Test Directory** | `C:\IT-Support-Test` |
| **Test File** | `Employee-Notes.txt` |

### Effective Permissions Summary
| Group / User | Assigned Permissions | Observed Behavior |
| :--- | :--- | :--- |
| **SYSTEM & Administrators** | Full Control | Full read, write, modify, and delete access. |
| **Authenticated Users** | Modify, Write | Allowed Standard User to create, edit, and delete files. |

## 🔍 5. Troubleshooting / Analysis
During the lab, I encountered an unexpected result when TestEmployee was still able to edit, create and delete files. I found that the Authenticated Users group had Modify and Write permissions, so I concluded that permissions can be granted through multiple groups. This means I need to look more closely at the effective permissions a user has rather than simply looking at the permissions assigned to one group.

## 💡 6. Skills and Key Learning
* Creating and managing local Windows user accounts.
* Using netplwiz to check account types.
* Investigating NTFS permissions.

## 📸 7. Screenshots

### Figure 1 – IT-Support-Test folder containing Employee-Notes.txt
![IT-Support-Test folder containing Employee-Notes.txt](screenshots/01_IT_Support_Test_Folder.png)

### Figure 2 – NTFS permissions assigned to the IT-Support-Test folder
![NTFS permissions assigned to the IT-Support-Test folder](screenshots/02_NTFS_Permissions.png)

### Figure 3 – Permissions assigned to the Users group
![Permissions assigned to the Users group](screenshots/03_netwpliz_verification.png)
