<!DOCTYPE html>
<html>
<head>
    <title>Important Terminal Commands</title>
</head>
<body>
    <pre>
# ----------------------------------------------------------------------
# WINDOWS INSTALLATION COMMANDS (Use PowerShell or CMD as Administrator)
# ----------------------------------------------------------------------

# 1. INSTALL/UPDATE WINGET (Windows Package Manager)
# This must be run first in an elevated (Administrator) PowerShell terminal.
Add-AppxPackage -Path https://aka.ms/getwinget -WhatIf:$false

# 2. INSTALL PYTHON (Prerequisite for Pip)
winget install Python.Python3 --silent --scope machine

# 3. UPGRADE PIP (Python Package Installer)
# Run after Python installation.
python -m pip install --upgrade pip

# 4. INSTALL NODE.JS (Prerequisite for NPM/Gemini CLI)
# Installs the Node.js LTS (Long Term Support) version.
winget install OpenJS.NodeJS.LTS --silent --scope machine

# 5. INSTALL GEMINI CLI (Command Line Interface)
# Requires Node.js/NPM to be installed first.
npm install -g @google/gemini-cli


# ----------------------------------------------------------------------
# MACOS/LINUX INSTALLATION COMMANDS (Use Bash/Zsh Terminal)
# ----------------------------------------------------------------------

# 1. INSTALL HOMEBREW (The macOS Package Manager)
# This is the official installation script.
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# 2. INSTALL NODE.JS
# Uses Homebrew to install the latest Node.js.
brew install node

# 3. INSTALL/UPGRADE PIP (Python Package Installer)
# Ensures Pip is up-to-date for Python 3 (which is included or installed via Brew).
python3 -m pip install --upgrade pip

# 4. INSTALL GEMINI CLI (Command Line Interface)
# Uses the Homebrew package for the CLI.
brew install gemini-cli
    </pre>
</body>
</html>
