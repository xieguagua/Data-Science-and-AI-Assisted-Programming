# Environment Setup Guide

This guide provides two environment setup options for you to choose from based on your personal needs.

---

## Option A: VS Code + Plugins

This is the de facto standard setup used by programmers and data scientists worldwide, offering unparalleled extensibility and customization.

### 1. Install Python (https://www.python.org/)

- VS Code functions only as a code editor (a "shell"); it requires Python to execute code.
- **Download**: We strongly recommend downloading the latest version (Python 3.10 or higher) directly from the official Python website.
- **Critical Step**: During installation, ensure you check the box labeled "Add Python to PATH" at the bottom of the setup window. This step is essential—omitting it will prevent your system from locating the Python interpreter, rendering code execution impossible.

### 2. Install VS Code (https://code.visualstudio.com/)

- **Download**: Visit the official VS Code website to download the installer for your operating system.
- **Set Up Chinese Language**: Launch VS Code → Click the Extensions icon (square-shaped) on the left sidebar → Search for "Chinese" → Install the language pack and restart VS Code to apply the change.

### 3. Install Core Plugins

In the Extensions Marketplace (left sidebar of VS Code), search for and install the following essential plugins:

- **Python**: Enables VS Code to recognize, syntax-highlight, and run Python code.
- **Jupyter**: Allows you to run code in modular "cells" (similar to lab notebooks), with instant visualization of tables and charts—eliminating the need to execute an entire script at once.

### 4. AI Programming Assistant

This is the key differentiator between your workflow and traditional programming:

- Activate **GitHub Copilot** (or equivalent AI tools) to access support from models like Gemini, Claude, and GPT-4o directly within the editor.

### 5. Configure Aliyun PyPI Mirror (Permanent Global Setting)

To speed up Python package installation (and avoid network issues), configure the Aliyun mirror:

#### For Windows:
1. Navigate to your user directory (e.g., C:\Users\YourUsername\).
2. Create a folder named **pip** (if it does not exist).
3. Inside the pip folder, create a file named **pip.ini**.

#### For Linux/macOS:
1. Navigate to your user directory (e.g., ~/.pip/).
2. Create/modify a file named **pip.conf** (create the .pip folder first if it does not exist).

#### Edit the Configuration File:

Add the following content to pip.ini (Windows) or pip.conf (Linux/macOS):

```ini
[global]
index-url = https://mirrors.aliyun.com/pypi/simple/

[install]
trusted-host = mirrors.aliyun.com
```

Save the file to apply the mirror settings permanently.

---

## Option B: TraeCN (Regularly Updated)

TraeCN is a streamlined, AI-native code editor optimized for data science workflows.

### 1. Install Python

- **Download**: Follow the same steps as Option A (use the official Python website).
- **Critical Step**: Double-click the installer and make sure to check "Add Python to PATH". Without this, TraeCN will fail to detect Python and cannot run any code.

### 2. Install TraeCN (https://www.trae.cn/)

- **Download**: Visit the official TraeCN website to download the installer (supports Windows and macOS).
- **Installation**: Proceed with the default setup (click "Next" through all prompts).
- **Language Configuration**: TraeCN typically auto-detects your system language. If it launches in English:
  - Click the gear icon (Settings) in the bottom-left corner → Select "Settings" → Search for "Display Language" → Choose "Chinese" → Restart TraeCN.

### 3. Intelligent Configuration (No Manual Plugin Hunting)

Unlike VS Code, TraeCN eliminates the need to search for plugins individually—it guides you through setup automatically and supports importing configurations from Cursor or VS Code:

#### First Launch Prompt:
- When opening TraeCN for the first time, you will see a popup asking: "Import VS Code configurations?"
- If VS Code is not installed on your computer, select "Start Fresh" to begin with a clean setup.

#### Install Python Extensions:
- When you create a .py or .ipynb file for the first time, a popup will appear in the bottom-right corner: "Do you want to install the recommended extensions for Python?"
- Click "Install"—TraeCN will automatically install the core Python and Jupyter plugins in the background (no manual searching required).

### 4. Activate Built-in AI Assistant ("Super Manager")

This is TraeCN's biggest advantage over VS Code: AI functionality is natively integrated into the editor (no need to install separate plugins):

- **Location**: Look for a chat bubble icon on the far right (or left) sidebar—this is "Trae Chat".
- **Login**: Click the icon and follow the prompts to log in (no VPN required, with extremely stable network connectivity).
- **Mode Selection**:
  - **Chat Mode**: Acts as a tutor to answer your coding/research questions.
  - **Builder Mode**: Functions as a hands-on assistant to create new files and write code (most commonly used for data science tasks).