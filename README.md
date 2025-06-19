# 🏃‍♂️ Where2Run-FullStack – Smart Route Generation & Training Platform

**Where2Run-FullStack** is the next-generation rebuild of the original Streamlit-based MVP — built to scale with a modern, production-ready tech stack.

The platform helps runners and cyclists plan smarter, more personalized routes using high-quality routing data, real-time logic, and flexible input options. This rebuild will support authentication, training plans, and user-specific route logic via a modular full-stack architecture.

---

## 🌐 Live App (MVP Legacy)

The original MVP is still live:  
https://where2run-beta.streamlit.app

---

## 🚧 Why This Rebuild?

To scale beyond a Streamlit MVP and support features like user accounts, training plan syncing, and future monetization, I’m rebuilding **Where2Run** using a production-grade tech stack: **React**, **FastAPI**, and **Azure PostgreSQL** — all fully cloud-deployed and version-controlled.

This full-stack transition is designed to:

- 💡 Demonstrate **scalable backend architecture** and **modern frontend development**
- 🔐 Lay the groundwork for **CI/CD pipelines**, **user authentication**, and **mobile-first design**
- ☁️ Strengthen hands-on experience with **cloud-native tools** and **DevOps workflows** aligned with modern **data engineering roles**

---

## 🧱 Tech Stack

| Layer        | Tech                                 |
|--------------|--------------------------------------|
| Frontend     | React (Vite or Create React App)     |
| Backend      | FastAPI (Python)                     |
| Database     | Azure PostgreSQL                     |
| Hosting      | Render (Backend) + Vercel/Netlify (Frontend) + GitHub CI/CD |
| Routing APIs | OpenRouteService, Overpass API       |
| Geocoding    | LocationIQ                           |
| Versioning   | GitHub + GitHub Projects             |

---

## ✅ Current Key Features

- 📍 Input your starting location (address or coordinates)
- 📏 Select route type and target mileage:
  - Loop
  - Out-and-Back (with directional bias)
  - Destination-based (run *to* a location)
- 🎯 Optional customization:
  - Add scenic waypoints or business destinations
  - Include preset route segments (e.g., bridge loops)
  - Filter by environment (trails, shaded, urban, etc.)
- 🌄 Elevation heatmap overlay for route preview
- 📤 Download GPX file for Garmin, Strava, or watch syncing
- 🧭 Environment-aware logic powered by Overpass API with fallback system


## 🚧 Planned Core Features

- 🏁 **Training Plan Sync**  
  Display today’s mileage from selected plan, sync with race date, and show countdown

- 🧠 **Personalized Suggestions**  
  Recommend routes based on historical behavior, past mileage, and user preferences

- ⛰️ **Elevation Tuning**  
  Adjust route based on preferred terrain: hills vs flat

- 📦 **User Profiles**  
  Save favorite routes, training plans, and recent locations

- 📥 **Smarter GPX Export**  
  Support syncing with Google Fit / Apple Health and training apps

- 🧱 **Full Backend Integration**  
  Centralized FastAPI route engine + PostgreSQL caching + user auth

---

## 🔧 Features in Development

- **Integrated Training Plans**  
  Structured race prep for Marathon and Half Marathon distances with:
  - Visual progress tracking
  - Countdown to race day
  - Real-world race GPX integration (future)
  - Calendar syncing (future)

- **Personalized Route Logic**  
  Suggest routes based on user history, past preferences, and training plan mileage

- **Elevation-Based Filtering**  
  Select route difficulty by prioritizing flat or hilly segments

- **Backend Infrastructure (FastAPI)**  
  - Modular route generation endpoints  
  - Centralized logic for route types, environment filtering, and caching

- **PostgreSQL Data Model (Azure)**  
  - User authentication and preferences  
  - Saved routes and history  
  - Overpass and geocode caching  
  - Training plan linkage per user

- **Frontend Development (React + TailwindCSS)**  
  - Modern, mobile-friendly interface  
  - Dynamic form inputs and route display components  
  - GPX download integration

- **Deployment Pipeline**  
  - Backend hosted on Render  
  - Frontend deployed on Vercel or Netlify  
  - GitHub-managed version control


---

## 📁 Folder Structure (Planned)

```
Where2Run-FullStack/
├── backend/                  # FastAPI app (Render-hosted)
│   ├── app/
│   │   ├── main.py
│   │   ├── routers/
│   │   └── utils/
│   └── requirements.txt
│
├── frontend/                 # React app (Vercel/Netlify-hosted)
│   ├── public/
│   ├── src/
│   └── package.json
│
├── database/                 # SQL schema setup
│   └── init.sql
│
├── .env.example              # Environment variable template
├── README.md
└── LICENSE
```

---

## 📌 Project Status

✅ MVP complete with Streamlit  
🚧 Full-stack rebuild in progress  
📅 Goal: Working React frontend + FastAPI endpoints by August 2025

---

## 🎯 Why I Built This

I’m currently training for another marathon, and I wanted a tool that not only supports my daily runs but aligns with my broader fitness goals. Most running apps felt either too rigid or locked behind paywalls.

Where2Run was born from my desire to merge two of my biggest passions — data and health. As a lifelong athlete and a dedicated data engineer, I wanted to build something that could evolve with my training while giving me the freedom to experiment, learn, and grow. This project isn’t just a tool for runners — it’s a reflection of my belief that data can empower better habits, smarter planning, and healthier lives.

Where2Run is the perfect intersection of my interests and a hands-on way for me to become a stronger, more well-rounded data engineer.


---

## 📜 License

This project is licensed for personal, non-commercial use only.  
All rights reserved © 2025 Zachary Ahearn.

---

## 📚 Acknowledgements

- OpenRouteService - https://openrouteservice.org  
- OpenStreetMap - https://www.openstreetmap.org  
- Overpass API - https://overpass-api.de  
- Azure (current production database) - https://azure.microsoft.com
