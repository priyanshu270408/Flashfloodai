🌊 FLOODGUARD AI

Predict Early. Warn Faster. Save Lives.

AI-Powered Flash Flood Prediction & Early Warning System for Hilly Regions

«Smart India Hackathon Prototype — SIH26192»

---

📌 Overview

FLOODGUARD AI is an AI-powered decision-support and early-warning platform designed to help predict and monitor flash-flood risks in hilly regions.

The system combines multiple environmental and geographical data sources such as:

- 🌧️ Rainfall
- 🌦️ Weather forecasts
- 🌊 River and water levels
- 💧 Soil moisture
- 🏔️ Elevation and terrain slope
- 🗺️ Geographic information
- 📊 Historical flood data

These inputs are processed through an AI/ML prediction pipeline to estimate flood probability and risk level, helping authorities and citizens take timely action.

---

🎯 Problem Statement

SIH26192 — Flash Flood Prediction for Hilly Regions

Hilly regions can experience sudden flash floods due to intense rainfall, rapid water accumulation, steep terrain, and rising river levels.

Traditional monitoring systems may not provide sufficiently localized or timely warnings.

FLOODGUARD AI aims to provide an integrated platform for:

«Data → Prediction → Risk Assessment → Early Warning → Response»

---

💡 Our Solution

FLOODGUARD AI combines:

Weather Data
     +
Rainfall Data
     +
River Data
     +
Soil Data
     +
Terrain Data
     +
Historical Data
        ↓
   Data Processing
        ↓
     AI / ML Model
        ↓
  Flood Probability
        ↓
    Risk Engine
        ↓
 Early Warning System
        ↓
 ┌───────────────┐
 │   Authorities │
 │   Citizens    │
 └───────────────┘

---

🚀 Key Features

🧠 AI Flood Prediction

Predicts flood probability using multiple environmental factors.

Provides:

- Flood probability
- Risk level
- Model confidence
- Prediction horizon
- Contributing factors
- Recommended action

---

🗺️ Live Flood Risk Map

Interactive GIS map showing:

- Flood-risk zones
- Rivers and streams
- Rainfall hotspots
- Monitoring stations
- Villages and roads
- Emergency shelters
- Safe zones
- Flood reports

Built using Leaflet + OpenStreetMap.

---

🌧️ Weather & Rainfall Monitoring

Monitor:

- Current rainfall
- Cumulative rainfall
- Forecast rainfall
- Temperature
- Humidity
- Wind speed
- Atmospheric conditions

---

🌊 River Monitoring

Track:

- Current water level
- Danger level
- Rate of rise
- Predicted water level
- River monitoring stations

---

🚨 Early Warning System

The platform classifies risk into:

Risk| Probability| Meaning
🟢 LOW| 0–30%| Normal monitoring
🟡 MODERATE| 30–60%| Increased monitoring
🟠 HIGH| 60–80%| Warning/preparedness
🔴 CRITICAL| 80–100%| Emergency response

Risk thresholds can be configured according to deployment requirements.

---

🏛️ Authority Control Room

Authorities can:

- Monitor high-risk areas
- Review AI predictions
- View active alerts
- Review supporting data
- Approve warnings
- Resolve alerts
- Monitor shelters
- View citizen flood reports
- Analyze historical events

---

📱 Citizen Safety Interface

Citizens can:

- Check local flood risk
- View active warnings
- Find nearby shelters
- View evacuation information
- Report flooding
- Share location
- Access emergency information

The interface is designed to be mobile-first and easy to understand during emergencies.

---

🏠 Shelter & Evacuation Support

Display:

- Emergency shelters
- Shelter capacity
- Available capacity
- Safe zones
- Suggested evacuation routes

«Evacuation routes shown by the prototype should be treated as decision-support information unless connected to verified official routing data.»

---

📸 Citizen Flood Reporting

Citizens can report flooding by submitting:

- Location
- Flood severity
- Description
- Photo
- Timestamp

Reports can be stored and displayed to authorities through the control room.

---

📊 Historical Analytics

Analyze:

- Previous flood events
- Rainfall patterns
- River-level trends
- Flood frequency
- High-risk regions
- Prediction performance

---

🌐 Multilingual Support

FLOODGUARD AI supports multiple Indian languages:

- 🇬🇧 English
- 🇮🇳 हिंदी
- বাংলা
- मराठी
- ગુજરાતી
- தமிழ்
- తెలుగు
- ಕನ್ನಡ
- മലയാളം
- ਪੰਜਾਬੀ
- ଓଡ଼ିଆ
- অসমীয়া
- اردو

The language selection is persistent, and RTL support is provided for Urdu.

---

