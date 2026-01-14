# Automation Tools Overview

This document provides a **short, centralized overview** of all internal automation tools available in this organization.

All tools are accessed through a **single Dashboard application**, which displays every tool as a button and handles launching them correctly.

---

## 🧭 Dashboard (Central Launcher)

**Purpose**  
The dashboard is the **main entry point** for all automation tools.

**What it does**
- Shows all tools in one place
- Opens tools using buttons
- Ensures correct paths and shared data usage
- Removes the need for command‑line execution

**Important**
- Always start tools **from the dashboard**
- Tools should not be launched directly unless for development

---

## 🛠️ Available Automation Tools

### 1️⃣ Apply License

**What it does**
- Applies license files to target devices
- Reduces manual license configuration work
- Ensures correct license usage per device

**Opened from dashboard**
- Click **Apply License**

---

### 2️⃣ Band Locker

**What it does**
- Locks specific frequency bands on devices
- Prevents unintended band changes
- Supports controlled testing scenarios

**Opened from dashboard**
- Click **Band Locker**

---

### 3️⃣ Create Test Results Excel File

**What it does**
- Automatically generates standardized test result Excel files to add your test results
- Ensures consistent format for reporting
- Reduces manual Excel creation errors

**Opened from dashboard**
- Click **Create Test Results Excel File**

---

### 4️⃣ Flash Helper

**What it does**
- Assists with flashing firmware on devices
- Guides users through required flashing steps
- Reduces flashing errors and rework

**Opened from dashboard**
- Click **Flash Helper**

---

### 5️⃣ HOTA Request Message

**What it does**
- Generates standardized HOTA request messages
- Uses shared device and country data
- Produces ready‑to‑send request content

**Opened from dashboard**
- Click **HOTA Request Message**

---

### 6️⃣ Install AresRT

**What it does**
- Installs AresRT, FieldTest and HLT apps on target devices
- Validates installation success
- Removes repetitive manual setup steps

**Opened from dashboard**
- Click **Install AresRT**

---

### 7️⃣ TAP Uploader

**What it does**
- Uploads MR and TA Excel test results to the TAP system
- Automates login, upload, and verification
- Generates logs and screenshots
- Moves completed files to a `Done` folder

**Opened from dashboard**
- Click **TAP Uploader**

---

## 📂 Shared Data – Main Files

**Main files** is a **shared data repository**, not a tool.

**Purpose**
- Stores centralized device information in Excel
- Acts as a single source of truth for all tools
- Provides device codes, countries, and serial numbers

**Important**
- Used automatically by tools
- Should not be modified without validation

---

## 🖥️ How Tools Are Used

1. Launch the **Dashboard**
2. Select the required tool
3. Click the corresponding button
4. Follow on‑screen instructions (if any)

✅ No manual script execution is required

---

## ⬇️ How to Download

### Step 1: Install required software
Ensure the following are installed:
- Python (recommended 3.9 or higher)
- Microsoft Excel
- Microsoft Edge
- Git

---

### Step 2: Clone repositories

    git clone https://github.com/<organization-name>/dashboard.git
    git clone https://github.com/<organization-name>/main-files.git
    git clone https://github.com/<organization-name>/<tool-repositories>.git

Clone all repositories into the same parent directory.

---

## ⚙️ How to Set Up on a Computer

### 1️⃣ Recommended folder structure

    automation-root/
    ├── dashboard/
    ├── main-files/
    ├── apply-license/
    ├── band-locker/
    ├── create-test-results-excel-file/
    ├── flash-helper/
    ├── hota-request-message/
    ├── install-aresrt/
    ├── fieldtest/
    ├── hlt/
    └── tap-uploader/

---

### 2️⃣ Environment variables

Some tools require credentials:

    LOGIN_USERNAME
    LOGIN_PASSWORD
    
Set these before starting the dashboard.

---

### 3️⃣ Start working
- Open the dashboard
- Choose a tool
- Click **Run**
- Complete the task

---

## ✅ Usage Guidelines

- Always use the dashboard to open tools
- Do not rename shared Excel files
- Do not change Excel column names
- Do not open Excel files while tools are running
- Keep repositories updated


