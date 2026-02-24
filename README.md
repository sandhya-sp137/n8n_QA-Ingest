<h1 align="center">🚀 QA Ingest Automation using n8n</h1>

<p align="center">
An automated workflow built using <b>n8n</b> that processes form submissions, 
verifies trusted emails, generates AI-powered tags, 
and stores structured data into a database.
</p>

---

## 📌 Project Overview

This workflow automates the ingestion of Q&A form submissions by:

- Capturing form responses  
- Checking if the email belongs to a trusted domain  
- Generating relevant tags using OpenAI  
- Storing structured data into a database  

It helps in organizing user queries efficiently with AI-based classification.

---

## 🛠️ Tech Stack

- ⚡ **n8n** – Workflow Automation  
- 🤖 **OpenAI Chat Model** – AI Tag Generation  
- 🗄️ **Database** – Insert structured records  
- 📩 **Form Trigger** – User submission handling  

---

## 🔄 Workflow Architecture


Form Submission
↓
Email Validation (is n8n.io email?)
↓
Trusted / Not Trusted Routing
↓
AI Tag Generation (OpenAI)
↓
Insert Row into Database


---

## 🧠 Workflow Explanation

### 1️⃣ On Form Submission  
Triggers whenever a user submits a form.

### 2️⃣ Email Check (is n8n.io email?)  
Checks whether the email belongs to a trusted domain.

### 3️⃣ Trust Routing  
- isTrusted.True  
- isTrusted.False  

Routes the workflow accordingly.

### 4️⃣ Add Tags (OpenAI Chat Model)

Uses AI to:

- Analyze question  
- Generate relevant tags  
- Categorize content automatically  

### 5️⃣ Insert Row  

Stores:

- Name  
- Email  
- Question  
- AI-generated Answer  
- Tags  
- Trust Status  
- Timestamps  

---

## 📊 Example Output Stored

| Name | Email | Question | Tags | isTrusted |
|------|-------|----------|------|-----------|
| Sandhya Potadar | sushmapotadar123@gmail.com | how to apply n8n Ambassador jobs? | n8n, ambassador program, application process | false |

---

## 🎯 Features

- ✅ Automated email trust validation  
- ✅ AI-based tagging system  
- ✅ Structured database storage  
- ✅ Scalable workflow design  
- ✅ Low-code automation  

---

## 🚀 How to Use

1. Import the workflow JSON into n8n  
2. Configure:
   - OpenAI API key  
   - Database credentials  
3. Publish the workflow  
4. Submit a test form  
5. Monitor execution logs  

---

## 📷 Workflow Screenshot

<img width="1663" height="784" alt="Screenshot (102)" src="https://github.com/sandhya-sp137/n8n_QA-Ingest/blob/5fe927203d8b5b1552ca8abbd79bac02ab550ccd/Screenshot%202026-02-24%20203509.png" />

---

## 📌 Future Improvements

- Add spam detection  
- Add sentiment analysis  
- Dashboard for analytics  
- Admin approval system  
- Auto email response  
