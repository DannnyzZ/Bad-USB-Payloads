
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

## ⚙️ Features

This payload, titled "Bad USB - winPEAS," is a script designed for USB Rubber Ducky or similar devices. It targets Windows 10/11 systems and performs the following actions:

Delays for 2 seconds to ensure the target system recognizes the device.

Emulates keyboard inputs to open the Windows Command Line:

Activates the Start menu.
Types "cmd" to open the Command Line.
Executes a series of commands:

Disables command echo.
Sets variables for a malicious download:
"downloadURL" points to a remote location.
"downloadPath" specifies a local path.
"runCommand" specifies the path to the downloaded file.
Downloads a file from the "downloadURL" and saves it locally.
Executes the downloaded file.
This payload aims to download and execute a potentially malicious file from a remote source. It leverages USB Rubber Ducky for physical delivery and targets Windows 10/11 Command Line environments.
``sh
dddd
``sh

---



## 🚀 Getting Started

<div align="center">
  <img src="https://github.com/DannnyzZ/CipherPurge/assets/119814239/92532790-82f3-4133-817f-2400675db24b" alt="gui_screen">
</div>


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


---
