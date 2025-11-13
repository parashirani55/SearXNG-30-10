
🧠 SearXNG-30-10 — AI Research & Valuation Assistant

SearXNG is an AI-powered research and company analysis tool built with Python, Streamlit, and Supabase.
It uses APIs like SerpAPI, OpenAI, and Playwright to fetch, analyze, and display business intelligence data.

🚀 Features

🌐 Intelligent company data collection via SerpAPI

🧾 Automatic report generation (PDF supported)

🧠 AI-driven company insights and summarization

💾 Data storage and management via Supabase

🧱 Interactive web interface using Streamlit

⚙️ Installation & Setup Guide

Follow these steps to set up and run the project locally.

1️⃣ Clone the Repository
git clone https://github.com/parashirani55/SearXNG-30-10.git
cd SearXNG-30-10

2️⃣ Create a Virtual Environment
python3 -m venv venv
source venv/bin/activate     # For Mac/Linux
venv\Scripts\activate        # For Windows

3️⃣ Install Dependencies
pip install -r requirements.txt


If you see missing package errors (optional installs), you can also install them manually:

pip install streamlit python-dotenv google-search-results playwright supabase

4️⃣ Install & Configure Playwright
playwright install


This installs browser drivers needed for automation.

5️⃣ Add Environment Variables

Create a .env file in your project root:

touch .env


Add your environment variables inside:

OPENAI_API_KEY=your_openai_api_key
SERPAPI_API_KEY=your_serpapi_api_key
SUPABASE_URL=https://your-project.supabase.co
SUPABASE_KEY=your_supabase_service_role_key


Make sure .env is listed in your .gitignore file so it’s not uploaded to GitHub.

6️⃣ Run the Application
streamlit run app.py


Once it starts, open the local URL:

http://localhost:8501

🧩 Troubleshooting

supabase_url is required
→ Ensure .env contains both SUPABASE_URL and SUPABASE_KEY.
→ Verify .env is in the project root.

zsh: command not found: streamlit
→ Install Streamlit:

pip install streamlit


ImportError: cannot import name 'GoogleSearch'
→ Make sure you have the correct package:

pip install google-search-results

📦 Requirements (main libraries)
Package	Version
streamlit	1.50.0
openai	2.2.0
google-search-results	2.4.2
playwright	1.42.0
supabase	2.21.1
python-dotenv	1.1.1
pandas	2.3.3
fpdf2	2.7.9
beautifulsoup4	4.14.2

Full list is available in requirements.txt.
