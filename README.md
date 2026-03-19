# 🕌 Eid Jamaat Koi | ঈদ জামাত কই

> **Find Eid Jamaat timings near you — crowdsourced, real-time, and open-source.**

🔗 **Live App: [https://eid-jamaat-koi.vercel.app](https://eid-jamaat-koi.vercel.app)**

A mobile-first web app for discovering and reporting Eid prayer (Jamaat) timings at nearby mosques. Built entirely with vanilla web technologies — no build tools required.

![Status](https://img.shields.io/badge/status-live-brightgreen)
![Vercel](https://img.shields.io/badge/deployed_on-Vercel-black?logo=vercel)
![License](https://img.shields.io/badge/license-MIT-blue)
![Made With](https://img.shields.io/badge/made_with-❤️_and_JavaScript-yellow)

---

## 📅 Update Logs (v1.1.0)
- **New:** Replaced Leaflet.js with **Google Maps JavaScript API**.
- **New:** Established an instant **5km** localized data fetch to retrieve the most relevant local mosques.
- **New:** Added a real-time **Search Bar** to instantly filter both the Live Feed and map markers.
- **New:** Expanded explicit queries to concurrently fetch 6 unique keywords natively (**"Mosque"**, **"Eidgah"**, **"masjid"**, **"mosjid"**, **"ঈদ্গাহ"**, **"মসজিদ"**) ensuring zero local omissions.
- **New:** Integrated the Aladhan API to dynamically calculate and display accurate upcoming Gregorian dates for **Eid al-Fitr** and **Eid al-Adha**.
- **Fix:** Reduced search radius to 5km and optimized regex matching to prevent Overpass API server timeouts. Increased geolocation timeout for better GPS reliability.
- **Fix:** Resolved an Overpass API syntax error (HTTP 400 Bad Request) caused by an unescaped case-insensitive regex modifier that forced the app to fall back to hardcoded default coordinates.
- **Architecture:** Permanently migrated data fetching from OpenStreetMap Overpass API to **Google Places API** utilizing a concurrent, paginated search algorithm for 100% reliable, instantaneous loading.
- **New:** Eid dates now dynamically adjust based on user's **GPS location**. A custom longitudinal algorithm applies a +1-day offset for regions East of 60° longitude (South Asia, Southeast Asia, Oceania) to match real-world physical moon sighting practices.

---

## ✨ Features

- 📍 **Auto-Geolocation** — Detects your GPS coordinates automatically or defaults to a central fallback.
- 🕌 **Real Mosque Data** — Fetches up to ~180 local mosques and open-air Eidgahs natively using the **Google Places API** with local storage caching for immediate display.
- 🔍 **Real-Time Search** — Filter the live feed and map markers instantly by typing a mosque's name.
- 📋 **Live Feed** — Scrollable, sorted-by-distance cards with reported Jamaat times, distances, and elapsed time.
- 🗺️ **Interactive Map** — Full Google Maps integration with pulsing user markers and clickable mosque markers with popup details.
- ✅❌ **Voting System** — Upvote (সঠিক) or downvote (ভুল) reported times for community verification.
- ➕ **Report Times** — Submit new Jamaat timings via a sleek modal form with photo upload support.
- 🌙 **Dark Mode** — Auto-detects system preference, manual toggle, remembers your choice.
- 💾 **Supabase Backend** — Real-time database for reports and votes.
- 🇧🇩 **Bilingual UI** — English and Bengali (বাংলা) labels throughout.
- 📱 **Mobile-First** — Optimized for smartphones with responsive design.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Structure & semantics |
| **Tailwind CSS** (CDN) | Utility-first styling |
| **Vanilla JavaScript** | All logic, no frameworks |
| **Google Maps API** | Interactive map rendering |
| **Google Places API** | Local mosque/Eidgah POI queries |
| **Supabase** (CDN) | Database for reports & votes |

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
