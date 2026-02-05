# Automotive German Teacher - Technical Vocabulary Pipeline 🇩🇪🚗

This repository contains an automated system designed to master German automotive engineering terminology. It leverages AI to transform technical video content into structured learning assets.

## 🏗️ System Architecture
The pipeline is fully automated via **n8n** and follows these steps:
1. **Source Monitoring:** Monitors specific automotive engineering channels via **YouTube API v3**.
2. **Transcription:** Uses **Supadata** to extract high-fidelity transcripts from new technical videos.
3. **AI Processing:** A GPT-4 agent analyzes the transcript to isolate technical terms (e.g., *Zahnriemen*, *Steuerkette*, *Drehmoment*) and translates them into Italian/English.
4. **Persistence & Sync:**
   - **Google Sheets:** Acts as a portable glossary for mobile review.
   - **SQL (MariaDB):** Stores the terms for long-term data analysis and duplicate prevention.

## 🛠️ Key Technical Features
* **Automated Deduplication:** Uses SQL queries to ensure the glossary remains clean and unique.
* **Context-Aware Translation:** The AI doesn't just translate words; it provides the automotive context for each term.
* **Scalable Data Mining:** Designed to process hours of technical documentation and video content into a structured database.


---
*Developed to accelerate professional integration into the German automotive engineering sector.*
