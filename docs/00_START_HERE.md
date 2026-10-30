# START HERE — Codegnan Open Saturday, Episode 01

**Date:** 31 October 2026 | **Time:** 10 AM–2 PM | **Location:** Codegnan Hyderabad  
**Theme:** Beyond ChatGPT — Build Your First AI Agent  
**Primary project:** AI Sales Enquiry Automation Agent using n8n Cloud + Google Gemini.

## Start in 5 minutes
1. Open `slides/Codegnan_Open_Saturday_Event_01_AI_Sales_Agent.pptx`.
2. Read `docs/Trainer_Checklist.md` and `docs/Credentials_and_Setup.md`.
3. In n8n Cloud, import `workflows/01_AI_Sales_Enquiry_Agent_CORE.json`.
4. Connect your own Gemini credential and select a supported model.
5. Test with `Hi, I'm a final-year student interested in Python Full Stack in Hyderabad.`
6. Follow `docs/Student_Lab.md` for the classroom exercise.

## What works vs. what is conceptual
- **Core import:** n8n chat trigger → AI agent → Gemini model, with memory and calculator tool. Produces a **structured lead summary and draft follow-up** in chat.
- **Not connected by default:** Google Sheets saving, email sending, WhatsApp messaging, real CRM, payments. Never claim a lead was saved or a message sent.
- **Archive:** The two `ARCHIVE_Career_Agent_*.json` workflows belong to an earlier career-preparation demo and are NOT the main Episode 01 lab.
- **Validation:** Core workflow JSON is structurally checked but **not tested against a live n8n tenant**. Complete trainer rehearsal before the event.

## Links
- Free workshop registration: https://forms.gle/kM1ooYwDjxaBc4wA9
- Event repository: https://github.com/maddydevcg/opensaturday-episode-1-oct-31
- n8n: https://n8n.io/ | Google AI Studio: https://aistudio.google.com/

## Privacy
Use fictitious enquiries during the demo. Do not commit API keys, OAuth tokens, real student phone numbers, registration exports, or execution logs containing personal data.
