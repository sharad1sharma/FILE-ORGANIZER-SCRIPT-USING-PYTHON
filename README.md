<div align="center">

# 📁 File Organizer Script Using Python

**An automated Python utility that cleans up cluttered directories by intelligently sorting and organizing files into dedicated subfolders based on file extensions.**

[![Python](https://img.shields.io/badge/Python-3.6%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Dependencies](https://img.shields.io/badge/Dependencies-Zero%20(Standard%20Library)-success)](#)
[![OS](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen)](#)

<br/>

> *Developed by **Sharad Sharma** for **SyntecXHub Technologies Pvt. Ltd.** (Task-2: Python Programming Internship).*

</div>

---

## 📌 Overview

Is your **Downloads** or **Desktop** folder cluttered with hundreds of unsorted PDFs, images, executables, documents, and code archives? 

**File Organizer Script** is an automated Python command-line tool built to solve digital clutter. Given any directory path, the script scans all contained files, parses their extensions, provisions destination folders on-the-fly, and relocates each file into its matching extension folder.

Built strictly with Python's built-in standard library (`os` and `shutil`), it requires **zero pip installations** and works out of the box on any system.

---

## 🔄 Before vs. After

```text
BEFORE (Cluttered Directory)            AFTER (Organized Directory)
📂 Downloads/                          📂 Downloads/
├── notes.txt                          ├── 📁 txt/
├── report.pdf                         │   └── notes.txt
├── picture.png                        ├── 📁 pdf/
├── invoice.pdf                        │   ├── report.pdf
├── installer.exe                      │   └── invoice.pdf
├── project.zip                        ├── 📁 png/
└── script.py                          │   └── picture.png
                                       ├── 📁 exe/
                                       │   └── installer.exe
                                       ├── 📁 zip/
                                       │   └── project.zip
                                       └── 📁 py/
                                           └── script.py
```

---

## ✨ Key Features

- ⚡ **Instant Bulk Organization**: Sorts through hundreds or thousands of files in seconds.
- 🧰 **Zero Third-Party Dependencies**: Built exclusively with Python's native `os` and `shutil` modules.
- 📂 **Dynamic Directory Provisioning**: Automatically detects novel file extensions and creates subdirectories on-the-fly.
- 🌐 **Cross-Platform Compatibility**: Fully compatible across Windows, macOS, and Linux distributions.
- 🛡️ **Non-Destructive Relocation**: Preserves original file names, extensions, and metadata using atomic moves.

---

## ⚙️ How It Works

```text
┌─────────────────────────────────┐
│     User Inputs Target Path     │
│   (e.g., C:/Users/Downloads)    │
└────────────────┬────────────────┘
                 │
                 ▼
┌─────────────────────────────────┐
│       Scan Directory Files      │
│         (os.listdir)            │
└────────────────┬────────────────┘
                 │
                 ▼
┌─────────────────────────────────┐
│     Extract File Extension      │
│       (os.path.splitext)        │
└────────────────┬────────────────┘
                 │
        ┌────────┴────────┐
        ▼                 ▼
Folder Exists?      Folder Missing?
(Skip creation)     (os.makedirs)
        └────────┬────────┘
                 │
                 ▼
┌─────────────────────────────────┐
│      Relocate File to Subdir    │
│          (shutil.move)          │
└────────────────┬────────────────┘
                 │
                 ▼
┌─────────────────────────────────┐
│  "Directory successfully        │
│          organized!"            │
└─────────────────────────────────┘
```

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.6 or higher installed:

```bash
python --version
```

*No third-party packages or virtual environments are needed!*

---

### Installation & Execution

1. **Clone the repository:**
   ```bash
   git clone https://github.com/sharad1sharma/FILE-ORGANIZER-SCRIPT-USING-PYTHON.git
   cd FILE-ORGANIZER-SCRIPT-USING-PYTHON
   ```

2. **Run the script:**
   ```bash
   python file_organizer_script.py
   ```

3. **Provide the target directory path:**
   - **Windows Example:**
     ```text
     Enter the path of the directory to organize: C:\Users\Username\Downloads
     ```
   - **macOS / Linux Example:**
     ```text
     Enter the path of the directory to organize: /home/username/Downloads
     ```

4. **Completion:**
   ```text
   Directory successfully organized!
   ```

---

## 🎯 Common Use Cases

- 🧹 **Tidying Downloads Folder**: Automatically sorts installers, PDFs, ZIP archives, and images.
- 📸 **Media Organization**: Categorizes `.jpg`, `.png`, `.mp4`, `.mkv`, and `.gif` files into clean subdirectories.
- 📑 **Document Archiving**: Groups `.pdf`, `.docx`, `.xlsx`, and `.pptx` documents together.
- 💻 **Developer Workspace**: Organizes scripts and configuration files by language (`.py`, `.js`, `.json`, `.sql`).

---

## 📂 Project Structure

```text
FILE-ORGANIZER-SCRIPT-USING-PYTHON/
│
├── file_organizer_script.py   # Core file sorting and organization script
└── README.md                  # Comprehensive documentation
```

---

## 👤 Author

**Sharad Sharma**
- GitHub: [@sharad1sharma](https://github.com/sharad1sharma)
- Email: [sharmasharad9531@gmail.com](mailto:sharmasharad9531@gmail.com)
- Organization: **SyntecXHub Technologies Pvt. Ltd.**

---

## 📄 License

This project is open-source and licensed under the [MIT License](LICENSE).
