🚀 QA Ingest Automation using n8n

An automated workflow built using n8n that processes form submissions, verifies trusted emails, generates AI-powered tags, and stores structured data into a database.

📌 Project Overview

This workflow automates the ingestion of Q&A form submissions by:

Capturing form responses

Checking if the email belongs to a trusted domain

Generating relevant tags using OpenAI

Storing structured data into a database

It helps in organizing user queries efficiently with AI-based classification.

🛠️ Tech Stack

⚡ n8n – Workflow Automation

🤖 OpenAI Chat Model – AI Tag Generation

🗄️ Database – Insert structured records

📩 Form Trigger – User submission handling

🔄 Workflow Architecture
Flow:
Form Submission
      ↓
Email Validation (is n8n.io email?)
      ↓
Trusted / Not Trusted Routing
      ↓
AI Tag Generation (OpenAI)
      ↓
Insert Row into Database
🧠 Workflow Explanation
1️⃣ On Form Submission

Triggers whenever a user submits a form.

2️⃣ Email Check (is n8n.io email?)

Checks whether the email belongs to a trusted domain.

3️⃣ Trust Routing

isTrusted.True

isTrusted.False

Routes the workflow accordingly.

4️⃣ Add Tags (OpenAI Chat Model)

Uses AI to:

Analyze question

Generate relevant tags

Categorize content automatically

5️⃣ Insert Row

Stores:

Name

Email

Question

AI-generated Answer

Tags

Trust Status

Timestamps

📊 Example Output Stored
Name	Email	Question	Tags	isTrusted
Sandhya Potadar	sushmapotadar123@gmail.com
	how to apply n8n Ambassador jobs?	n8n, ambassador program, application process	false
🎯 Features

✅ Automated email trust validation
✅ AI-based tagging system
✅ Structured database storage
✅ Scalable workflow design
✅ Low-code automation

🚀 How to Use

Import the workflow JSON into n8n

Configure:

OpenAI API key

Database credentials

Publish the workflow

Submit a test form

Monitor execution logs

📷 Workflow Screenshot

(Add your screenshot here)

📌 Future Improvements

Add spam detection

Add sentiment analysis

Dashboard for analytics

Admin approval system

Auto email response
