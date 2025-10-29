แน่นอนครับ phayao ✨  
ด้านล่างนี้คือเนื้อหาของไฟล์ `.gitignore` และ `README.md` ที่เหมาะกับโปรเจกต์ e-learning automation bot ของคุณ:

---

## 📄 .gitignore

```gitignore
# Virtual environment
env/
venv/

# Python cache
__pycache__/
*.pyc

# Cookies and session data
cookies.json

# Screenshots
screenshot.png

# Logs
*.log

# OS-specific
.DS_Store
Thumbs.db
```

> ไฟล์นี้ช่วยให้ Git ไม่ track ไฟล์ที่ไม่จำเป็น เช่น cookies, env, cache, และภาพ screenshot

---

## 📘 README.md

```markdown
# E-Learning Automation Bot

This project automates learning on the OCSC Learning Portal using Selenium. It handles login via cookies, tracks lesson progress, and sends real-time updates via Telegram.

---

## 🚀 Features

- Auto-login using saved cookies
- Session recovery with QR/Verify prompt
- Learning time tracking until completion
- Telegram notifications (text + screenshot)
- Screenshot capture on key events
- Robust error handling and session persistence

---

## 📁 Project Structure

```
e-learning-bot/
├── main.py              # Main automation script
├── config.py            # Configuration for URL and Telegram
├── cookies.json         # Saved login cookies (ignored by Git)
├── requirements.txt     # Python dependencies
├── run_main.bat         # Windows batch file to run the bot
├── screenshot.png       # Screenshot sent to Telegram (generated during runtime)
└── .gitignore           # Files to exclude from Git tracking
```

---

## ⚙️ Setup Instructions

### 1. Create virtual environment

```bash
python -m venv env
env\Scripts\activate
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure Telegram

Edit `config.py`:

```python
course_url = "https://learningportal.ocsc.go.th"
TELEGRAM_BOT_TOKEN = "your_bot_token"
TELEGRAM_CHAT_ID = "your_chat_id"
```

---

## ▶️ Running the Bot

Double-click `run_main.bat` or run manually:

```bash
python main.py
```

> The bot will check internet connection, activate the environment, and start the automation.

---

## 📸 Telegram Notifications

The bot sends:
- Start and completion messages for each lesson
- Screenshot of login/verify page if session expires
- Final screenshot when the program ends

---

## 🛠️ Notes

- Make sure Chrome and ChromeDriver versions match
- Cookies are saved to `cookies.json` after successful login
- If cookies are missing or expired, manual login is required once

---

## 📌 License

This project is for educational and internal automation purposes only.
```

---

คุณสามารถ copy เนื้อหานี้ไปวางในไฟล์ `.gitignore` และ `README.md` ได้ทันที  
ถ้าต้องการให้ผมช่วยสร้าง template ZIP พร้อมไฟล์ทั้งหมด หรือ deploy ขึ้น GitHub ก็แจ้งได้เลยครับ
