# AI-Resume-Matcher

# 🤖 AI-Powered Resume Screening App

This project is a **Streamlit-based web app** that uses **Groq's LLaMA-4 model** for intelligent resume screening. It matches uploaded resumes (PDF/DOCX) against a job description, scores them using LLM intelligence, and automates workflows via **n8n**.

---

## 🚀 Features

- 📋 **Job Description Matching**  
  Upload multiple resumes and match them to a job description using an LLM (LLaMA 4 via Groq API).

- 📊 **Automated Scoring System**  
  Each resume is rated between 0–100 based on relevance to the job description.

- 🔄 **n8n Webhook Integration**  
  Sends resume names and match scores to your n8n workflow for automation (e.g., alerts, storage, database sync).

- 🧠 **Modular AI Design**  
  Easily customizable prompts and models using the `langchain_groq` integration.

- 🖥️ **Simple UI with Streamlit**  
  User-friendly and responsive frontend for fast resume uploads and analysis.

---

## 📂 File Structure

```plaintext
app.py             # Main application file
.env               # Environment variables (API keys, webhook URLs)
requirements.txt   # Python dependencies
README.md          # You're here!
```




## 🛠️ Setup Instructions
1. Clone the Repository
```   

git clone https://github.com/your-username/resume-matcher.git
cd resume-matcher
```
3. Install Dependencies
Create a virtual environment and install the required packages:

```

pip install -r requirements.txt
```
3. Environment Configuration
Create a .env file in the root directory and add your credentials:
```

GROQ_API_KEY=your_groq_api_key
N8N_WEBHOOK_URL=https://your-n8n-instance/webhook/your-path
```
## ⚠️ Never expose your API keys in the codebase.

4. Run the App
```   

streamlit run app.py
The app will open in your browser at http://localhost:8501.
```
## 📸 UI Preview

## 🧠 How It Works
- Upload resumes (PDF/DOCX).

- Paste the job description in the input field.

- Click "Match Resumes".

- The LLM compares each resume against the job description and assigns a score.

- Results are displayed and also sent to your n8n automation pipeline.

## ✅ To-Do / Improvements
-  Add CSV export of match results.

-  Show extracted resume highlights and keywords.

 - Add advanced prompt tuning interface.

- Integrate authentication for admin access.

## 🤝 Contributing
Pull requests are welcome! Feel free to suggest features, report bugs, or fork for your own use case.

## 📄 License
MIT License. See LICENSE file for details.

## 📬 Contact
Project Maintainer: **Biswajeet Dixit**

LinkedIn: https://www.linkedin.com/in/biswajeet-dixit-047015261/

