# 🎥 YouTube Comment Sentiment Analyzer

This is a Flask-based web app that:
- ✅ Fetches YouTube comments using YouTube Data API
- 🧠 Analyzes sentiment using CardiffNLP and provides summaries via Google Gemini
- 📊 Displays interactive pie charts and tables
- 📄 Lets users download a PDF report

## 🚀 Features
- YouTube comment fetching (up to 300)
- Sentiment classification: Positive, Negative, Neutral
- Gemini-powered AI summarization (fallback: Facebook BART)
- Clean UI with Bootstrap & Chart.js
- PDF Report generation

## 🔧 Tech Stack
- Flask (Backend)
- HuggingFace Transformers (Model)
- Google Gemini API
- Chart.js, Bootstrap (Frontend)
- ReportLab (PDF generation)

## 🛠️ Setup Instructions

### Clone the repository
```bash
git clone https://github.com/your-username/youtube-sentiment-analysis.git
cd youtube-sentiment-analysis
