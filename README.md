# SafetyPulse Montgomery 🚨
### AI-Powered Public Safety Intelligence Dashboard
**WWV 2026 Hackathon Submission — Public Safety, Emergency Response & City Analytics**

> Built solo in under 48 hours with no prior AI or coding experience.

---

## 🌐 Live Demo
**[https://ram-dev-repo.github.io/safetypulse-montgomery/](https://ram-dev-repo.github.io/safetypulse-montgomery/)**

> ⚠️ Active API keys are included for judges to test immediately. Keys may expire over time — if you see any errors, see Setup Instructions below to generate free replacements in under 5 minutes.

---

## 🎬 Demo Video
https://youtu.be/xM_kyd5BuyY

---

## 💡 The Problem
Montgomery already has an official public safety dashboard — but it's designed for city analysts. Ordinary residents have no simple way to understand their local emergency data, or know when to call 911 versus the non-emergency line.

## ✅ The Solution
SafetyPulse Montgomery pulls **live data** directly from Montgomery's official ArcGIS APIs to give residents:
- At-a-glance 911 call stats and emergency trends
- Fire & medical crew response times by district
- An interactive safety map with fire stations, shelters and 311 issues
- **Live safety news** scraped in real-time via Bright Data SERP API
- An AI chatbot (Gemini 2.5 Flash) that answers plain-language resident questions

---

## 🔑 API Keys — For Judges

Active API keys are included in the deployed app for immediate testing.

**If keys have expired**, both can be replaced in under 5 minutes:

### 1. Google Gemini API Key (Free)
1. Go to [https://aistudio.google.com](https://aistudio.google.com)
2. Sign in with a Google account
3. Click **Get API Key** → **Create API Key**
4. Copy the key

### 2. Bright Data SERP API Key (Free trial — no credit card needed)
1. Go to [https://brightdata.com](https://brightdata.com) and sign up free
2. Navigate to **API Keys** → Create a new **SERP API** zone named `safetypulse_news`
3. Copy the API key

### 3. Replace Keys in the App
Open `index.html` in a text editor and find:
```javascript
const GEMINI_KEY = "your-key-here";
const BRIGHT_DATA_KEY = "your-key-here";
```
Replace with your keys, save, then open `index.html` in Chrome.

---

## 🏗️ Tech Stack
| Component | Technology |
|---|---|
| Data Source | Montgomery ArcGIS REST APIs (live) |
| News Scraping | Bright Data SERP API |
| AI Chatbot | Google Gemini 2.5 Flash |
| Maps | Leaflet.js + OpenStreetMap |
| Charts | Chart.js |
| Styling | Tailwind CSS |
| Hosting | GitHub Pages |

---

## 📊 Data Sources (All Live & Free)
- **911 Calls** — Montgomery ArcGIS FeatureServer (647,999 records)
- **Fire & Rescue Incidents** — Montgomery ArcGIS FeatureServer (55,000+ records)
- **Fire Station Locations** — Montgomery ArcGIS FeatureServer
- **Tornado Shelters** — Montgomery ArcGIS FeatureServer
- **311 Service Requests** — Montgomery GIS FeatureServer
- **Live News** — Google Search via Bright Data SERP API

---

## ✨ Key Features
- **Global Year Filter** — every stat, chart, insight and map updates instantly
- **Honest Data Transparency** — clearly flags unpublished data (e.g. 2026 fire incidents)
- **Response Time by District** — 24 districts ranked fastest to slowest
- **Live Safety News** — real-time headlines scraped via Bright Data
- **AI Chatbot** — resident-focused Q&A grounded in real Montgomery data
- **Non-Emergency Line** — 334-625-2651 prominently featured throughout

---

## 👤 About
Built by **Seetharam Meduru**, Splunk Observability Engineer, Sydney Australia.
Solo participant · No prior AI or coding experience · WWV 2026 Hackathon