🏗️ System Architecture

                         FLOODGUARD AI
                               │
              ┌────────────────┴────────────────┐
              │                                 │
          Frontend                         Backend/API
         Next.js                              │
              │                               │
              │                    ┌──────────┼──────────┐
              │                    │          │          │
              │                Supabase     ML       Data APIs
              │                    │          │          │
              └────────────────────┴──────────┴──────────┘
                               │
                        Risk Assessment
                               │
                        Early Warning
                               │
                   ┌───────────┴───────────┐
                   │                       │
              Authorities              Citizens

---

🛠️ Technology Stack

Frontend

- Next.js
- React
- TypeScript
- Tailwind CSS
- shadcn/ui
- Recharts
- Leaflet
- React-Leaflet
- Lucide React

Backend

- Next.js API routes / server-side APIs
- REST-style API architecture
- Zod/input validation where applicable

Database & Authentication

- Supabase
- PostgreSQL
- Supabase Auth
- Supabase Storage
- Row Level Security

AI / Machine Learning

- Python
- Pandas
- NumPy
- Scikit-learn
- Random Forest
- Logistic Regression
- XGBoost where available
- FastAPI for ML API where required

GIS

- Leaflet
- OpenStreetMap
- GeoJSON

Deployment

- Vercel — Next.js application
- Supabase — Database/Auth/Storage
- Separate ML API deployment when required

---

📂 Project Structure

floodguard-ai/
│
├── app/
│   ├── dashboard/
│   ├── risk-map/
│   ├── prediction/
│   ├── weather/
│   ├── alerts/
│   ├── historical-data/
│   ├── reports/
│   ├── control-room/
│   ├── shelters/
│   ├── evacuation/
│   ├── report-flood/
│   ├── about/
│   ├── settings/
│   ├── login/
│   └── register/
│
├── components/
│   └── ui/
│
├── hooks/
├── lib/
├── services/
├── types/
├── data/
├── public/
│
├── supabase/
│   ├── schema.sql
│   └── seed.sql
│
├── ml/
│   ├── model/
│   ├── training/
│   ├── preprocessing/
│   ├── prediction/
│   └── README.md
│
├── scripts/
│
├── .env.example
├── .gitignore
├── package.json
├── next.config.*
└── README.md

---

⚙️ Getting Started

Prerequisites

Install:

- Node.js 20+
- npm
- Git

For ML development:

- Python 3.10+

You will also need a Supabase project if you want to use the database/authentication functionality.

---

1. Clone the Repository

git clone YOUR_GITHUB_REPOSITORY_URL
cd floodguard-ai

---

2. Install Dependencies

npm install

---

3. Configure Environment Variables

Create:

.env.local

Copy the values from:

.env.example

Example:

NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=

SUPABASE_SERVICE_ROLE_KEY=

ML_API_URL=

WEATHER_API_KEY=

DATA_MODE=mock

Important

Never commit ".env.local" or any file containing secrets.

---

🧪 Mock Mode

FLOODGUARD AI supports a complete demo/mock mode.

Set:

DATA_MODE=mock

Mock mode allows the application to run without external API credentials.

It provides demonstration data for:

- Weather
- Rainfall
- River levels
- Soil moisture
- Terrain
- Flood predictions
- Risk zones
- Alerts
- Shelters
- Historical flood events

This makes the project suitable for demonstrations and hackathon presentations.

---

🌐 Live Mode

For real integrations, configure the required APIs and set:

DATA_MODE=live

The service layer is designed so mock data can be replaced with real data sources without changing the frontend architecture.

---

🗄️ Supabase Setup

Create a Supabase project.

Then run:

supabase/schema.sql

to create the database structure.

Run:

supabase/seed.sql

to insert demonstration data.

Configure:

NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=

If server-side administrative operations are required:

SUPABASE_SERVICE_ROLE_KEY=

Never expose the service-role key to the browser.

---

🤖 ML Service

If the project uses the separate FastAPI ML service:

cd ml

Create a virtual environment:

python -m venv .venv

Activate it.

Windows

.venv\Scripts\activate

Linux/macOS

source .venv/bin/activate

Install dependencies:

pip install -r requirements.txt

Run the ML service:

uvicorn main:app --reload

Configure the frontend/backend:

ML_API_URL=YOUR_DEPLOYED_ML_API_URL

---

🧠 Prediction API

Example request:

POST /api/predictions

Example input:

{
  "location": "Demo Valley",
  "rainfall_1h": 72,
  "rainfall_24h": 180,
  "river_level": 4.8,
  "river_rise_rate": 0.4,
  "soil_moisture": 82,
  "elevation": 1200,
  "slope": 38
}

Example response:

{
  "flood_probability": 87,
  "risk_level": "HIGH",
  "confidence": 91,
  "prediction_horizon": "3 hours",
  "contributing_factors": [
    "Heavy rainfall",
    "Rapid river-level rise",
    "High soil saturation",
    "Steep terrain"
  ],
  "recommendation": "Prepare for possible flooding and follow official emergency instructions."
}

