# 📋 Google Sheets to Slack Alert Automation (n8n)

Automate alerts from a Google Sheet into Slack using n8n.  
This is part of a 40-day automation challenge (Day 1 – Project 2).

---

## 🛠️ Project Overview

📌 **Goal:**  
Send an alert to Slack whenever a new row is added in a Google Sheet.

🧰 **Tech Stack:**
- n8n (Self-hosted or Cloud)
- Google Sheets (with OAuth2)
- Slack Webhooks (Incoming)

---

## 📸 Example Slack Message

📋 New Task Entry:
• Name: Saad
• Email: saadtahir009@gmail.com
• Task: Follow UP with Clients

---

## 📂 Folder Structure

```
n8n-google-sheets-to-slack-alert/
│
├── workflow.json # Exported n8n workflow (you can import directly)
├── screenshots/
│   ├── workflow-ui.png # Screenshot of n8n flow
│   └── slack-message.png # Output message in Slack
└── README.md # Project documentation
```

---

## 🧩 Nodes in Workflow

1. **Google Sheets Trigger**
   - Triggers when a new row is added
2. **Set Node**
   - Formats the Slack message
3. **HTTP Request**
   - Sends the message to a Slack channel via webhook

---

## 🔐 Setup Instructions

### 🔹 Google Sheets
- Create a Google Sheet with columns: `NAME`, `EMAIL`, `TASK`
- Connect Google account using OAuth2 in n8n
- Use **Google Sheets Trigger** node in n8n

### 🔹 Slack
- Create a [Slack App](https://api.slack.com/apps)
- Enable **Incoming Webhooks**
- Generate a webhook URL (e.g. `https://hooks.slack.com/services/...`)
- Use it in HTTP Request node

---

## 🚀 How to Use

1. Import the `workflow.json` into n8n
2. Update:
   - Google Sheets Trigger → your sheet
   - HTTP Node → your Slack webhook URL
3. Activate the workflow
4. Add a new row in the Google Sheet
5. Check your Slack channel for the alert 🎉

---

## 📸 Screenshots

The following screenshots are included in the `/screenshots` folder:

- `workflow-ui.png`: Full n8n workflow layout
- `slack-message.png`: Message received in Slack

---

## 🧠 Learning Outcome

- Using Google Sheets as a trigger source
- Formatting data with JavaScript expressions
- Sending JSON payloads to external services

---

## 👨‍💻 About the Author

This project was created by Ahmad Raza, a skilled freelancer specializing in automation and development. 

If you want to connect, let's connect there:  
- [LinkedIn](https://www.linkedin.com/in/ahmad-raza-403bbd0278)

If you want the service, let's get the service done for you:  
- [Fiverr](https://www.fiverr.com/sellers/nitrola/)
