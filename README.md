# Recruit.AI 🤖
### *Automating the Bridge Between Talent and Opportunity*

**Recruit.AI** is an intelligent recruitment orchestration platform designed to eliminate the "resume black hole." It uses Semantic Search and LLM-powered analysis to match candidates to job descriptions based on actual skills and potential, rather than just keywords.

---

## 🛠️ Technical Architecture
I built this project to demonstrate how AI can handle high-volume data processing while maintaining high accuracy for HR professionals.

* **Frontend:** A clean, data-driven dashboard built with **React** and **Tailwind CSS**, designed for recruiters to scan candidate profiles quickly.
* **Orchestration:** **n8n** workflows manage the pipeline—from receiving a resume to scoring it against a specific Job Description (JD).
* **Intelligence Layer:** Utilizes **Llama 3** (via Groq) for high-speed parsing and **Embeddings** to calculate semantic similarity scores.
* **Automation:** Integrated with **Google Sheets/Airtable** to simulate a real-world Applicant Tracking System (ATS).

---

## 🌟 Key Features & Engineering Decisions

### 🧠 Semantic Matching (Beyond Keywords)
Traditional ATS tools fail because they only look for exact word matches. 
* **The Solution:** I implemented an LLM-based scoring system that understands context. If a resume says "Expert in building interfaces" and the JD asks for "Frontend Developer," Recruit.AI recognizes they are the same thing.

### 📉 Bias Reduction Filter
The system is designed to focus on skills and experience metrics.
* **The Decision:** By structuring the data into a skill-first format before the final evaluation, the tool helps recruiters focus on competency-based hiring.

### ⚡ Lightning-Fast Screening
By utilizing **Groq's LPU inference**, the system can analyze and score a 3-page resume in under 2 seconds.
* **The "Why":** In high-volume recruiting, speed is a feature. This allows for real-time feedback to applicants.

---

## 📂 Project Structure
* **/frontend**: The React-based Recruiter Dashboard.
* **/backend**: The n8n JSON workflows for resume parsing and scoring.
* **/assets**: System architecture diagrams and UI screenshots.

---

## 👨‍💻 "Magic Lines" for the Interview
* "Recruit.AI isn't just a filter; it's a **semantic engine** that understands the relationship between a candidate's experience and the company's needs."
* "I chose a **low-code backend** to allow for rapid iteration of the scoring prompts, which is critical when fine-tuning AI for HR sensitivity."

---

## 🚀 Future Roadmap
* **Auto-Emailer:** Integrating SendGrid to automatically schedule interviews for high-scoring candidates.
* **LinkedIn Scraper:** A browser extension to pull candidate data directly into the Recruit.AI engine.