---

🔌 API Endpoints

Example application endpoints:

GET  /api/weather
GET  /api/rainfall
GET  /api/river
GET  /api/locations
GET  /api/risk-zones
GET  /api/alerts
GET  /api/shelters
GET  /api/historical-floods

POST /api/predictions
POST /api/flood-reports
POST /api/alerts

POST /api/alerts/:id/approve
POST /api/alerts/:id/resolve

The exact endpoints may vary depending on the final implementation.

---

▶️ Development

Run the development server:

npm run dev

Open:

http://localhost:3000

---

🏭 Production Build

Run:

npm run lint

Then:

npm run build

Start the production server:

npm start

---

🚀 Deploy to Vercel

Step 1 — Push to GitHub

git init
git add .
git commit -m "Initial FloodGuard AI implementation"
git branch -M main
git remote add origin YOUR_GITHUB_REPOSITORY_URL
git push -u origin main

Step 2 — Import into Vercel

Import the GitHub repository into Vercel.

Vercel should automatically detect the Next.js project.

Use:

Build Command:
npm run build

---

Step 3 — Add Environment Variables

Add the required production variables in Vercel:

NEXT_PUBLIC_SUPABASE_URL
NEXT_PUBLIC_SUPABASE_ANON_KEY
ML_API_URL
WEATHER_API_KEY
DATA_MODE

Only add variables that are actually required by the deployed configuration.

---

🧩 Deployment Architecture

The recommended production architecture is:

                 ┌───────────────────┐
                 │      Vercel       │
                 │    Next.js App    │
                 └─────────┬─────────┘
                           │
                    Backend/API
                           │
             ┌─────────────┼─────────────┐
             │             │             │
         Supabase       ML API       Weather API
             │             │             │
             └─────────────┴─────────────┘
                           │
                     FloodGuard AI

The Python ML service should be deployed separately if required.

---

🔐 Security

Never commit:

.env
.env.local
.env.production
API keys
Passwords
Service-role keys
Private credentials

The Supabase service-role key must only be used on trusted server-side environments.

Client-side environment variables should only contain values that are safe to expose.

---

🧪 Testing Checklist

Before deployment, verify:

Frontend

- [ ] Dashboard loads
- [ ] Navigation works
- [ ] Risk map works
- [ ] Charts work
- [ ] Alerts work
- [ ] Mobile layout works
- [ ] Language switching works

Backend

- [ ] API endpoints work
- [ ] Validation works
- [ ] Error handling works
- [ ] Authentication works

Database

- [ ] Supabase connection works
- [ ] Tables exist
- [ ] RLS policies work
- [ ] Seed data loads
- [ ] Storage works

ML

- [ ] Model loads
- [ ] Prediction endpoint works
- [ ] Mock prediction works
- [ ] Risk classification works

Deployment

- [ ] "npm run build" succeeds
- [ ] No localhost URLs remain
- [ ] Environment variables are configured
- [ ] Vercel deployment succeeds

---

🔄 Demo Flow

The complete hackathon demonstration can follow this flow:

Select Hilly Region
        ↓
Environmental Data Loads
        ↓
Rainfall / River / Soil / Terrain Analysis
        ↓
AI Flood Prediction
        ↓
Flood Probability Generated
        ↓
Risk Level Calculated
        ↓
Early Warning Recommendation
        ↓
Authority Control Room
        ↓
Alert Review
        ↓
Alert Approval
        ↓
Citizen Warning
        ↓
Shelter / Evacuation Information
        ↓
Citizen Flood Report
        ↓
Authority Monitoring

---

🎯 Future Improvements

Potential future enhancements include:

- Real-time satellite imagery
- More government/open-data integrations
- Advanced hydrological models
- High-resolution DEM analysis
- IoT water-level sensors
- Automated rainfall station integration
- SMS/IVR warning systems
- Offline-first citizen application
- More regional languages
- Improved evacuation routing
- Continuous model retraining
- Explainable AI
- More advanced spatiotemporal ML models

---

⚠️ Disclaimer

FLOODGUARD AI is a Smart India Hackathon prototype created for demonstration and research purposes.

It is a decision-support and early-warning prototype and does not replace official government disaster-management authorities, emergency services, weather warnings, or evacuation instructions.

Predictions and mock data shown by the prototype should not be treated as real-world emergency warnings.

---

👥 Team

Project: FLOODGUARD AI
Problem Statement: SIH26192
Theme: Disaster Management
Event: Smart India Hackathon

---

📄 License

This project is intended for educational, research, and hackathon purposes.

Add an appropriate open-source license here if the project is released publicly.

---

🌊 FLOODGUARD AI

Predict Early. Warn Faster. Save Lives.
