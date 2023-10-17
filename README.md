

<div align="center">
<h1 align="center">
<img src="https://github.com/DannnyzZ/CipherPurge/blob/main/CipherPurge_logo_wide.png?raw=true" >
<br>
</h1>
<p align="center">
</p>
 
<p align="center">
  <img src="https://img.shields.io/badge/Batch-Script-brightgreen.svg?style=for-the-badge&logo=Windows&logoColor=white" alt="Batch" />
  <img src="https://img.shields.io/badge/Rubber%20Ducky-Hardware-red.svg?style=for-the-badge&logo=usb&logoColor=white" alt="Rubber Ducky" />
  <img src="https://img.shields.io/badge/Bad%20USB-Hardware-purple.svg?style=for-the-badge&logo=usb&logoColor=white" alt="Bad USB" />
  <img src="https://img.shields.io/badge/PowerShell-Script-blue.svg?style=for-the-badge&logo=powershell&logoColor=white" alt="PowerShell" />
  <img src="https://img.shields.io/badge/Payload-Content-orange.svg?style=for-the-badge&logo=file&logoColor=white" alt="Payload" />
</p>


![GitHub license](https://img.shields.io/github/license/eli64s/readme-ai?style&color=5D6D7E)
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
  - [🎮 Using CipherPurge](#-using-CipherPurge)
  - [⚠️ Warning](#-warning)
- [🗺 Roadmap](#-roadmap)
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

| Feature                                   | Description                                                                                                                                                                                                                                              |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **⚙️ Data Encryption with AES-256**       | CipherPurge implements AES-256 encryption to ensure robust data security. The Advanced Encryption Standard with a 256-bit key provides high-level data confidentiality. It uses the `cryptography` library to perform AES encryption in Cipher Feedback (CFB) mode.    |
| **🔐 Secure File Overwriting**            | Enhancing data protection, the program securely overwrites files using a two-step process: randomization and zeroing. Random data is generated to match the original file's size, and zeroing ensures complete data erasure, preventing data recovery attempts.        |
| **📝 Action Logging**                    | CipherPurge maintains a detailed action log that records timestamped entries. This audit trail provides a comprehensive history of operations, aiding in accountability and troubleshooting. The log file is created in a "Logs" folder within the program directory.      |
| **🔄 Multithreaded Processing**           | To maintain a responsive user interface during time-consuming tasks, the program employs multithreading. Background operations, such as emptying the trash, run in separate threads, ensuring a smooth user experience while efficiently executing tasks.           |
| **📂 File Selection and Management**      | Users can select multiple files through a file dialog, and the program efficiently manages these selections in a Python list. Selected files are displayed in a user-friendly list, including file names, sizes, and extensions for easy reference and management.    |
| **🎨 UI Customization**                   | CipherPurge offers interface customization options, allowing users to define background and button colors, as well as font styles. This customization enhances visual appeal and tailors the program's appearance to individual preferences.                  |
| **❗ Error Handling and Reporting**        | Robust error-handling mechanisms catch and report exceptions during file operations. User-friendly error messages provide clear guidance in case of unexpected issues, ensuring a seamless and user-friendly experience.                                       |
| **🖼️ Resizable User Interface**          | Users can resize the application window, adapting it to different screen resolutions and preferences. This feature enhances user comfort and usability, accommodating various display configurations and environments.                                        |
| **📁 File Format Versatility**           | Designed to accommodate diverse file formats, CipherPurge is versatile and suitable for processing various data types, including text, binary, documents, and images. This flexibility ensures compatibility with a wide range of file formats.                  |


---

## 🧩 Supported formats


| File Type                   | File Extensions                                      |
|-----------------------------|------------------------------------------------------|
| **Documents**               | .docx - Microsoft Word Document                      |
|                             | .xlsx - Microsoft Excel Spreadsheet                  |
|                             | .pptx - Microsoft PowerPoint Presentation            |
|                             | .pdf - Adobe Portable Document Format                |
|                             | .txt - Text Document                                  |
|                             | .rtf - Rich Text Format                              |
| **Images**                  | .jpg / .jpeg - JPEG Image                            |
|                             | .png - Portable Network Graphics                     |
|                             | .gif - Graphics Interchange Format                   |
|                             | .bmp - Bitmap Image                                  |
|                             | .tiff - Tagged Image File Format                     |
|                             | .eps - Encapsulated PostScript                       |
| **Archives**                | .zip - ZIP Archive                                   |
|                             | .rar - RAR Archive                                   |
|                             | .7z - 7-Zip Archive                                 |
|                             | .tar - Tape Archive                                  |
|                             | .gz / .gzip - GZIP Compressed Archive                |
| **Spreadsheets and Databases** | .csv - Comma-Separated Values                    |
|                             | .db / .sqlite - Database File                       |
|                             | .xls - Microsoft Excel 97-2003 Workbook            |
|                             | .accdb - Microsoft Access Database                  |
| **Emails**                  | .eml - Email Message                                 |
|                             | .pst - Microsoft Outlook Personal Storage Table     |
| **Presentations**           | .ppt - Microsoft PowerPoint Presentation (Legacy)    |
|                             | .key - Apple Keynote Presentation                    |
| **Web-Related**             | .html / .htm - HTML Web Page                         |
|                             | .xml - Extensible Markup Language                    |
|                             | .json - JavaScript Object Notation                   |
|                             | .php - PHP Script                                   |
|                             | .asp - Active Server Pages                          |
| **Compressed Data**         | .tar.gz / .tgz - Tar GZIP Compressed Archive         |
|                             | .bz2 - BZIP2 Compressed Archive                      |
| **Source Code and Scripts** | .py - Python Script                                 |
|                             | .java - Java Source Code                            |
|                             | .c / .cpp - C/C++ Source Code                       |
|                             | .js - JavaScript Code                               |
|                             | .sh - Shell Script                                  |
| **Audio and Video**         | .mp3 - MP3 Audio File                               |
|                             | .mp4 - MP4 Video File                               |
|                             | .avi - Audio Video Interleave                       |
| **CAD and Design Files**    | .dwg - AutoCAD Drawing Database                     |
|                             | .psd - Adobe Photoshop Document                     |
| **Backup and Configuration** | .bak - Backup File                                  |
|                             | .conf - Configuration File                          |
| **Data Formats**            | .xml - Extensible Markup Language (XML) File        |
|                             | .json - JavaScript Object Notation (JSON) File      |
| **Virtualization and Disk Images** | .iso - Disk Image File (e.g., for OS installation) |
|                             | .vhd - Virtual Hard Disk                            |
|                             | .vmdk - VMware Virtual Disk                        |
| **Database Backup**         | .bak - Database Backup File (commonly associated with SQL databases) |

This list represents only part of supported formats and extensions. Software doesn't support erasing folders.

---

## 🚀 Getting Started

<div align="center">
  <img src="https://github.com/DannnyzZ/CipherPurge/assets/119814239/92532790-82f3-4133-817f-2400675db24b" alt="gui_screen">
</div>


### ✔️ Prerequisites

Before you begin, ensure that you have the following prerequisites installed:

>  ` Windows 7/8/10/11`

>  ` Python`

>  ` Python Package Installer `

>  ` Python library: tkinter `

>  ` Python library: cryptography `

>  ` Python library: send2trash `

>  ` Internet connection `

### 💻 Installation

1. Install python
```sh
1.	Visit the official Python website: https://www.python.org/downloads/
2.	Go to the Downloads section and choose the version of Python you want to install (e.g., Python 3.9.6).
3.	Scroll down to the bottom of the page and select the installer that matches your system architecture (32-bit or 64-bit).
4.	Run the downloaded installer.
5.	In the installer, select the option to add Python to the system PATH, which will make it accessible from the command line.
6.	Make sure that in optional features you choose pip to be installed.
7.	Complete the installation by following the on-screen instructions.
```

2. Install dependencies
```sh
pip install pip & pip install tkinter & pip install cryptography & pip install send2trash & pip install tk
```

3. Check version of python and pip:
```sh
python --version && pip --version
```

### 🎮 Using CipherPurge


1. Download cipherpurge.py from this link:
```sh
https://github.com/DannnyzZ/CipherPurge/blob/main/cipherpurge.py
```
2. Run commandline or powershell and execute:
```sh
python cipherpurge.py
```
WARNING! Make sure You provide the correct location of CipherPurge.

Example of use:
```sh
python C:\Users\Danny\Desktop\cipherpurge.py
```

---


### ⚠️ Warning


**Using CipherPurge safely:**

1. Data Irreversibility: Understand that CipherPurge permanently deletes and overwrites files. Once an operation is performed, it cannot be undone. Make sure you have backups or are absolutely certain about the files you select for processing.

2. Data Loss: CipherPurge sanitizes files by clearing their content, randomizing data, zeroing it out, encrypting it, and moving it to the trash. This may result in complete data loss. Do not use this tool on files you intend to keep.

3. Use with Caution: CipherPurge is designed for secure data destruction and not for general file management. Use it responsibly and only on files you explicitly intend to delete.

4. Backup Important Data: Before using CipherPurge, back up any important or valuable data to ensure it is not accidentally deleted or overwritten.

5. Contact Developer: If you have any doubts or need assistance, contact the developer for guidance.

**Use CipherPurge wisely to enhance data security while minimizing risks.**


## 🗺 Roadmap

> - [X] ` Task 1: Multiple bug fixes`
> - [X] ` Task 2: Support for new extensions of files.`

> - [ ] ` Incoming feature 1: New feature: sanitization of whole drives (internal or external memory)`
> - [ ] ` Incoming feature 2: New feature: drag and drop`
> - [X] ` Incoming feature 3: Support for more file extensions.`
> - [ ] ` Incoming feature 4: Support for whole folders not only choosen objects.`
> - [ ] ` Incoming feature 5: Meter on list of objects choosen to sanitize.`
> - [ ] ` Incoming feature 6: Full launch from .exe file (portable version).`
> - [ ] ` Incoming improvement: Better, more user friendly GUI.`


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
   
  `ℹ️  ChatGPT 4.0`
   
  `ℹ️  Readme-ai https://github.com/eli64s/readme-ai`

  `ℹ️  Logo.com https://logo.com`
  

---
