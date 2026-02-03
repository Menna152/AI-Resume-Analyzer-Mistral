
#  AI Resume Analyzer - HR Expert System

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Mistral_Nemo-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/LangChain-121011?style=for-the-badge&logo=chainlink&logoColor=white" />
  <img src="https://img.shields.io/badge/Gradio-FF9D00?style=for-the-badge&logo=gradio&logoColor=white" />
</p>

##  Overview
**AI Resume Analyzer** is an intelligent recruitment tool designed to bridge the gap between job seekers and their dream jobs. By leveraging the power of **Mistral-Nemo-12B**, the system analyzes PDF resumes against specific job descriptions to identify missing skills and provide actionable career advice.

---

##  Key Features
- **Smart PDF Parsing:** Seamlessly extracts text from uploaded CVs.
- **Skill Gap Analysis:** Compares candidate skills with job requirements in real-time.
- **Professional Recommendations:** Generates personalized advice for skill development.
- **Interactive Dashboard:** A user-friendly interface for instant analysis and structured results.
- **Structured Data:** Outputs findings in a clean, tabular format (DataFrame).

---

##  Tech Stack
- **Language:** Python 
- **LLM:** Mistral-Nemo-Instruct-2407 (via HuggingFace Transformers)
- **Orchestration:** LangChain (Structured Output Parsers & Prompt Engineering)
- **Frontend:** Gradio
- **Deployment:** Ngrok for public URL tunneling
- **Environment:** Developed on Kaggle with GPU acceleration (T4 x2)

---

##  How It Works


1. **Upload:** User uploads a CV in PDF format.
2. **Input:** User pastes the target Job Description (JD).
3. **Processing:** The LLM extracts skills and performs a cross-match analysis.
4. **Result:** The system displays a table containing:
    - **Skill Name:** Extracted from the JD.
    - **Exists:** (Yes/No) presence in the CV.
    - **Improvement:** Steps to acquire or polish the skill.

---

##  Demo

https://github.com/Menna152/AI-Resume-Analyzer-Mistral/releases/tag/v1.0

##  Installation & Usage

1. **Install Dependencies:**
   ```bash
   pip install langchain langchain-community pypdf transformers torch gradio pyngrok
