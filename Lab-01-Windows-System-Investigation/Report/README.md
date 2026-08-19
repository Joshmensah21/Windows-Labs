# Lab 01 – Windows System Investigation

![Category](https://img.shields.io/badge/Category-Windows%20%2F%20System%20Administration-blue)
![Date](https://img.shields.io/badge/Date%20Completed-16th%20July%202026-brightgreen)
![Tool](https://img.shields.io/badge/Tools-Command%20Prompt%20%2F%20Task%20Manager%20%2F%20Device%20Manager-orange)

## 📌 1. Objective
The objective of this lab was to investigate a Windows computer and collect important system, hardware, storage, and network information. This helps develop the skills required by IT support technicians when identifying device specifications and troubleshooting user issues.

## 🛠️ 2. Tools Used
* Windows Command Prompt
* Task Manager
* Device Manager
* File Explorer
* `hostname`
* `systeminfo`
* `ipconfig /all`

## ⚙️ 3. Procedure
1. Used Command Prompt commands (`hostname`, `systeminfo`, `ipconfig /all`) to collect system and network information.
2. Reviewed storage details using File Explorer.
3. Monitored resource usage using Task Manager.
4. Checked Device Manager for hardware or driver issues.

## 📊 4. Findings

### System Information
| Setting | Value |
| :--- | :--- |
| **OS Name** | Microsoft Windows 11 Home |
| **Version** | 10.0.26200 N/A Build 26200 |
| **System Type** | x64-based PC |
| **Processor** | Intel (R) Core (TM) i3-N305 @ 1.80 GHz |
| **RAM** | 8.00 GB |

### Network Information
| Setting | Value |
| :--- | :--- |
| **IPv4 Address** | `192.168.4.23` |
| **Default Gateway** | `192.168.4.1` |
| **MAC Address** | `20-0B-74-26-46-24` |
| **DHCP Enabled** | Yes |

### Hardware Health
* **Device Manager warnings:** None

## 🔍 5. Troubleshooting / Analysis
The investigation showed that the computer is running Windows 11 64-bit with an Intel® Core™ i3-N305 processor and 8 GB RAM. Network settings were verified using `ipconfig /all`, showing DHCP is enabled, and the device is receiving configuration from the router automatically. Device Manager showed no warnings, indicating no detected hardware or driver issues.

## 💡 6. Skills and Key Learning
* Used Windows command-line tools to collect system information.
* Analyzed network configuration including IPv4, MAC address, DHCP, and gateway information.
* Used Device Manager and Task Manager for basic troubleshooting.

## 📸 7. Screenshots

### Figure 1 - Output of systeminfo
![Output of systeminfo](Lab-01-Windows-System-Investigation/screenshots/01_system_info.png)

### Figure 2 - Output of ipconfig /all
![Output of ipconfig /all](Lab-01-Windows-System-Investigation/screenshots/02_ipconfig_all.png)

### Figure 3 - Task Manager (Before)
![Task Manager Before](Lab-01-Windows-System-Investigation/screenshots/03_task_manager_before.png)

### Figure 4 - Task Manager (After)
![Task Manager After](Lab-01-Windows-System-Investigation/screenshots/04_task_manager_after.png)

### Figure 5 – Storage Details
![Storage Screenshot](Lab-01-Windows-System-Investigation/screenshots/05_storage_screenshot.png)

### Figure 6 – Device Manager Status
![Device Manager](Lab-01-Windows-System-Investigation/screenshots/06_device_manager.png)
