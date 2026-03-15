---
# 🤖 ResumeForge AI  
## License
This project is licensed under the MIT License.
### Intelligent ATS Optimization Engine  
<p align="center">  <img src="https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python" /> <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" /> <img src="https://img.shields.io/badge/Streamlit-App-ff4b4b?style=for-the-badge&logo=streamlit" /> <img src="https://img.shields.io/badge/LangGraph-Agentic-purple?style=for-the-badge" /> <img src="https://img.shields.io/badge/LLM-Groq%20%7C%20Gemini-orange?style=for-the-badge" /> </p> <p align="center"> <b>Agentic Resume Intelligence powered by Hybrid ATS Scoring & Semantic Alignment</b> </p>

ResumeForge AI is an intelligent, full-stack agentic workflow designed to optimize resumes for Applicant Tracking Systems (ATS) compatibility using hybrid scoring and semantic reasoning.

It doesn’t just rewrite resumes — it structures them, scores them, identifies skill gaps, and iteratively improves alignment using semantic intelligence powered by LLMs.

---

## 🚀 Key Features

### 🧠 Intelligent Resume Structuring
Transforms unstructured resumes (PDF/TXT) into structured, validated JSON:
- Professional Summary  
- Experience  
- Skills  
- Projects  
- Certifications  

Strict no-hallucination enforcement ensures accuracy and reliability.

---

### 🎯 Hybrid ATS Scoring Engine

Multi-dimensional scoring framework:

- 🔑 **Keyword Match Score** – High-impact skill overlap  
- 📈 **Quantification Score** – Measurable achievements detection  
- 🧠 **Semantic Relevance Score** – Context-aware LLM alignment  
- ⚠️ **Missing Skills Analysis** – Gap detection vs Job Description  

```text
Overall ATS Score =
(Keyword × 0.4) +
(Quantification × 0.2) +
(Semantic × 0.4)
```

This ensures resumes are optimized both syntactically and semantically.

---

### 🔄 Agentic Optimization Workflow (LangGraph)

ResumeForge AI models resume enhancement as a deterministic state machine:

1️⃣ Generate Structured Resume  
2️⃣ Compute ATS Score  
3️⃣ Detect Missing High-Impact Skills  
4️⃣ Generate Strategic Gap Questions  
5️⃣ Apply Improvements  
6️⃣ Re-score & Compare  

This creates a continuous feedback-driven optimization loop.

---

### 🌍 Multi-LLM Support

- Groq (Llama 3 / GPT-OSS)  
- Google Gemini  
- Dynamic provider selection  
- RPM-based rate limiting  

Designed for flexibility and production safety.

---

### 🖥️ Cross-Platform PDF Engine

Built for both local and cloud environments:

- Windows → MS Word (docx2pdf)  
- Cloud / Linux → Pure Python (ReportLab fallback)  
- Automatic fail-safe handling  

No environment lock-in.

---

## 🏗️ Architecture

The system is built on **LangGraph**, treating resume optimization as a structured state machine.

### Core Nodes

- Generate Resume Node  
- ATS Score Node  
- Gap Analysis Node  
- Resume Update Node  

Each transition is validated and production-safe.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | Streamlit |
| Orchestration | LangChain + LangGraph |
| LLM Providers | Groq, Gemini |
| Resume Parsing | PyMuPDF |
| PDF Engine | docx2pdf, ReportLab |
| Validation | Regex + JSON sanitation |

---

## ⚡ Quick Start

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/ResumeForge-AI.git
cd ResumeForge-AI
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Configure API Keys

```env
GROQ_API_KEY=your_groq_api_key
GEMINI_API_KEY=your_gemini_api_key
```

### 4️⃣ Run Application

```bash
streamlit run app.py
```

---

## 🖥️ Usage Guide

### Generate Mode
Upload your resume and paste a job description.  
The system structures your resume and generates a complete ATS compatibility report.

### Improve Mode
Answer AI-generated strategic gap questions.  
The system refines your resume and displays before/after score improvements.

### Analyze Mode
Review missing skills, alignment insights, and semantic breakdown.

---

## 🎯 Supported Domains

ResumeForge AI dynamically adapts skill categorization and supports:

- Data Science  
- Software Engineering  
- Accounting & Finance  
- Banking  
- Marketing  
- HR & Operations  
- MBA / Freshers  

---

<img width="951" height="443" alt="image" src="https://github.com/user-attachments/assets/3c56be69-0e4e-4fd1-918c-82b7794d28d6" />

---
<img width="953" height="428" alt="image" src="https://github.com/user-attachments/assets/b63e932f-fb3f-47f2-a65d-b403f3291651" />

---
<img width="807" height="421" alt="image" src="https://github.com/user-attachments/assets/362961f7-09ed-4b2a-9f4e-21308e324818" />


---
## 🌐 Live Demo

🚀 Try ResumeForge AI Online:  
👉 https://resume-deep-ai-agent.onrender.com/
