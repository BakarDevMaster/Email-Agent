# 📧 Email Assistant Agent

A smart, AI-powered Email Assistant that can **read, summarize, categorize, and send emails** on behalf of the user. Built with Python, `agents` framework, and Google Gemini (`gemini-2.0-flash`) model via the OpenAI-compatible API interface.

---

## 🚀 Features

* **Email Reading**:

  * Fetch emails from Gmail inbox (or other folders).
  * Summarize sender, subject, and body.
  * Filter by date range and limit number of emails.

* **Email Replying & Sending**:

  * Draft professional replies.
  * Send new emails with attachments.
  * Maintain contextual tone (professional, casual, friendly).

* **Inbox Management**:

  * Categorize emails (urgent, informational, spam).
  * Detect ongoing threads and conversations.
  * Track unresolved action items.

* **AI-Powered Assistance**:

  * Context-aware responses.
  * Summarization of multiple emails.
  * Follow-up suggestions.

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

### 2. Create and Activate Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file in the project root with the following keys:

```
GEMINI_API_KEY=your_gemini_api_key
EMAIL_ADDRESS=your_email@gmail.com
EMAIL_APP_PASSWORD=your_app_password
```

⚠️ **Note**: Use a Gmail App Password (not your regular Gmail password). You can generate it from your Google Account Security settings.

### 5. Run the Assistant

```bash
python main.py
```

---

## 🛠️ Usage Examples

* **Summarize Emails**

  ```
  Enter the query: Summarize my last 5 emails.
  ```

* **Reply to Email**

  ```
  Enter the query: Reply to John saying I’ll join the meeting at 3 PM.
  ```

* **Send New Email**

  ```
  Enter the query: Send an email to hr@example.com with subject 'Leave Request' and body 'I’d like to apply for leave from June 10 to June 15.'
  ```

---

## 📡 Tech Stack

* **Language**: Python 3.10+
* **Libraries**:

  * `openai` (OpenAI-compatible Gemini client)
  * `agents` framework
  * `imaplib`, `smtplib` for email handling
  * `python-dotenv` for environment variables
* **Model**: `gemini-2.0-flash` (via OpenAI API-compatible interface)

---

## 🔐 Security Notes

* Never commit `.env` files or API keys to GitHub.
* Always add `.env` to `.gitignore`.
* Use Gmail App Passwords instead of your main password.

---

## 📜 License

This project is provided for **educational and personal use**. Please ensure you comply with Gmail and API provider terms of service when deploying.

---

## 👤 Author

Developed by **M Abubakar**
For queries, reach out via email or GitHub issues.
