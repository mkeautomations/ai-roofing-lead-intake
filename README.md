# ai-roofing-lead-intake
An AI-powered roofing lead qualification system built with n8n OpenAI, Gmail, and Google Sheets.

## Features

- AI lead qualification
- Emergency lead routing
- AI-generated sales notes
- Customer confirmation emails
- Owner notifications
- Google Sheets CRM logging
- Company Settings node for easy customization

## Tech Stack

- n8n
- OpenAI
- Gmail API
- Google Sheets API

## Workflow Overview
<img width="1356" height="409" alt="Screenshot 2026-08-03 211919" src="https://github.com/user-attachments/assets/f49a49c2-7591-4244-979c-f4d31e26f5fb" />
📥 Lead Submission

<img width="877" height="902" alt="Customer Form" src="https://github.com/user-attachments/assets/7f945194-4530-4ecf-b67c-d6e65614ece6" />

🧠 AI Analysis

<img width="910" height="597" alt="AI emergency " src="https://github.com/user-attachments/assets/7faa3499-3205-4454-9edf-13216a40862c" />

🤖 AI Sales Notes

<img width="872" height="613" alt="Sales notes 1" src="https://github.com/user-attachments/assets/3f7849c0-7a9e-4b99-98e1-8d4527d9e4c7" />
<img width="938" height="464" alt="Screenshot 2026-08-03 213652" src="https://github.com/user-attachments/assets/ef3d897b-91fd-4d54-95ba-82f4039e2084" />


### 🚨 Emergency Detection

The workflow automatically prioritizes urgent roofing requests.

A lead is classified as an emergency when:

- AI classifies the request as **High** urgency
- Lead score exceeds the configurable emergency threshold

Emergency leads trigger:

- 🚨 Priority owner email
- AI-generated action plan
- Immediate customer contact recommendation
<img width="782" height="417" alt="Emergency code" src="https://github.com/user-attachments/assets/7c961d58-661b-4297-882c-ecea0452e973" />
<img width="527" height="437" alt="Emergency json" src="https://github.com/user-attachments/assets/5cd6e5d0-db2e-4058-bdb1-782b2fe68505" />
<img width="1025" height="568" alt="Screenshot 2026-08-03 214857" src="https://github.com/user-attachments/assets/75a9f9e4-dede-4061-948a-c5fa09bd373c" />



📧 Owner Notification

<img width="1508" height="426" alt="Email" src="https://github.com/user-attachments/assets/98a43f6a-7ef7-479e-90b7-4defa6b7d936" />
<img width="1265" height="367" alt="custo info" src="https://github.com/user-attachments/assets/abb25513-febd-4fee-86a3-02f73f121930" />


### 📊 Lead Tracking

Every submission is automatically logged to Google Sheets with:

- Customer information
- AI lead analysis
- Urgency
- Lead score
- Project value
- Customer sentiment
- Recommended action

This creates a searchable lead database for the business.
↓<img width="1897" height="412" alt="Screenshot 2026-08-03 222207" src="https://github.com/user-attachments/assets/f3e80910-e85e-42ea-8e7f-55421f5f0a49" />


📨 Customer Confirmation
<img width="1516" height="442" alt="Screenshot 2026-08-03 220631" src="https://github.com/user-attachments/assets/be2589c7-d407-4428-b29d-3f9d34d5cc25" />
