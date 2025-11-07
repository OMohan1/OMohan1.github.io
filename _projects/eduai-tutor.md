---
title: EduAI 
tags: studybuddy, quality education
---
# 📘 EduAI – AI Study Buddy

An **AI-powered flashcard generator** that transforms raw study notes into interactive quiz cards, helping students revise smarter and faster.  
Built with **Flask + MySQL + Hugging Face AI + HTML/CSS/JS**.

---

## 🚀 Features

- 📝 Paste study notes → get quiz questions instantly  
- 🤖 AI-powered (Hugging Face Question-Answering API)  
- 🎴 Interactive flip cards (HTML/CSS/JS)  
- 💾 Save & reuse flashcards (MySQL backend)  
- 🌍 Beginner-friendly but highly impactful  

---

## 🛠 Tech Stack

**Frontend:** HTML5, CSS3, JavaScript  
**Backend:** Python (Flask)  
**Database:** MySQL  
**AI Integration:** Hugging Face Transformers API  

---

## ⚙️ How It Works

1. User pastes study notes into the app.  
2. Flask backend sends notes to the Hugging Face API to generate quiz questions.  
3. JavaScript frontend displays interactive flip cards with questions and answers.  
4. Flashcards are stored in MySQL for reuse and tracking.  

---

## 📂 Project Structure

EduAI-StudyBuddy/
│── backend/
│ ├── app.py # Flask app
│ ├── models.py # Database models
│ ├── routes.py # API endpoints
│ ├── requirements.txt # Python dependencies
│
│── frontend/
│ ├── index.html # Main UI
│ ├── style.css # Styling
│ ├── script.js # Flashcard logic
│
│── database/
│ ├── schema.sql # MySQL schema
│
│── docs/
│ ├── README.md # Documentation
│
│── .gitignore
│── config.example.json
│── LICENSE

yaml
Copy code

---

## 📸 Demo

**Workflow Overview:**
- Paste notes → AI generates flashcards  
- Click cards to flip & view answers  
- Save decks for future revision  

*(Screenshots or demo GIFs can be added here)*

---

## 📈 Key Insights

- Automates flashcard creation from raw text using NLP  
- Demonstrates full-stack integration (Frontend + Backend + Database + AI)  
- Showcases practical application of Flask, APIs, and MySQL  
- Can be extended to mobile or e-learning platforms  

---

## 🔮 Future Improvements

- Add user accounts & personalized decks  
- Multiple-choice and difficulty-based flashcard generation  
- Deploy to mobile (Flutter or React Native)  
- Integrate cloud storage for user data  

---

## 🧑‍💻 Installation & Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/EduAI-StudyBuddy.git
   cd EduAI-StudyBuddy
Set up the backend

bash
Copy code
cd backend
pip install -r requirements.txt
python app.py
Initialize the database

bash
Copy code
mysql -u root -p < database/schema.sql
Launch the frontend

Open frontend/index.html in your browser.

📜 License
MIT License – free to use and modify for educational or research purposes.

✨ Author
Mohan Otieno
💻 Penetration Tester | Software Developer | AI Enthusiast
📧 otienomohan678@gmail.com

🙌 Acknowledgments
Hugging Face for NLP APIs

Flask and MySQL communities
