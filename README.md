# Ollama-File-Manager-MacOS64
A lightweight (12mb), native macOS file manager powered by Ollama. Browse, search, and manage your files with the help of AI-backed  insights and tagging — all in a simple, fast, and offline-first desktop app.

# OllamaFM 

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg) ![Platform](https://img.shields.io/badge/platform-macOS%20%7C%20Linux-lightgrey.svg) ![Status](https://img.shields.io/badge/status-stable-success.svg)

**OllamaFM** is a high-performance, asynchronous Terminal User Interface (TUI) file manager designed for developers. It combines classic file navigation with local AI intelligence, automated Git context, and smart cloud storage handling.

Unlike standard file managers, OllamaFM runs on a non-blocking game loop (20 FPS), ensuring the interface remains fluid even while scanning gigabytes of code or waiting for network responses.

---

## 🚀 Key Features

### 1. 🧠 AI Code Reviews (Local)
Integrated with **[Ollama](https://ollama.com/)** to provide instant, privacy-focused code reviews.
- **Privacy First:** Your code never leaves your machine.
- **Background Scanning:** Start a scan on one folder and keep working elsewhere.
- **Supported Models:** Automatically detects any model installed via Ollama (e.g., `llama3`, `mistral`, `deepseek-coder`).

### 2. ⚡️ Async Git Integration
Never wait for `git status` again.
- **Live Context:** Automatically detects repositories, branches, and remote origins.
- **Smart Filtering:** Only shows changes relevant to the *current* folder (ignoring sibling directories).
- **Background Fetching:** Git checks run in invisible threads, preventing UI freeze.
- **Repo Links:** Displays dimmed links to remote repositories (GitHub/GitLab).

### 3. ☁️ Smart iCloud Hydration
Solves the "hanging terminal" issue on macOS.
- **Dataless Detection:** Identifies files that exist in metadata but aren't downloaded.
- **Mini-Pie Chart:** Visualizes download progress (`○ ◔ ◑ ◕ ●`) in the control panel.
- **Selective Sync:** Downloads *only* relevant source files for inspection, automatically ignoring heavy folders like `node_modules` or `.git`.

### 4. 🧹 Maintenance Tools
- **Orphan Pruning:** Scans text files to find assets (images/scripts) that are never referenced in your code, allowing you to move them to a `PRUNED_ASSETS` folder.

---

## 🛠 Installation

### Prerequisites
1. **Python 3.8+**
2. **Ollama:** Must be installed and running.
