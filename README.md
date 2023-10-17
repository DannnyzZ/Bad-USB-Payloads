
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
- [🧩 Supported formats](#-supported-formats)
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

CipherPurge stands as a commanding solution for those seeking robust data protection mechanisms. Merging advanced data wiping, data zeroing, data over AES-256 encryption, data zeroing, and data overwriting capabilities, CipherPurge introduces a powerful and intuitive Tkinter GUI interface for effortless data security management.

**CipherPurge** was created with a singular, paramount purpose: to enhance data security and protect your sensitive information in an increasingly digital and interconnected world.

In today's landscape of ever-evolving cyber threats and data breaches, ensuring the confidentiality and integrity of your digital assets is of utmost importance. Whether you're an individual seeking to safeguard personal documents or a business striving to protect proprietary information, CipherPurge offers a comprehensive solution. The software's sole purpose is to provide you with a powerful and accessible tool to:

> **Sanitize Data:** CipherPurge ensures that your data is thoroughly sanitized before encryption. By randomizing and zeroing out its contents, it guarantees that no trace of your original data remains.

> **Encrypt Securely:** Employing the AES-256 encryption standard, CipherPurge transforms your files into an unreadable format, adding an additional layer of security to your data.

> **Dispose Safely:** CipherPurge securely disposes of your encrypted files by moving them to the system and user trash. With the option to empty both trash locations, you can be certain that your sensitive files are beyond recovery.

CipherPurge incorporates the principles of **"Defense in Depth**," a cybersecurity strategy that emphasizes multiple layers of protection. This approach ensures that even if one layer is compromised, others remain intact to thwart potential threats. 

By offering military-grade encryption, data randomization, and secure file disposal in a user-friendly interface, CipherPurge empowers individuals and organizations to take control of their data security. 


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
