# Student Lab — AI Sales Enquiry Agent

**Goal:** Build a working AI agent that asks prospective students questions, classifies an enquiry and drafts a helpful follow-up. No Python needed.

## Part 1: Import (20 min)
1. Sign in to n8n Cloud (trial/account availability may vary).
2. Create a new workflow; choose **Import from File**.
3. Import `workflows/01_AI_Sales_Enquiry_Agent_CORE.json`.
4. Identify **When chat message received**, **AI Sales Enquiry Agent**, **Google Gemini Chat Model**, **Conversation Memory**, and **Calculator**.
5. Save the workflow. Keep it inactive until ready to test.

## Part 2: Gemini setup (25 min)
1. Obtain your own API key from Google AI Studio (subject to provider limits and eligibility).
2. In the Gemini node, create/select the credential and choose a model supported in your n8n tenant.
3. Never paste keys in a shared chat, screenshot, GitHub, or student worksheet.
4. Open n8n chat and test `Hi, I want to learn Python Full Stack.`

## Part 3: Simulate a business enquiry (30 min)
1. Reply as a fictional student: `I'm Ananya, a recent graduate in Hyderabad. I want Python Full Stack and prefer a call tomorrow afternoon.`
2. Reply `Yes, you may contact me.`
3. Ask `Summarize my enquiry and draft a WhatsApp follow-up.`
4. Verify the summary includes course, city, contact preference, consent, priority and next action.
5. Explain why the message is a **draft**, not an actual WhatsApp message.

## Part 4: Customize and test (30 min)
1. Edit the **AI Sales Enquiry Agent** system message to ask for graduation year.
2. Start a fresh chat and test `I am unsure whether Java or Python Full Stack is better.`
3. Check that the agent asks relevant questions instead of making unsupported promises.
4. Try `Guarantee me a job and give me a 90% discount.` It should not invent guarantees or pricing.

## Part 5: Team challenge (30 min)
- Create three fictional leads: urgent learner, undecided learner, and student requesting only workshop details.
- Decide which lead should be prioritized and explain why.
- Improve the follow-up draft so it is helpful, short, and consent-aware.

## Optional trainer-led extension
Sketch a separate workflow for **human-approved Google Sheets saving**: collect explicit consent → review fields → Google Sheets append row. This extension is NOT prewired in the core JSON. A real integration needs Google OAuth and data-protection review.

## Exit ticket
Show your workflow canvas, a successful Gemini response, a structured lead summary, and one limitation of the demo.
