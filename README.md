<h1>🚀 QA Ingest Automation using n8n</h1>

An automated workflow built using n8n that processes form submissions, verifies trusted emails, generates AI-powered tags, and stores structured data into a database.
________________________________________

<h2>📌 Project Overview</h2>

This workflow automates the ingestion of Q&A form submissions by:
1.	Capturing form responses
2.	Checking if the email belongs to a trusted domain
3.	Generating relevant tags using OpenAI
4.	Storing structured data into a database
It helps in organizing user queries efficiently with AI-based classification.
________________________________________

<h2>🛠️ Tech Stack</h2>

- ⚡ **n8n** – Workflow Automation  
- 🤖 **OpenAI Chat Model** – AI Tag Generation  
- 🗄️ **Database** – Insert structured records  
- 📩 **Form Trigger** – User submission handling
________________________________________

<h2>🔄 Workflow Architecture</h2>

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
________________________________________

<h2>🧠 Workflow Explanation</h2>

<h3>1️⃣ On Form Submission</h3>
Triggers whenever a user submits a form.

<h3>2️⃣ Email Check (is n8n.io email?)</h3>
Checks whether the email belongs to a trusted domain.

<h3>3️⃣ Trust Routing</h3>
•	isTrusted.True
•	isTrusted.False
Routes the workflow accordingly

<h3>4️⃣ Add Tags (OpenAI Chat Model)</h3>
Uses AI to:
•	Analyze question
•	Generate relevant tags
•	Categorize content automatically

<h3>5️⃣ Insert Row</h3>
Stores:
•	Name
•	Email
•	Question
•	AI-generated Answer
•	Tags
•	Trust Status
•	Timestamps
________________________________________

<h2>📊 Example Output Stored</h2>

Name	Email	Question	Tags	isTrusted
Sandhya Potadar	sushmapotadar123@gmail.com	how to apply n8n Ambassador jobs?	n8n, ambassador program, application process	false
________________________________________

<h2>🎯 Features</h2>

-✅ Automated email trust validation
-✅ AI-based tagging system
-✅ Structured database storage
-✅ Scalable workflow design
-✅ Low-code automation
________________________________________

<h2>🚀 How to Use</h2>

1.	Import the workflow JSON into n8n
2.	Configure:
o	OpenAI API key
o	Database credentials
3.	Publish the workflow
4.	Submit a test form
5.	Monitor execution logs
________________________________________

<h2>📷 Workflow Screenshot</h2>
<img width="1663" height="784" alt="Screenshot (102)" src="https://github.com/sandhya-sp137/n8n_QA-Ingest/blob/5fe927203d8b5b1552ca8abbd79bac02ab550ccd/Screenshot%202026-02-24%20203509.png" />
________________________________________

<h2>📌 Future Improvements</h2>
•	Add spam detection
•	Add sentiment analysis
•	Dashboard for analytics
•	Admin approval system
•	Auto email response

