# Telegram Bot Remote

This is a Python-based Telegram bot that allows you to control your Windows system remotely via Telegram commands. The bot can lock the screen, restart, shut down, take screenshots, list processes, and more.

## 🚀 Features
- 🔒 Lock screen  
- 🔄 Restart or ⏻ Shut down the system  
- 📸 Take and send screenshots  
- 📄 List running processes  
- 🌍 Open URLs  
- 🗂 Change directories and list files  
- 💻 Run commands on the system  
- ℹ Retrieve system information  

---

## 🔧 Prerequisites
- A **Windows machine**  
- **Python** installed → [Download Python](https://www.python.org/downloads/)  
- A **Telegram account**  
- A **Telegram bot token** (see instructions below)  

---

## 🤖 Creating a Telegram Bot

1. Open Telegram and search for **BotFather**.  
2. Start a chat with BotFather and send the command:  
3. Follow the instructions to set a **bot name** and **username**.  
4. After successful creation, BotFather will provide a **bot token**. **Save this token**.  
5. To get your **chat ID**, start the bot and send any message. Then visit:  
```bash
https://api.telegram.org/bot<YOUR_TOKEN>/getUpdates
```
6. Look for "chat": {"id": YOUR_CHAT_ID} in the response and save your chat ID.

## 📥 Installation
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/maulik882/telegram-bot-remote.git
cd telegram-bot-remote
```
### 2️⃣ Create and Activate Virtual Environment
```bash
python -m venv venv
venv\Scripts\activate
```
### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Set Up Authentication  
Create an `auth.json` file in the project root with the following format:  

```json
{
    "TOKEN": "your-telegram-bot-token",
    "CHAT_ID": "your-telegram-chat-id"
}
```
### 5️⃣ Rename User_name
Change "USERNAME" With your Actual Username
```bash
if update.message.chat["username"] != "USERNAME":
```
### 6️⃣ Run the Bot
```bash
python bot.py
```

# 🎮 Usage
Start the bot by sending the command:
```bash
/start
```
### Commands
| Command | Description |
|---------|------------|
| `🔒 Lock screen` | Locks the computer screen |
| `⏻ Shutdown` | Shuts down the system immediately |
| `🔄 Restart` | Restarts the system immediately |
| `📸 Take screenshot` | Captures and sends a screenshot |
| `📄 List process` | Lists all running processes |
| `❌ Kill process <process_name>` | Kills a specific process |
| `💻 Run Command <cmd_command>` | Runs a command in CMD |
| `🌍 Open URL <website>` | Opens a URL in the default browser |
| `🗂 Change Directory <path>` | Changes the working directory |
| `📥 Download File <file_path>` | Sends a file from the PC to Telegram |
| `ℹ System Info` | Shows CPU, RAM usage, and system uptime |


# 🤖 Telegram Bot Remote - Contribution Guide

Thank you for considering contributing to the **Telegram Bot Remote**! Your help is greatly appreciated. This guide will help you get started with contributing to the project.

---

## 📌 How to Contribute

### 1️⃣ Fork the Repository
Click the **"Fork"** button at the top right of this repository. This creates your own copy of the project.

### 2️⃣ Clone Your Fork
Clone the repository to your local machine using:
```bash
git clone https://github.com/maulik882/telegram-bot-remote.git
cd telegram-bot-remote
```
### 3️⃣ Create a New Branch
Before making changes, create a new branch to keep things organized:
```bash
git checkout -b feature-branch
```
Replace feature-branch with a relevant name for your changes.
### 4️⃣ Make Your Changes

You can contribute to the **Telegram Bot Remote** in multiple ways:

### 🔧 Fix Bugs 🛠
- Identify and fix reported issues in the [GitHub Issues](https://github.com/maulik882/telegram-bot-remote/issues).
- Debug errors and improve stability.
- Ensure compatibility with different Python versions.

### ⚡ Improve Performance 🚀
- Optimize existing functions for better speed.
- Reduce memory usage and improve efficiency.
- Refactor code for better maintainability.

### 🎉 Add New Features
- Implement new functionality as requested in feature requests.
- Ensure new features **do not break existing ones**.
- Add documentation for any new feature.

### 📝 Improve Documentation 📖
- Improve the **README.md** for better clarity.
- Add more comments to explain complex code.
- Create examples and tutorials for users.

---

### 5️⃣ Test Your Changes

Before submitting, **test your changes** to ensure everything works properly:

### 6️⃣ Commit Your Changes
After making changes, commit them with a clear message:
```bash
git add .
git commit -m "Added feature XYZ"
```

### 7️⃣ Push Your Changes
Upload your changes to GitHub:
```bash
git push origin feature-branch
```
### 8️⃣ Create a Pull Request (PR)
1. Go to the original repository on GitHub.

2. Click the "Pull Requests" tab.

3. Click "New Pull Request".

4. Select your fork and branch.

5. Submit the PR for review.

## 🔥 Contribution Guidelines

✅ Follow the existing code style and project structure.

✅ Keep PRs focused on a single feature or bug fix.

✅ Make sure your code does not break existing functionality.

✅ Test your changes before submitting a PR.

✅ Keep commit messages clear and descriptive.

❌ Do NOT include unnecessary files (e.g., venv, __pycache__, .DS_Store).

❌ Do NOT push directly to the main branch.
