# AI-Powered Lead Management and Sales Workflow

**Tools:** n8n · Airtable · Groq AI (LLaMA 3.3) · Gmail · Slack · JavaScript



## The Business Problem

Most small and medium-sized businesses lose potential customers not because they have a bad product but because their follow-up is too slow or too generic. When enquiries come in through a contact form, someone on the team has to manually read each one, decide which leads are worth pursuing, write individual emails, and remember to alert the sales team about the good ones.

That process is slow, inconsistent, and very easy to get wrong at any kind of scale. This project solves all of that automatically.



## What This Workflow Does

The moment someone submits the contact form, the system automatically:

1. Captures the lead's details and saves them to Airtable.
2. Scores the lead out of 100 using a custom JavaScript algorithm.
3. Classifies the lead as Hot, Warm, or Cold.
4. Uses Groq AI to generate a personalized follow-up email and sends it through Gmail.
5. Sends an instant Slack notification for Hot leads.

## The Lead Scoring Logic

I designed the scoring system based on how sales teams actually prioritize leads.

| Scoring Factor | Answer | Points |
|---|---|---:|
| Budget | Under $5,000 | 10 |
| Budget | $5,000–$20,000 | 25 |
| Budget | $20,000–$50,000 | 40 |
| Budget | $50,000+ | 50 |
| Company Size | 1–10 employees | 5 |
| Company Size | 11–50 employees | 15 |
| Company Size | 51–200 employees | 22 |
| Company Size | 201–500 employees | 27 |
| Company Size | 500+ employees | 30 |
| Job Title | VP, Chief or C-Suite | 20 |
| Job Title | Director or Head | 14 |
| Job Title | Manager | 8 |
| Job Title | Other | 3 |



## Tools Used

- **n8n** – Workflow automation
- **Airtable** – CRM database
- **Groq AI (LLaMA 3.3)** – AI-generated follow-up emails
- **Gmail** – Automatic email delivery
- **Slack** – Instant notifications for Hot leads
- **JavaScript** – Lead scoring and email parsing logic



## Business Value

- Reduces manual work
- Responds to every lead automatically
- Prioritizes high-value leads
- Improves sales response time
- Stores all leads in Airtable
- Uses AI to personalize emails



## Project Structure

```text
ai-lead-management-n8n/
├── screenshots/
├── ai-lead-management-workflow.json
└── README.md
```



## Author

**Godslove Nnoli**

AI Automation Engineer | No-Code Developer | Workflow Automation Specialist
