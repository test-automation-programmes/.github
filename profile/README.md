# 🧰 Automation Tools Overview

This document provides a short, centralized overview of all internal automation tools available in this organization.

All tools are accessed through a single **Dashboard application**, which displays every tool as a button and handles launching them correctly.

---

## 🧭 Dashboard (Central Launcher)

Purpose  
The dashboard is the main entry point for all automation tools.

What it does
- 📋 Shows all tools in one place
- 🖱️ Opens tools using buttons
- 📂 Ensures correct paths and shared data usage
- 🚫 Removes the need for command-line execution

Important
- ✅ **Always start tools from the dashboard**
- ⚠️ Tools should not be launched directly unless for development

---

## 🖥️ Dashboard Executable (Dashboard.exe)

The dashboard can also be used as a Windows executable file to simplify usage and remove the need to manually run Python files.

What the executable provides
- 🚀 One-click startup using Dashboard.exe
- 🧑‍💻 No command-line interaction required
- 🔁 Same behavior as dashboard.pyw
- 🔍 Automatic detection of all available tools

How to use the executable
1. 📁 Place Dashboard.exe inside the **dashboard** folder
2. 📁 Ensure all tool folders are located in the same parent directory as the **dashboard** folder
3. 🖱️ Double-click Dashboard.exe to launch the dashboard
4. 🎯 Select the required tool by clicking its button
5. 📌 Follow on-screen instructions if shown

Required folder structure example

    automation-root/
    ├── dashboard/
    │   ├── Dashboard.exe
    │   └── dashboard_icon.ico
    ├── main-files/
    ├── apply-license/
    ├── band-locker/
    ├── create-test-results-excel-file/
    ├── flash-helper/
    ├── hota-request-message/
    ├── install-aresrt/
    ├── fieldtest/
    ├── hlt/
    ├── log-puller/
    └── tap-uploader/

Important notes
- ❌ If Dashboard.exe is moved out of the dashboard folder, tools will not be detected
- ⚠️ The message "No scripts found" indicates an incorrect folder structure
- ✅ **Tools should always be launched from the dashboard executable**

---

## 🛠️ Available Automation Tools

### 1️⃣ Apply License

What it does
- 🔑 Applies license files to target devices
- ⏱️ Reduces manual license configuration work
- ✅ Ensures correct license usage per device

Opened from dashboard
- 🖱️ Click Apply License

---

### 2️⃣ Band Locker

What it does
- 📡 Locks specific frequency bands on devices
- 🔒 Prevents unintended band changes
- 🧪 Supports controlled testing scenarios

Opened from dashboard
- 🖱️ Click Band Locker

---

### 3️⃣ Create Test Results Excel File

What it does
- 📊 Automatically generates standardized test result Excel files to add your test results
- 📐 Ensures consistent format for reporting
- ❌ Reduces manual Excel creation errors

Opened from dashboard
- 🖱️ Click Create Test Results Excel File

---

### 4️⃣ Flash Helper

What it does
- 💾 Assists with flashing firmware on devices
- 🧭 Guides users through required flashing steps
- ✅ Reduces flashing errors and rework

Opened from dashboard
- 🖱️ Click Flash Helper

---

### 5️⃣ HOTA Request Message

What it does
- ✉️ Generates standardized HOTA request messages
- 🌍 Uses shared device and country data
- ✅ Produces ready-to-send request content

Opened from dashboard
- 🖱️ Click HOTA Request Message

---

### 6️⃣ Install AresRT

What it does
- 📲 Installs AresRT, FieldTest and HLT apps on target devices
- ✅ Validates installation success
- 🔁 Removes repetitive manual setup steps

Opened from dashboard
- 🖱️ Click Install AresRT

---

### 7️⃣ TAP Uploader

What it does
- ☁️ Uploads MR and TA Excel test results to the TAP system
- 🤖 Automates login, upload, and verification
- 🖼️ Generates logs and screenshots
- 📂 Moves completed files to a Done folder

Opened from dashboard
- 🖱️ Click TAP Uploader

---

### 8️⃣ Log Puller

What it does
- 📥 **Automatically extracts** system logs, FieldTest logs, and screen recordings from connected devices
- 🧹 **Cleans up** extracted files from the device's SD card to free up storage space
- 🗜️ **Compresses** all gathered data into a neatly named ZIP file locally for easy sharing

Opened from dashboard
- 🖱️ Click Log Puller

---

## 📂 Shared Data – Main Files

Main files is a shared data repository, not a tool.

Purpose
- 📘 Stores centralized device information in Excel
- 🧠 Acts as a single source of truth for all tools
- 🆔 Provides device codes, countries, and serial numbers

Important
- 🔄 Used automatically by tools
- ⚠️ **Should not be modified without validation**

---

## 🧑‍💻 How Tools Are Used

1. ▶️ Launch the Dashboard
2. 🎯 Select the required tool
3. 🖱️ Click the corresponding button
4. 📌 Follow on-screen instructions if any

✅ **No manual script execution is required**

---

## ⬇️ How to Download

### Step 1 Install required software  
Ensure the following are installed
- 🐍 Python (recommended 3.9 or higher)
- 🎭 Playwright (required for browser automation)
- 📊 Microsoft Excel
- 🌐 Microsoft Edge
- 🔧 Git

---

### Step 2 Clone repositories

```bash
git clone https://github.com/test-automation-programmes/dashboard.git
git clone https://github.com/test-automation-programmes/main-files.git 
git clone https://github.com/test-automation-programmes/tap-uploader.git
git clone https://github.com/test-automation-programmes/install-aresrt-fieldtest-hlt.git
git clone https://github.com/test-automation-programmes/hota-request-message.git
git clone https://github.com/test-automation-programmes/flash-helper.git
git clone https://github.com/test-automation-programmes/create-test-results-excel-file.git
git clone https://github.com/test-automation-programmes/band-locker.git
git clone https://github.com/test-automation-programmes/apply-license.git
git clone https://github.com/test-automation-programmes/log-puller.git
