# Phase 1: Lead Scraping & Deduplication
**n8n Automated data extraction from LinkedIn & StartupJobs.cz with vector-based filtering.**

---

### 📺 System Execution (6-Second Loop)
![System Demo](assets/demo.gif)
*The n8n orchestrator processing multi-stream data into Supabase.*

---

### 📊 Objective Results
* **71% Noise Filtering:** Two-stage Regex targets only relevant listings and data for the database.
* **Direct XML/HTML Extraction:** 11-node custom parser extracts data directly from raw source code (0 cost and maintenance).
* **Semantic Deduplication:** 95% Cosine Similarity threshold (via pgvector) prevents duplicate leads across different sources.
* **Modular Structure:** Designed to accept new sources (e.g., Google Sheets) by mapping to a unified schema.

---

### 🎥 Video Walkthrough (100 Seconds)
Click the image below to watch the technical breakdown of the logic and database:

[![Video Walkthrough Preview](https://img.youtube.com/vi/P3Jgx5Q_dyU/0.jpg)](https://www.youtube.com/watch?v=P3Jgx5Q_dyU)

---

### 🖼️ Workflow Architecture
Below are the primary logic gates for the ingestion and deduplication stages:

**The n8n Ingestion Flow:**
![n8n Workflow Preview](assets/screenshot_workflow.png)

**Vector Deduplication Logic:**
![Deduplication Preview](assets/screenshot_supabase.png)

---

### 📂 Technical Documentation
* [**Raw JSON Workflows**](01-lead-ingestion/workflows/) — *Direct access to the logic files.*
* [**Detailed Technical README**](README.md) — *Full documentation on setup and variables.*

---
[← Return to Portfolio](https://linktr.ee/dpha05)
