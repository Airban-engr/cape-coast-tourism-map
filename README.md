# Cape Coast Tourism Hotspots – Interactive Map

Live demo:https://airban-engr.github.io/cape-coast-tourism-map/

An interactive web map highlighting major tourism hotspots in and around Cape Coast, Ghana — including **Cape Coast Castle**, **Elmina Castle**, **Fort San Jago**, **Kakum National Park (Canopy Walkway)**, **Hans Cottage Botel**, **Elmina Harbour**, **Brenu Beach**, and more.

Built for clarity and speed using **Leaflet** + **GitHub Pages**. Designed to showcase how lightweight geospatial apps can support **tourism planning, storytelling, and visitor experience**.

---

## 🗺️ Features
- Styled circle markers by **type**: Historical, Cultural, Nature, Beach
- Clickable **popups**: name, type, city, and short description
- Auto **fit-to-bounds** on load
- Minimal **legend** (bottom-right)
- Static hosting on **GitHub Pages** for easy sharing

---

## 📁 Data
File: `data/tourism_hotspots.geojson`  
Fields:
- `name` – site name
- `type` – Historical | Cultural | Nature | Beach
- `city` – nearest city/town
- `description` – short note

> Coordinates are approximate (demo quality). For production use, replace with official data sources or verified GPS.

---

## 🚀 Run Locally
1. Clone this repo
2. From the project folder, start a simple server:
   ```bash
   # Python 3
   python -m http.server 5500
   ```
3. Open: `http://localhost:5500/`

---

## 🧩 Tech Stack
- [Leaflet](https://leafletjs.com/) for web mapping
- OpenStreetMap tiles for basemap
- Static hosting with GitHub Pages

---

## 🧭 Customize
- Replace `data/tourism_hotspots.geojson` with your own points
- Adjust color mapping in `index.html` → `typeColor()`
- Tweak popup fields in `onEachFeature` for richer content
- Update OG/Twitter meta tags in `<head>` for rich link previews

---

## 📂 Structure
```
cape-coast-tourism-map/
  index.html
  README.md
  preview.jpg (or .png)
  data/
    tourism_hotspots.geojson
```

