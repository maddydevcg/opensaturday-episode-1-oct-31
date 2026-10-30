# Codegnan Open Saturday — Episode 01

**Beyond ChatGPT: Build Your First AI Agent**  
**31 October 2026 | 10:00 AM–2:00 PM | Codegnan Hyderabad**

A hands-on beginner-friendly workshop where students build an **AI Sales Enquiry Agent** with **n8n Cloud** and **Google Gemini**. The agent chats with a prospective learner, gathers useful enquiry details, assigns a suggested priority and drafts a follow-up response.

> **Important:** This is a classroom simulation. The core workflow does **not** send WhatsApp/email, save records to Google Sheets, access Codegnan's CRM, or guarantee any admissions/placement outcomes.

## Quick start

1. Read [Start Here](docs/00_START_HERE.md) and [Setup](docs/Credentials_and_Setup.md).
2. Import [`01_AI_Sales_Enquiry_Agent_CORE.json`](workflows/01_AI_Sales_Enquiry_Agent_CORE.json) into n8n Cloud.
3. Configure your **own** Google Gemini credential in the model node; select an available model.
4. Open the chat and enter: `Hi, I'm a recent graduate interested in Python Full Stack in Hyderabad.`
5. Answer the agent's questions using **fictional details**, then ask it to summarize the lead and draft a follow-up.
6. Follow the [Student Lab](docs/Student_Lab.md).

## Repository contents

```text
.
├── README.md
├── .gitignore
├── LICENSE
├── assets/
│   └── workshop-registration-qr.png
├── data/
│   ├── Sample_Leads.csv
│   └── Question_Bank.csv               # legacy optional demo data
├── docs/
│   ├── 00_START_HERE.md
│   ├── Credentials_and_Setup.md
│   ├── Student_Lab.md
│   ├── Trainer_Guide.md
│   ├── Trainer_Checklist.md
│   └── Troubleshooting.md
├── slides/
│   └── Codegnan_Open_Saturday_Event_01_AI_Sales_Agent.pptx
└── workflows/
    ├── 01_AI_Sales_Enquiry_Agent_CORE.json
    ├── ARCHIVE_Career_Agent_CORE.json
    └── ARCHIVE_Career_Agent_Sheets.json
```

## Workshop agenda

| Time (IST) | Session |
|---|---|
| 10:00–10:20 | Opening: from chatbot to AI agent |
| 10:20–10:40 | Business automation examples |
| 10:40–11:10 | n8n + Gemini architecture |
| 11:10–11:40 | Import and credential setup |
| 11:40–12:10 | First AI enquiry conversation |
| 12:10–12:20 | Break |
| 12:20–12:55 | Guided agent customization |
| 12:55–1:25 | Student challenge |
| 1:25–1:45 | Showcases and safe automation |
| 1:45–2:00 | Q&A and optional next-step bootcamp |

## Workshop and resource links

- [Free workshop registration](https://forms.gle/kM1ooYwDjxaBc4wA9)
- [n8n](https://n8n.io/)
- [Google AI Studio](https://aistudio.google.com/)
- [Trainer Guide](docs/Trainer_Guide.md)
- [Student Lab](docs/Student_Lab.md)
- [Troubleshooting](docs/Troubleshooting.md)

## Trainer readiness

The workflow JSON has been checked for valid structure and internal node references; **it has not been executed against a live n8n Cloud account**. The trainer must import it, connect Gemini, and complete a full dry run before students arrive. The `ARCHIVE_*` workflows demonstrate an earlier career-preparation agent and are **not** the primary Episode 01 project.

## Safety and privacy

Use fictional enquiries during the event. Do not commit API keys, OAuth tokens, personal registration data, private execution logs, or real student contact details. Human approval and appropriate permissions are required before enabling external messaging or lead storage.

## Optional follow-on bootcamp

A proposed five-day AI Automation Bootcamp at **₹499**: lead management, customer support, recruitment, invoice processing, and capstone. This is an optional next step, subject to approved enrollment/payment details.

## Uploading this package to GitHub manually

Open the repository on GitHub, choose **Add file → Upload files**, and upload the extracted folder **contents** while preserving folder paths. If the browser upload does not preserve nested directories, use Git locally:

```bash
git clone https://github.com/maddydevcg/opensaturday-episode-1-oct-31.git
cd opensaturday-episode-1-oct-31
# Copy all extracted package contents here, including hidden .gitignore
git add .
git commit -m "Add Episode 01 trainer kit, sales agent workflow and slides"
git push origin HEAD
```

Do not upload the ZIP itself as the only repository file: extract it first so the README, JSON, slides, and docs are browsable.
