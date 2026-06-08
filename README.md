# TikTok Auto-Posting Automation

This project automates scheduling and publishing content to TikTok from Airtable using Make.com and Zernio.
<img width="947" height="535" alt="Screenshot (1435)" src="https://github.com/user-attachments/assets/57162f86-1cbf-4c93-a708-bb2c456c86d0" />

## 🚀 Features
* **Dynamic Scheduling:** Triggered by Airtable 'Scheduled Posting Time'.
* **Multi-Format Support:** Handles single videos and multi-image carousels.
* **Auto-Status Sync:** Updates Airtable checkbox once published.
* **Zernio Integration:** Bypasses long TikTok API approval processes.

## 🛠️ Tech Stack
* **Airtable:** CMS & Scheduler.
* **Make.com:** Workflow Automation.
* **Zernio:** Third-party API for TikTok.

## 📋 Automation Workflow
1. **Airtable Search:** Polls base every 15 mins for pending records.
2. **Router:** Directs data by content type (Video vs. Carousel).
3. **JSON Handling:** Custom payloads sent via HTTP to Zernio API.
4. **Airtable Update:** Marks record as `Posted to TikTok`.

##  Key Learnings
Carousel logic required advanced **Array Aggregation** and specific JSON formatting to handle multi-image structures correctly.
