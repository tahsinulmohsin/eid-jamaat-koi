# 🕌 Eid Jamaat Koi | ঈদ জামাত কই

> **Find Eid Jamaat timings near you — crowdsourced, real-time, and open-source.**

A mobile-first web app for discovering and reporting Eid prayer (Jamaat) timings at nearby mosques. Built entirely with vanilla web technologies — no build tools required.

![Status](https://img.shields.io/badge/status-live-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Made With](https://img.shields.io/badge/made_with-❤️_and_JavaScript-yellow)

---

## ✨ Features

- 📍 **Auto-Geolocation** — Detects your GPS coordinates automatically; falls back to Azimpur, Dhaka if denied.
- 🕌 **Real Mosque Data** — Fetches nearby mosques from OpenStreetMap via the Overpass API (2.5km radius).
- 📋 **Live Feed** — Scrollable, sorted-by-distance cards with reported Jamaat times, distances, and elapsed time.
- 🗺️ **Interactive Map** — Full Leaflet.js map with pulsing user marker and clickable mosque markers with popup details.
- ✅❌ **Voting System** — Upvote (সঠিক) or downvote (ভুল) reported times for community verification.
- ➕ **Report Times** — Submit new Jamaat timings via a sleek modal form with photo upload support.
- 🇧🇩 **Bilingual UI** — English and Bengali (বাংলা) labels throughout.
- 📱 **Mobile-First** — Optimized for smartphones with responsive design.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Structure & semantics |
| **Tailwind CSS** (CDN) | Utility-first styling |
| **Vanilla JavaScript** | All logic, no frameworks |
| **Leaflet.js** (CDN) | Interactive map rendering |
| **OpenStreetMap** | Map tiles & geodata |
| **Overpass API** | Real-time mosque POI queries |

> **Zero build tools.** No Webpack, no Vite, no npm. Just a single `index.html` file.

---

## 🚀 Deploy to Vercel (3 Steps)

Deploy this app to the web in under 60 seconds:

### Step 1: Push to GitHub

Create a new GitHub repository (e.g., `eid-jamaat-koi`) and push this project:

```bash
git init
git add .
git commit -m "Initial commit: Eid Jamaat Koi"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/eid-jamaat-koi.git
git push -u origin main
```

### Step 2: Import to Vercel

1. Go to [vercel.com/new](https://vercel.com/new)
2. Click **"Import Git Repository"**
3. Select your `eid-jamaat-koi` repo
4. Leave all settings as default — Vercel will auto-detect the static HTML

### Step 3: Deploy

Click **"Deploy"**. That's it! Your app will be live at `https://eid-jamaat-koi.vercel.app` within seconds.

> 💡 **Tip:** Every push to `main` will auto-deploy. Add a custom domain from Vercel's dashboard if needed.

---

## 🏗️ Project Structure

```
eid-jamaat-koi/
├── index.html   ← Entire application (HTML + CSS + JS)
└── README.md    ← You are here
```

---

## 📄 License

MIT — use it, fork it, improve it. Eid Mubarak! 🌙
