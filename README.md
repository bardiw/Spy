# 🔐 Multi-Feature Data Capture Tool (Keylogger, Webcam, Screenshot, Chrome Passwords)

> ⚠️ **DISCLAIMER**: This project is intended for **educational and ethical purposes only**. Unauthorized usage may violate privacy laws and local regulations. Always obtain **explicit permission** before using such tools on any system that is not your own.

---

## 🧠 Description

This Python-based tool integrates **multiple powerful data-capturing features** into one script. It can:
- 🧾 Log keystrokes (Keylogger)
- 📷 Capture an image from the webcam
- 🖥️ Take a screenshot of the current screen
- 🔐 Extract saved passwords from Google Chrome

---

## 🚀 Features

| Feature            | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| 🎹 Keylogger        | Logs all keystrokes for 10 seconds and saves to `kl.txt`.                  |
| 📸 Webcam Capture   | Takes a single image from the default webcam and saves as `spycam.png`.    |
| 🖼️ Screenshot        | Captures a full-screen screenshot and saves it as `screenshot.png`.        |
| 🔑 Chrome Passwords | Extracts saved Chrome credentials and writes to `ch_pass.txt`.             |

---

## ⚙️ Requirements

Install all dependencies with pip:

```bash
pip install pynput opencv-python pyautogui pycryptodomex pypiwin32
```

---

## 🧰 How It Works
1. Keylogger
- Captures keystrokes for 10 seconds.

-  Logs standard keys and maps special keys (Enter, Space, etc.).

-  Stores results in kl.txt.

2. Webcam Capture
-  Captures a single frame using OpenCV and saves it as spycam.png.

3. Screenshot
-  Takes a screenshot using pyautogui and saves it as screenshot.png.

4. Chrome Password Extraction
-  Uses win32crypt and Cryptodome to decrypt the Chrome password database.

-  Saves readable credentials to ch_pass.txt.

⚠️ Works only on Windows, as it accesses system-specific Chrome storage files.

---

## 📂 Output Files
kl.txt – Contains logged keystrokes.

spycam.png – Captured webcam image.

screenshot.png – Screenshot of the current screen.

ch_pass.txt – Extracted saved passwords from Chrome.

---

## 🛡️ Legal & Ethical Use
This tool demonstrates system vulnerabilities for educational cybersecurity research. Misusing it could:

- Violate privacy laws (e.g., GDPR, HIPAA)

- Breach ethical and professional codes

- Lead to prosecution or academic sanctions

✔️ Always test on systems you own or with explicit written consent.

---

## ❗ Important Notes
- Chrome password extraction only works on local accounts with unencrypted login storage.

- Antivirus software may flag this script as malicious due to its behavior.

- The script currently runs all modules sequentially. You can modularize them for specific use cases.

--- 

## 📌 To Do
* Add OS checks (Windows-only logic)

* Add email sending for logs (optional & controlled)

* Modularize features (toggle via CLI flags or UI)


