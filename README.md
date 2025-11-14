Installation Request Agent (n8n Workflow)

This project is a simple but powerful AI-driven automation workflow built using n8n (open-source automation tool).
It collects installation requests through a form, checks if the preferred date is within 7 days, and automatically sends a notification to Slack.

✨ Features
🔹 1. Form Submission Trigger

Users fill a form with:

Email Address

Preferred Installation Date

The workflow starts as soon as the form is submitted.

🔹 2. Automatic Date Validation

The workflow checks:

Is the preferred installation date within the next 7 days?

✔️ If YES: A Slack notification is sent

❌ If NO: The workflow continues to a placeholder node (for future actions)

🔹 3. Slack Notification

If the request is within 7 days, the workflow sends a message to a Slack channel including:

User’s email

Requested installation date

This helps teams get real-time alerts for urgent installations.

🧩 Workflow Logic (Summary)

Form Trigger → Captures user details

IF Node → Checks if date ≤ 7 days from today

Slack Node → Sends notification

TODO Node → For requests outside 7 days (customize later)

📁 Files Included

workflow.json — The full n8n workflow to import directly

This README

▶️ How to Use
🔸 1. Import Workflow

Go to n8n → Workflows → Import from File
Select workflow.json.

🔸 2. Configure Credentials

You'll need:

Slack OAuth2 credentials

n8n Form Trigger webhook (auto created)

🔸 3. Publish

Activate the workflow — your automation is live!
link:https://zeelshah1205.app.n8n.cloud/form/1749f99f-640f-4b6f-884e-7d408853f20e


<img width="509" height="489" alt="ai-1" src="https://github.com/user-attachments/assets/8551b8a0-9180-445e-bc41-f9bd2f4c51c0" />
<img width="468" height="472" alt="ai-2" src="https://github.com/user-attachments/assets/14bda580-fcf6-4dc0-88a3-7f56dce2b91b" />
<img width="1293" height="550" alt="ai-3" src="https://github.com/user-attachments/assets/2b771ced-d20d-49a5-a100-f5f20a4adb1d" />
<img width="253" height="101" alt="ai-4" src="https://github.com/user-attachments/assets/71c9023a-f2a1-4d98-a122-f68c5e16d73f" />

🚧 Future Improvements

Auto-email reply to the user

Link with a scheduling system

Add AI-generated response messages

Store form entries in Google Sheets / Notion

Notify via WhatsApp or SMS

Build a UI for the form

💡 Why This Exists

This workflow makes installation scheduling easier, faster, and more automated.
Great for SaaS, services, or field installation businesses.


