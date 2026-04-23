AI Automation Intern: Prospecting & Engagement Bot .This repository contains an automated lead generation and engagement pipeline built using n8n. It targets niche-specific leads on Instagram and X or Twitter for an AI Agency.

🛠 Tech Stack Automation Engine: n8n (Self-hosted or Desktop)

Scraping: Apify (Instagram/Twitter Scrapers)

AI Engine: Groq API (Llama 3 / Mixtral) for hyper-personalized DMs

Database/Reporting: Google Sheets API

Communication: Email (SMTP) for daily reports

 Features Multi-Platform Scraping: Filters leads by bio keywords, location, and follower/engagement ratios.

AI Personalization: No generic templates. Groq analyzes lead data to draft custom AI agency service pitches.

Smart Delays- Randomized wait times to stay within rate limits and avoid platform bans.

Event Detection: Triggers based on new follows or bio updates...

Reporting: Automatic sync to Google Sheets with real-time conversion tracking.

📂 Repository Structure workflow.json: The exported n8n workflow (Import this into your n8n).

samples/: Screenshots of the Google Sheet and AI-generated DM logs.

demo.mp4: Screen recording showing the full automation in action.

⚙️ Setup Instructions Import workflow.json into your n8n instance.

Credentials: Add your Apify, Groq, and Google Sheets credentials in the respective node settings.

Configuration: Set your target keywords (e.g., "Real Estate", "E-commerce") in the Trigger node.

Run: Activate the workflow and monitor the "Daily Report" Google Sheet for incoming leads.

💡 Reasoning for Tool Choices n8n: Chosen for its flexibility in handling complex JSON logic and multi-step follow-ups without the high cost of Zapier.

Groq API: Used for near-instant inference speed and generous free tier, ensuring high-quality personalized DMs without latency.

Apify: Reliable cloud-based scraping that bypasses basic IP blocks which often stop local scrapers.

📈 Future Improvements (Budget/Time) Lead Scoring: Implement a deeper "Bio Relevance" score using LLM analysis to filter high-ticket prospects only.

Proxy Rotation: Use residential proxies to scale from 100 to 1000+ DMs/day safely.

Sentiment Analysis: Automatically detect "Interested" vs "Not Interested" replies to intelligently pause or continue follow-up sequences...
