# 🏠 AI Roofing Office Assistant

An end-to-end AI-powered lead intake and qualification system built with **n8n**, **OpenAI**, **Gmail**, and **Google Sheets**.

## About

Small roofing companies often spend valuable time manually reviewing incoming leads and determining which jobs need immediate attention.

This workflow automates that process by using AI to:

- Analyze customer requests
- Score lead quality
- Detect emergency jobs
- Generate sales notes
- Notify the business owner
- Send a customer confirmation email
- Log every lead into Google Sheets

The result is faster response times, better lead organization, and a more consistent customer experience.
Each submission is enriched with:

- 10 structured AI fields
- AI-generated sales notes
- AI-generated customer email
- Emergency classification
- Automatic CRM entry

## Architecture

```text
Customer Form
      │
      ▼
Company Settings
      │
      ▼
Lead ID
      │
      ▼
AI Analysis
      │
      ▼
AI Sales Notes
      │
      ▼
Emergency Detection
      │
 ┌────┴────┐
 ▼         ▼
Emergency  Owner
 Email      Email
      │
      ▼
Google Sheets
      │
      ▼
Customer Confirmation
```

## Tech Stack

![n8n](https://img.shields.io/badge/n8n-Automation-orange)

![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4.1--mini-green)

![Google Sheets](https://img.shields.io/badge/Google-Sheets-brightgreen)

![Gmail](https://img.shields.io/badge/Gmail-API-red)

## Demo

Example workflow:

Customer submits a roofing request

↓

AI analyzes urgency and lead quality

↓

Emergency leads are prioritized automatically

↓

Owner receives a detailed AI-generated report

↓

Customer receives a confirmation email

↓

Lead is stored in Google Sheets

## Workflow Overview
<img width="1356" height="409" alt="Screenshot 2026-08-03 211919" src="https://github.com/user-attachments/assets/f49a49c2-7591-4244-979c-f4d31e26f5fb" />
📥 Lead Submission

<img width="877" height="902" alt="Customer Form" src="https://github.com/user-attachments/assets/7f945194-4530-4ecf-b67c-d6e65614ece6" />

### 🧠 AI Analysis

The workflow classifies each lead, scores buying intent, detects insurance claims, estimates project value, and recommends the next action.

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



### 📧 Owner Notification

The business owner receives a professional email containing:

- AI lead summary
- Lead score
- Urgency
- Customer information
- AI-generated sales notes
- Recommended next action

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

## Setup

1. Import the workflow into n8n.
2. Configure your OpenAI API credentials.
3. Configure Gmail OAuth.
4. Connect Google Sheets.
5. Update the Company Settings node.
6. Publish the form.

## Roadmap

- SMS notifications
- Calendar scheduling
- CRM dashboard
- Weekly AI reports
- Multi-industry support

## Conclusion

This project demonstrates how AI and workflow automation can streamline lead management for service-based businesses.

Although built for roofing contractors, the architecture can be adapted to HVAC, plumbing, electrical, landscaping, and other home service industries by updating the Company Settings node and AI prompts.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
