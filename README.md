# Roofing Automation — automation/v1

This branch contains a v1 implementation for an automation system to capture leads, qualify, book appointments, and run follow-ups for a roofing company.

What's included:
- Folder structure and example code for webhooks and service integrations
- Make.com JSON examples for core workflows
- Airtable CRM schema (JSON)
- AI prompts for the website chatbot and follow-up flows
- Step-by-step setup guide for v1

Core flows implemented (paper + code):
- Website chatbot: answers FAQs, qualifies lead, pushes to CRM, books Google Calendar appointment, triggers follow-up if needed.
- Automated follow-ups across channels: website form → SMS+email flow, FB/IG DM lead → auto reply + multi-step follow-up, missed phone call/no answer → text back + booking link.
- CRM: Airtable schema with lead statuses and message logs.
- Weekly reporting: sample query structure and fields for reporting.

Tech stack: Make.com, Google Calendar, Airtable, Twilio (or CallRail), Facebook & Instagram Messaging API, website chat widget (webhook with OpenAI API).

Files in this branch:
- FOLDER_STRUCTURE.txt — repo layout
- src/ — webhook server + service modules
- crm/airtable_schema.json — CRM schema
- make/ — sample Make.com module JSON exports
- prompts/ — AI prompts for chatbot and follow-ups
- docs/SETUP_GUIDE.md — step-by-step setup instructions

Core flows implemented and how to use them live in the docs/SETUP_GUIDE.md