# APRS
AI-Powered WhatsApp Consistency Bot – Automates and personalizes WhatsApp replies using free AI tools, ensuring consistent tone, quick response times, and secure message handling.
# 🤖 AI-Powered WhatsApp Consistency Bot

## 📌 Overview
This project automates and personalizes WhatsApp replies using **AI and free tools** — no paid APIs required.  
It ensures:
- Consistent tone matching your personal style.
- Faster, automated response times.
- Secure handling of private data.

Built with:
- **Python**
- **Google Colab** (Free GPU for training)
- **Hugging Face Transformers**
- **Selenium / PyWhatKit** for automation

---

## 📂 Features
✅ Export and parse WhatsApp chats into structured data.  
✅ Label messages for tone & urgency (manual + rule-based).  
✅ Train a **DistilBERT** model to predict reply style.  
✅ Generate replies from pre-defined templates.  
✅ Send automated responses via WhatsApp Web.  
✅ Fully local — no paid APIs or cloud storage required.

---

## 📊 Flowchart
![Flowchart](whatsapp_ai_flowchart.png)

---

## 🚀 Getting Started

### 1️⃣ Clone Repository
```bash
git clone https://github.com/Zakir176/APRS.git
cd whatsapp-ai-bot
```
2️⃣ Export WhatsApp Chat
On Android: Chat → 3 dots → Export chat (No media)

On iPhone: Use iExplorer (Free trial)

3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```
4️⃣ Parse Chat Data
```bash
python parse_chats.py
```
5️⃣ Label Messages
Edit the generated CSV in Excel/Google Sheets.

Add columns: tone and urgency.

6️⃣ Train Model (Google Colab)
Open train_model.ipynb in Google Colab.

Upload your labeled CSV.

Fine-tune DistilBERT.

Save model to my_whatsapp_model/.

7️⃣ Automate Replies
```bash
python send_replies.py
```



⚠️ Privacy & Ethics
Always disclose AI usage to close contacts.

Never commit your personal chat exports to a public repo.

Keep sensitive data in .gitignore.

🛠️ Requirements
Python 3.8+

Google Chrome (for Selenium)

WhatsApp Web

Hugging Face transformers

Pandas

Selenium

PyWhatKit

