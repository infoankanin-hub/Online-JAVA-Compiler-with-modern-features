# ☕ Secure Web-Based Java IDE & Compiler

[![Live Demo](https://img.shields.io/badge/Live_Deployment-GitHub_Pages-success?style=for-the-badge&logo=github)](YOUR_GITHUB_PAGES_LINK_HERE)
[![Security Focus](https://img.shields.io/badge/Security-Anti--Plagiarism_Enabled-red?style=for-the-badge&logo=shield)](YOUR_GITHUB_PAGES_LINK_HERE)
[![Code Quality](https://img.shields.io/badge/Code-Clean_Architecture-blue?style=for-the-badge)](#)
[![Status](https://img.shields.io/badge/Status-Active_Development-brightgreen?style=for-the-badge)](#)

A browser-based Java execution environment engineered specifically for academic assessments and technical interviews. This platform allows users to write, compile, and debug Java code in real-time while strictly enforcing original problem-solving by neutralizing external copy-paste mechanisms.

---

## 📖 Table of Contents
- [The Engineering Challenge](#-the-engineering-challenge)
- [Core Features](#-core-features)
- [System Architecture](#%EF%B8%8F-system-architecture)
- [Technical Stack](#-technical-stack)
- [Installation & Local Setup](#-installation--local-setup)
- [Development Roadmap](#-development-roadmap)

---

## 🎯 The Engineering Challenge

Standard online IDEs are optimized for convenience. However, in remote learning and assessment environments, this convenience becomes a vulnerability. It is incredibly easy for users to paste pre-written solutions, bypassing the actual evaluation of their logic and syntax skills.

**The Solution:** I engineered this compiler to act as a "secure sandbox" at the DOM level. By intercepting specific keyboard and mouse events, the interface forces the user to write their logic from scratch, ensuring high-integrity evaluation.

---

## ✨ Core Features

### 🛡️ Anti-Plagiarism Protocol (DOM Security)
* **Clipboard Blocking:** Systematic nullification of `Ctrl+C`, `Ctrl+V`, and `Ctrl+X` within the editor window.
* **Context Menu Disablement:** Right-click actions are suppressed to prevent mouse-based pasting.
* **Drop Interception:** Prevents users from dragging and dropping text files directly into the code execution window.

### 💻 Execution & UX
* **Real-Time Compilation:** Sends raw text payloads to the compilation engine and returns `stdout` or `stderr` instantly.
* **Distraction-Free UI:** A minimalist, dark-mode focused interface designed to mimic professional environments like VS Code or IntelliJ.
* **Responsive Design:** Fully fluid layout adapting to desktop and tablet viewports.

---

## ⚙️ System Architecture

*(Note: Update the backend section below based on how your app currently compiles code)*

1. **Client Layer (Browser):** Captures user keystrokes and enforces security policies via JavaScript Event Listeners.
2. **Payload Generation:** Packages the raw Java string into a JSON format.
3. **Execution Engine (Backend API):** Receives the JSON payload, spins up an isolated execution thread/container, compiles the `.java` file, and captures the output.
4. **Response Handling:** The frontend parses the API response and renders either the successful output or the stack trace formatting for errors.

---

## 🛠 Technical Stack

| Component | Technology Used | Purpose |
| :--- | :--- | :--- |
| **Frontend Structure** | HTML5 | Semantic layout and editor structure |
| **Styling & Layout** | CSS3 | Responsive grid/flexbox and syntax visuals |
| **Logic & Security** | Vanilla JavaScript | DOM manipulation, API fetching, event interception |
| **Deployment** | GitHub Pages | Continuous integration and live hosting |

---

## 🚀 Installation & Local Setup

To run this environment locally on your machine:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/infoankanin-hub/Online-JAVA-Compiler-with-modern-features.git](https://github.com/infoankanin-hub/Online-JAVA-Compiler-with-modern-features.git)
