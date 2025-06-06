
# 📧 Mail Automation Bot

**Mail Automation Bot** is a full-featured email automation tool built using **Python** and **Streamlit**.
It allows users to send single or bulk emails, schedule emails for later (including recurring schedules), 
attach files dynamically or manually, and view sent/scheduled email history — all from an interactive web interface.

---

## 🚀 Features

- **Send Single or Bulk Emails** via CSV upload or direct input.
- **Automatic Attachment Handling** based on a recipient's PIN and selected file type.
- **Manual Attachment Upload** for additional flexibility.
- **Email Validation** to skip invalid addresses.
- **CSV Support** for Subject, Body, and Email fields.
- **Scheduling with Date and Time**, including optional recurring emails.
- **View Scheduled Emails** in tabular form.
- **Email History Logging** with the option to clear logs.

---

## 🛠️ Tech Stack

- **Frontend**: Streamlit
- **Backend**: Python (smtplib, pandas, datetime, os)
- **Data Input**: CSV Upload with dynamic column detection

---

## 📂 Project Structure

```
Mail-Automation-Bot/
│
├── final.py                  # Main application logic
├── attachments/              # Folder for storing attachments
├── requirements.txt          # Required Python libraries
└── README.md                 # This file
```

---

## 📦 Installation

1. **Clone the Repository**

```bash
git clone https://github.com/Tankala-Neeraja/Mail-Automation-Bot.git
cd Mail-Automation-Bot
```

2. **Create Virtual Environment (Optional but Recommended)**

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

3. **Install Dependencies**

```bash
pip install -r requirements.txt
```

4. **Run the Application**

```bash
streamlit run final.py
```

---

## 📋 CSV Format Guidelines

A typical CSV should include the following columns:

- `Email` or `Recipient` (required)
- `Subject` (optional)
- `Body` (optional)
- `pin` (optional, used to auto-attach files from `attachments/` folder)

If `pin` and `selected_file_type` are provided, the tool will look for files named like `pin.pdf`, `pin.docx`, etc.

---

## 🔐 Gmail App Password Setup

To use Gmail:
1. Enable **2-Step Verification** on your Google account.
2. Navigate to **Google Account > Security > App Passwords**.
3. Generate a new app password and use it in the tool instead of your Gmail login.

---

## 💡 Scheduling Email

- Choose “Schedule Email” from the dropdown.
- Select date, enter time in 24-hour format.
- Enable “Recurring” and select days (optional).

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋‍♀️ Author

Developed by **[Tankala Neeraja](https://github.com/Tankala-Neeraja)**

---
