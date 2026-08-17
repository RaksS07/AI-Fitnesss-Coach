# AI Gym & Fitness Assistant

### Major AI/ML Project

## 📌 Project Overview

**AI Gym & Fitness Assistant** is an integrated AI-powered fitness platform designed to provide personalized workout guidance, nutrition planning, fitness tracking, and intelligent gym recommendations. The system combines **computer vision, machine learning, NLP, behavioral analytics, and recommendation systems** across seven core modules.

| # | Module                              | Technology / Approach                    |
| - | ----------------------------------- | ---------------------------------------- |
| 1 | 🏋️ **AI Gym Trainer**              | MediaPipe, OpenCV, Pose Detection        |
| 2 | 🥗 **AI Dietician & Calorie Coach** | NLP, BMI, TDEE & Meal Planning           |
| 3 | 📡 **Smart Gym Assistant**          | IoT Simulation, Heart-Rate Zone Analysis |
| 4 | 📊 **AI Fitness Habit Tracker**     | Behavioral Analytics, Skip Prediction    |
| 5 | 🤖 **Virtual Gym Buddy**            | Sentiment Analysis, Conversational AI    |
| 6 | 🎯 **Pose-to-Performance Analyzer** | Motion Analysis, Performance Scoring     |
| 7 | 🗺️ **Gym Recommender & Planner**   | Recommendation Engine, Challenges        |

---

## 🛠️ Technology Stack

| Layer                 | Technologies                                |
| --------------------- | ------------------------------------------- |
| **Frontend**          | React.js, Vite                              |
| **Backend**           | Python, FastAPI                             |
| **AI/ML**             | MediaPipe, OpenCV, scikit-learn             |
| **Conversational AI** | NLP, Sentiment Analysis, Rule-Based Systems |
| **Analytics**         | Custom Scoring & Behavioral Algorithms      |

---

## 🚀 Setup & Execution

### Backend

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload --port 8000
```

Backend: **http://localhost:8000**
API Documentation: **http://localhost:8000/docs**

### Frontend

```bash
cd frontend
npm install
npm run dev
```

Frontend: **http://localhost:3000**

### Production

Configure the required environment variables and run:

```bash
cd backend
uvicorn main:app --host 0.0.0.0 --port "${PORT:-8000}"
```

For the frontend:

```bash
cd frontend
npm ci
npm run build
```

The generated `frontend/dist` directory can then be deployed to a static hosting service.

The **AI Gym Trainer** uses the bundled MediaPipe pose model to perform real-time pose landmark detection, exercise form analysis, repetition counting, and visual feedback.

---

## 📁 Project Architecture

```text
ai-gym-fitness/
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   └── routers/
│       ├── gym_trainer.py
│       ├── dietician.py
│       ├── smart_gym.py
│       ├── habit_tracker.py
│       ├── virtual_buddy.py
│       ├── pose_analyzer.py
│       └── gym_recommender.py
│
└── frontend/
    ├── package.json
    ├── vite.config.js
    ├── index.html
    └── src/
        ├── main.jsx
        ├── App.jsx
        ├── App.css
        └── components/
            ├── GymTrainer.jsx
            ├── Dietician.jsx
            ├── SmartGym.jsx
            ├── HabitTracker.jsx
            ├── VirtualBuddy.jsx
            ├── PoseAnalyzer.jsx
            └── GymRecommender.jsx
```

---

## 🔗 API Overview

### Module 1 — AI Gym Trainer

* `POST /api/gym-trainer/analyze-frame` — Analyze exercise posture from an image
* `POST /api/gym-trainer/generate-plan` — Generate a personalized workout plan
* `GET /api/gym-trainer/exercises` — Retrieve supported exercises

### Module 2 — AI Dietician

* `POST /api/dietician/diet-plan` — Generate a personalized diet plan
* `POST /api/dietician/grocery-list` — Generate a weekly grocery list
* `POST /api/dietician/track-meal` — Log and analyze meals

### Module 3 — Smart Gym

* `POST /api/smart-gym/monitor` — Process simulated gym sensor data
* `POST /api/smart-gym/adjust-resistance` — Dynamically adjust equipment resistance
* `GET /api/smart-gym/equipment-status` — Check equipment status

### Module 4 — Habit Tracker

* `POST /api/habit-tracker/predict-skip` — Estimate workout skip probability
* `POST /api/habit-tracker/log-workout` — Record completed workouts
* `GET /api/habit-tracker/leaderboard/weekly` — Retrieve weekly rankings

### Module 5 — Virtual Gym Buddy

* `POST /api/virtual-buddy/chat` — Interact with the AI fitness companion
* `POST /api/virtual-buddy/analyze-emotion` — Analyze user sentiment/emotion
* `GET /api/virtual-buddy/daily-quote` — Retrieve motivational content

### Module 6 — Pose Analyzer

* `POST /api/pose-analyzer/analyze-session` — Evaluate workout performance
* `POST /api/pose-analyzer/weekly-performance` — Generate weekly performance reports
* `GET /api/pose-analyzer/efficiency-tips/{exercise}` — Provide exercise-specific tips

### Module 7 — Gym Recommender

* `POST /api/gym-recommender/recommend-gyms` — Recommend suitable gyms
* `POST /api/gym-recommender/recommend-program` — Recommend fitness programs
* `GET /api/gym-recommender/challenges` — Retrieve available fitness challenges

---

## 📊 Project Deliverables

* ✅ AI Gym Trainer using MediaPipe pose detection
* ✅ AI Dietician with BMI, TDEE, and meal planning
* ✅ Smart Gym simulation with IoT and heart-rate monitoring
* ✅ Behavioral AI-based workout habit tracker
* ✅ Virtual Gym Buddy with sentiment analysis
* ✅ Pose-based workout performance evaluation
* ✅ Gym and fitness-program recommendation system
* ✅ Interactive React fitness dashboard
* ✅ FastAPI backend with RESTful APIs

---


**Made by Rakshit Swami**
**Indian Institute of Technology Bombay (IIT Bombay)**
**AI/ML Project**
