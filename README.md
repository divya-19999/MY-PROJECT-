# 🌱 JanRakshak AI
**"Predict Before It's Critical"**

![JanRakshak Cover](https://via.placeholder.com/800x400/1b4332/74c69d?text=JanRakshak+AI+Rural+Health+Platform)

JanRakshak AI is a powerful, offline-capable rural health intelligence platform meticulously designed to empower India's 1.2 million ASHA (Accredited Social Health Activist) workers. By bringing fast, low-latency AI health screening directly to any smartphone, we aim to bridge the primary healthcare access gap for over 600 million rural Indians.

## 🏆 National Level Hackathon 2026 Project

Built for speed, accessibility, and real-world impact, this lightweight Progressive Web App (PWA) requires no heavy cloud dependency and provides responses in under 100ms. It translates complex health vitals into actionable risk scores and guides healthcare workers through appropriate treatments or emergency procedures.

## ✨ Core Features & Innovations

- 🧠 **AI Risk Scoring Engine:** Analyzes patient vitals (Age, Weight, Blood Pressure, Glucose, Hemoglobin) locally to calculate risk percentiles for conditions like Heart Disease, Diabetes, and Anemia. Adjusts dynamically to factors like obesity.
- 🌐 **Real-Time Multilingual Support:** Native, instant translation across **English**, **Hindi (हिन्दी)**, and **Telugu (తెలుగు)** without relying on heavy third-party NPM libraries.
- 📍 **GPS-Anchored Health Map:** One-tap GPS integration using Leaflet.js that identifies health centers and hospitals within a 1.5km radius of the patient.
- 💊 **Fuzzy Medicine Search & Prescriptions:** Instant lookup for 20+ diseases. Fast fuzzy search (e.g., "loose motion" maps to Diarrhea) providing brand names (Dolo, Glycomet), dosage, and treatment duration.
- 🌿 **Traditional Home Remedy Engine:** A culturally localized database of 80+ Indian remedies (Karela, Giloy, Papaya Leaf) complete with step-by-step preparation instructions.
- 📞 **1-Tap Emergency Routing:** Bypasses manual dialing by using built-in `tel:` protocols to dispatch 108/102/112 emergency services directly from the browser during critical situations.

## 🏗️ Technical Architecture

JanRakshak AI is a lightweight, full-stack application designed specifically for low-resource environments (e.g., ₹6000 Android smartphones, 2G/3G networks).

- **Frontend:** React 18 + Vite (Fast PWA-ready builds).
- **Backend:** Python Flask (Lightweight API, CORS enabled).
- **Mapping:** Leaflet.js + OpenStreetMap (OSM) for offline-capable real-location rendering.
- **AI/Logic:** Custom Scoring Algorithm tailored for clinical accuracy and explainability.
- **i18n:** Custom `translations.js` for instant multilingual switching.

## 🚀 Run Locally

### Prerequisites
- Node.js (v16+)
- Python (v3.8+)

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/JanRakshak-AI.git
cd JanRakshak-AI
```

### 2. Start the Backend (Flask API)
```bash
cd backend
python -m venv .venv

# On Windows
.venv\Scripts\activate
# On Mac/Linux
source .venv/bin/activate

pip install -r requirements.txt
python app.py  # or python app_utf8_clean.py
```
*The backend will run on `http://localhost:5000`*

### 3. Start the Frontend (React + Vite)
```bash
# Open a new terminal
cd JanRakshak-AI/frontend
npm install
npm run dev
```
*The frontend will run on `http://localhost:5173` (or the port Vite provides).*

## 🌍 Social Impact
This platform is built in alignment with:
- **SDG 3** (Good Health & Well-being)
- **Ayushman Bharat** & **National Health Mission (NHM)**
- India's **ASHA Digitisation Program**

*A Healthy India is a Prosperous India. Built with ❤️ for Rural India by the JanRakshak AI Team.*
