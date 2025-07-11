🎥 YouTube Comment Sentiment Analyzer
This is a Flask-based web app that:

✅ Fetches YouTube comments using the YouTube Data API

🧠 Analyzes sentiment using CardiffNLP and summarizes using Google Gemini (fallback: Facebook BART)

📊 Displays sentiment statistics using interactive Pie Charts

📄 Generates a downloadable PDF Report with labeled comments

🚀 Features
🔗 Paste a YouTube video link and analyze up to 300 comments

🤖 Sentiment classification: Positive, Negative, Neutral using RoBERTa

🧠 Dual-layer summarization using Gemini and BART

📈 Clean visualization using Bootstrap + Chart.js

📄 PDF Report download with all labeled comments

🖼️ App Walkthrough
1️⃣ Homepage — Welcome Screen
<img width="1912" height="979" alt="Screenshot 2025-07-11 153517" src="https://github.com/user-attachments/assets/1fa2f8eb-0108-4308-811c-78e438116c45" />
The landing page shows a simple clean interface with a prompt to paste the video URL.

2️⃣ Enter YouTube Link
<img width="1912" height="975" alt="Screenshot 2025-07-11 153530" src="https://github.com/user-attachments/assets/e25cdd65-1649-4bf4-8ce6-a492f6e044ae" />
Paste a valid YouTube video link and hit Analyze to begin sentiment processing.

3️⃣ Sentiment Results
<img width="1901" height="1084" alt="Screenshot 2025-07-11 153443" src="https://github.com/user-attachments/assets/079f3ab8-815d-4c95-85ed-d85263a92083" /> <img width="1671" height="818" alt="Screenshot 2025-07-11 153459" src="https://github.com/user-attachments/assets/d770f8d2-a5b5-4ef8-a920-e625bbcc69d5" />
Includes:

📊 Sentiment Pie Chart

🥇 Top 5 Positive Comments

💔 Top 5 Negative Comments

🤖 AI Summary (based on sentiment distribution)

🧠 Gemini/BART-generated Summary

4️⃣ PDF Report Download
You can download all labeled comments as a clean, shareable PDF Report.

🧪 Tech Stack
Layer	Tools Used
Backend	Flask, Python
ML/NLP	HuggingFace Transformers, CardiffNLP, BART
Summarizer	Google Gemini (google.generativeai)
Visualization	Chart.js, Bootstrap, Jinja2
PDF Generation	ReportLab
API	YouTube Data API v3

🛠️ Setup Instructions
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/your-username/youtube-sentiment-analysis.git
cd youtube-sentiment-analysis
2. Create a Virtual Environment
bash
Copy
Edit
python -m venv venv
source venv/bin/activate       # On Windows: venv\Scripts\activate
3. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
4. Set Your API Keys in a .env File
Create a file named .env in the root directory with:

ini
Copy
Edit
YOUTUBE_API_KEY=your_youtube_api_key
GOOGLE_API_KEY=your_gemini_api_key
5. Run the App
bash
Copy
Edit
python app.py
Then open your browser and visit: http://127.0.0.1:5000

📂 Project Structure
arduino
Copy
Edit
.
├── app.py
├── templates/
│   ├── home.html
│   ├── index.html
│   └── results.html
├── requirements.txt
├── .gitignore
└── README.md
🙋‍♂️ Contributors
👨‍💻 Developed by: M. Bala Sainadh Reddy

📜 License
This project is licensed under the MIT License.

