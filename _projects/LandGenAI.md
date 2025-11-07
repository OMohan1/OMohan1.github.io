# 🌍 LandGen AI

**LandGen AI** is an intelligent environmental dashboard that analyzes and visualizes key ecological indicators — weather patterns, soil health, deforestation data, and wildlife extinction risk — using **AI models** and **real-time open-data APIs**.

Built with **Streamlit**, **Supabase**, and optional **Sentinel satellite data**, LandGen AI helps users understand and predict environmental changes anywhere on Earth.

---

## ✨ Features

- 🔐 **Supabase Authentication** – Login, signup, and password reset  
- 🌦️ **Real-Time Weather Monitoring** – Powered by Open-Meteo API  
- 🌾 **AI-Powered Soil Health Detection** – SoilGrids + ML model  
- 🌲 **Deforestation Insights** – Sentinel / Global Forest Watch data  
- 🐾 **Wildlife Extinction Risk Analysis** – Custom-trained AI models  
- 💾 **Supabase Database** – Stores user data and subscriptions  
- 🚀 **Streamlit Web Interface** – Interactive and visual dashboards  
- 🧠 **Mock Mode** – Test locally without API keys  

---

## 🗂️ Project Structure

LandGen-AI/
│
├── dashboard.py # Main Streamlit app
├── fetch_data.py # Weather, soil, deforestation, wildlife data
├── ai_models.py # Machine learning prediction models
├── soil_detector.py # Soil health analyzer
├── auth.py # User authentication logic
├── subscription.py # Subscription and plan management
├── config.py # API and Supabase configuration
├── sentinel_api.py # Optional Sentinel imagery handler
├── requirements.txt # Python dependencies
└── .env # Environment variables (not committed)

yaml
Copy code

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/landgen-ai.git
cd landgen-ai
2️⃣ Create a Virtual Environment
bash
Copy code
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate
3️⃣ Install Dependencies
bash
Copy code
pip install -r requirements.txt
🔐 Environment Variables
Create a file named .env in the project root and add:

bash
Copy code
# Supabase credentials
SUPABASE_URL=https://your-project-id.supabase.co
SUPABASE_KEY=your-anon-or-service-key

# Sentinel Hub (optional — use "demo" for mock mode)
SENTINEL_CLIENT_ID=demo
SENTINEL_CLIENT_SECRET=demo

# Other API keys (optional)
OPENWEATHER_API_KEY=your_open_meteo_api_key
💡 Using “demo” for Sentinel credentials enables mock mode, allowing the app to run without real satellite access.

🌦️ Data Sources
Data Type	API Source	Notes
Weather	Open-Meteo API	Free, no API key required
Soil	SoilGrids API	Global soil composition data
Deforestation	Global Forest Watch	Country-level forest loss data
Wildlife	Custom AI Model	Predicts extinction probability
Sentinel Images	Sentinel Hub (optional)	Real satellite imagery

🚀 Running the App
Start the Streamlit dashboard:

bash
Copy code
streamlit run dashboard.py
Then open in your browser:
👉 http://localhost:8501

🧠 Mock / Demo Mode
If you don’t have Sentinel credentials, set the following in .env:

bash
Copy code
SENTINEL_CLIENT_ID=demo
SENTINEL_CLIENT_SECRET=demo
LandGen AI will automatically generate synthetic data for testing without external APIs.

🧩 Supabase Integration
Supabase handles:

🔐 User authentication

💾 Data storage for soil and wildlife predictions

💳 Subscription tracking

Example (config.py):

python
Copy code
from supabase import create_client
import os
from dotenv import load_dotenv

load_dotenv()
supabase = create_client(os.getenv("SUPABASE_URL"), os.getenv("SUPABASE_KEY"))
🧮 AI Models
🌦️ Weather Trend Predictor – Detects potential rainfall and temperature shifts

🐾 Wildlife Extinction Risk Model – Classifies endangered species probability

🌾 Soil Health Detector – Evaluates fertility and nutrient balance

Models are modular and can be retrained or extended with new datasets.

📦 Example requirements.txt
nginx
Copy code
streamlit
pandas
numpy
requests
supabase
python-dotenv
sentinelhub
Pillow
scikit-learn
🌐 Deployment
You can deploy easily on:

☁️ Streamlit Community Cloud

⚙️ Render or Railway (for backend hosting)

🤗 Hugging Face Spaces (for public AI demos)

🧑‍💻 Contributing
Pull requests are welcome!

Fork this repository

Create a feature branch

Commit and push your changes

Submit a PR

🪪 License
Released under the MIT License — free to use, modify, and distribute with attribution.

❤️ Acknowledgements
Supabase – Authentication & database

Open-Meteo – Weather data

SoilGrids – Soil composition data

Global Forest Watch – Deforestation insights

Sentinel Hub – Optional satellite imagery

Author: Mohan Otieno
📧 otienomohan678@gmail.com
💻 AI Developer | Environmental Data Engineer | Python Enthusiast
