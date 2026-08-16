# Travel Advisory

Ayubowan🙏

This project is a travel safety and advisory app for visiting tourists in Srilanka.
It helps users choose safer places by combining map search, weather conditions, safety scoring, and local etiquette tips.

## What The System Does

- Lets users pick a location on a map (or search manually).
- Fetches weather data for that location.
- Calculates a safety score and risk level from live conditions.
- Shows local etiquette guidance for the selected place type.
- Supports user accounts and incident reporting workflow.

## Main Features

- Interactive Mapbox map with:
  - search by place name
  - "find my location" support
  - Sri Lanka-focused map bounds
- Weather API integration for real-time conditions.
- Safety score API (`0-100`) with risk factors.
- Etiquette API with do/don't guidance by location type.
- JWT authentication and role-based access (including admin report review).

## SPECIALTY

- **Creativity:** It combines practical travel safety with cultural behavior guidance in one experience, not just a weather app or a map app.
- **Data-driven:** Recommendations are based on live location + weather data, and can be improved with real user reports from the field.
- **Real-world use:** A traveler can pick a place, quickly see risk level, and learn what behavior is respectful/safe before visiting.

## Setup

### 1) Backend (.NET 8 + PostgreSQL)

1. Go to backend:
   - `cd backend/backend`
2. Restore and run:
   - `dotnet restore`
   - `dotnet run`
3. Backend starts on:
   - `http://localhost:5251` (used by frontend proxy)

### 2) Frontend (React + Vite)

1. Open a new terminal and go to frontend:
   - `cd frontend/app`
2. Install and run:
   - `npm install`
   - `npm run dev`
3. Open:
   - `http://localhost:5173`

### 3) Required Config

Backend config is in `backend/backend/appsettings.json`.
Before real deployment, replace local/dev secrets with your own values:

- PostgreSQL connection string
- JWT key/issuer/audience
- Mapbox access token
- OpenWeather API key(have an old key before subscription was introduced lol)

---

That is it. Run backend + frontend, then open the app and test by searching a location in Sri Lanka.

## Screenshots


<img width="1350" height="604" alt="travel-advisory1" src="https://github.com/user-attachments/assets/0181b034-f38f-4dc8-9e44-bd5f31010a6c" />
<img width="967" height="463" alt="travel-advisory2" src="https://github.com/user-attachments/assets/cfd25bde-ea53-4b05-b249-e3462755063c" />


