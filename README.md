TikTok Auto-Posting Automation
This project automates the process of scheduling and publishing content to TikTok directly from an Airtable base using Make.com and Zernio.
![Demo](demo.gif)
🚀 Features
Dynamic Scheduling: Posts are triggered based on a specific 'Scheduled Posting Time' column in Airtable.
Multi-Format Support: Handles both single video uploads and multi-image carousels.
Auto-Status Sync: Automatically updates a checkbox in Airtable once a post is successfully published.
Zernio Integration: Uses Zernio for streamlined API handling and bypassing long approval processes.
🛠️ Tech Stack
Airtable: Content Management System (CMS) & Scheduler.
Make.com: Workflow Automation Platform.
Zernio: Third-party API tool for TikTok publishing.
📋 Automation Workflow
Airtable Search: Polls the base every 15 minutes for records where Status = POSTED and the Scheduled Time is due.
Router: Directs the data based on content type (Video vs. Carousel).
JSON Handling: Custom JSON payloads are sent via HTTP modules to the Zernio API.
Airtable Update: After a successful response, the record is marked as Posted to TikTok.
 Key Learnings
Implementing the Carousel logic required advanced Array Aggregation and specific JSON formatting to ensure multi-image posts were correctly processed by the TikTok API structure.
