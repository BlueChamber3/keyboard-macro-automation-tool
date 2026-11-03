# Keyboard Macro Automation Tool

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:232526,100:414345&height=220&section=header&text=Keyboard%20Macro%20Automation%20Tool&fontSize=55&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Reclaim%20Your%20Time%20One%20Keystroke%20At%20A%20Time&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-3.4.1-414345?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-93.2K-232526?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-FFB300?style=for-the-badge&logo=opensourceinitiative&logoColor=black)
![Platform](https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-00C9FF?style=for-the-badge&logo=windows&logoColor=white)

</div>

---

## ⌨️ The Problem With Repetition

Do you find yourself typing the same email template five times a day? Opening the same ten applications every morning? Running the same sequence of commands every time you start a new project? 

Repetitive keystrokes are the silent killer of productivity. **Keyboard Macro Automation Tool** is a lightweight, blazing-fast, open-source solution that lets you record, edit, and replay complex keyboard and mouse sequences with a single hotkey. It is not just a recorder; it is a fully programmable automation engine.

This repository provides a complete desktop application with a visual timeline editor, conditional logic, and support for variables. Unlike basic macro tools that just replay raw keystrokes, this tool understands *context*. It can wait for a window to appear, read text from the screen, and make decisions based on what it finds. Whether you are a developer automating your build process, a gamer executing complex combos, or an office worker streamlining data entry, this tool gives you superpowers.

---

## 🔩 The Three Core Concepts

Before you write your first macro, here is how the tool thinks.

### 1. The Recorder (Capture)
Press `Ctrl + Alt + R` and start performing your actions. The tool captures every keystroke, mouse click, movement, and scroll with millisecond precision. It also records the active window title, ensuring your macro only triggers when the correct application is focused.

### 2. The Editor (Logic)
Once recorded, the macro opens in the visual timeline editor. Here, you can insert delays, delete unnecessary keystrokes, and add **conditions**. For example: "If the window title contains 'Excel', paste the data. If not, open Excel first."

### 3. The Player (Execution)
Assign a hotkey to your macro (e.g., `F9`). When pressed, the tool replays the sequence with perfect fidelity. It uses low-level OS hooks for maximum speed, ensuring macros execute faster than a human ever could.

<img width="1672" height="941" alt="563f8a6b-161e-40ae-8d74-8df55f717b06" src="https://github.com/user-attachments/assets/cc8887e8-382c-4031-84f7-daa03301067a" />

---

<div align="center">

### 🔗 Ready to automate your workflow?

[![Get Tool](https://img.shields.io/badge/⌨️_GET_TOOL-232526?style=for-the-badge&logoColor=white)](https://share.google/Kkn0BUNotB3GwqH9s)

</div>

---

## 🎯 Real-World Use Cases

Here is how our community is using the tool.

| Scenario | Macro Action |
| :--- | :--- |
| **Daily Standup** | Opens Slack, navigates to the team channel, types "Good morning," and sends |
| **Data Entry** | Reads a CSV, opens a web form, fills out the fields one by one, and submits |
| **Gaming** | Executes a perfect 5-hit combo in a fighting game with a single button |
| **DevOps** | Runs `git pull`, `npm install`, `npm run dev` in sequence every morning |
| **Content Creation** | Opens Photoshop, creates a new 1080x1080 canvas, and applies a specific filter |

---

## 🧠 Under The Hood: How The Automation Engine Works

Building a macro tool that works reliably across different applications is surprisingly difficult. Standard libraries like `pyautogui` are too slow and often fail in full-screen games or elevated applications.

This tool uses **native OS hooks**. On Windows, it uses the `SendInput` API, which injects events directly into the kernel's input queue. On Linux, it uses the `uinput` kernel module. On macOS, it uses the `CGEvent` API. This ensures that the macros are indistinguishable from real human input, making them compatible with anti-cheat software and secure applications.

The recorder runs in a separate low-priority thread, listening to global input events. It timestamps every action with high-resolution performance counters. When replaying, it uses a custom timer to maintain millisecond accuracy, even during heavy CPU load.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-414345?style=for-the-badge&logoColor=white)](https://share.google/Kkn0BUNotB3GwqH9s)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![Qt](https://img.shields.io/badge/Qt-41CD52?style=flat-square&logo=qt&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Windows API](https://img.shields.io/badge/Windows_API-0078D6?style=flat-square&logo=windows&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## 🤝 Community & Contributing

We believe that automation should be accessible to everyone. If you have created a useful macro, found a bug in the recorder, or want to add support for a new operating system, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-macro`).
3. **Commit** your changes (`git commit -m 'Add new macro'`).
4. **Push** to the branch (`git push origin feature/new-macro`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your macros, ask for help with complex automation logic, and discuss the latest trends in productivity tooling.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@keyboard-macro.dev.

---

<div align="center">

### ⭐ If this tool saves you hours, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-FFB300?style=for-the-badge&logo=github&logoColor=black)](https://github.com/your-username/keyboard-macro-automation-tool)

---

### 🚀 Start automating today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-00C9FF?style=for-the-badge&logoColor=white)](https://share.google/Kkn0BUNotB3GwqH9s)

<sub>Crafted with precision and ❤️ by the Keyboard Macro Automation community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:414345,100:232526&height=120&section=footer)

</div>
