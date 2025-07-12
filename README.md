# 🧠 AI Powered ATS Resume Optimizer

This is a Streamlit-based AI-powered application that analyzes your resume against a job description and helps you improve to pass Applicant Tracking Systems (ATS). It uses Google’s Gemini LLM - 2.0 Flash to generate actionable feedback and rewrite your resume to maximize job match score.

## 🚀 Features

✅ Upload or paste your resume  
✅ Paste any job description  
✅ AI-driven resume evaluation with:
- Match percentage score
- Missing/weak keywords
- Profile summary generation
- Clear improvement suggestions 

✅ Full resume rewrite optimized for the job  
✅ Highlights what was changed between your original and optimized resume  
✅ ATS-friendly formatting  
✅ Clean, responsive web interface using Streamlit  


## 📦 Tech Stack

- Python
- Streamlit
- Google Generative AI (Gemini)
- PyPDF2
- dotenv

---

## 📁 Project Structure

```
📁 ats-resume-optimizer
├── app.py # Main Streamlit app
├── requirements.txt # Python dependencies
├── .env # API Key (keep secret)
├── README.md # Project documentation
├── .gitignore # Ignore venv and sensitive files
└── .streamlit/
└── config.toml # Optional UI settings
```

## How It Works

User uploads a PDF resume/n
User pastes a job description/n
The app sends both to Gemini 2.0 via a well-crafted prompt/n
Gemini returns a JSON string with:
- JD Match
- MissingKeywords
- Profile Summary
- ImprovementSuggestions
Streamlit parses and displays the results in a clean UI

---

## ⚙️ Installation & Setup

### Clone the repo**

git clone https://github.com/yourusername/ats-resume-optimizer.git
cd ats-resume-optimizer

---

### Create virtual environment **

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

### Install dependencies
pip install -r requirements.txt

### Add your Google Gemini API key
GOOGLE_API_KEY=your_gemini_api_key_here

### Run Locally
streamlit run app.py


## 🙋 Author

Jigme Dorji
