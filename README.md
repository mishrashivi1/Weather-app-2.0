# 🌤️ Weather-App

A sleek, card-based weather application that fetches real-time weather data using a public API and displays it in a modern mobile-style UI.

## 📸 Preview
<img width="1920" height="1027" alt="Screenshot (82)" src="https://github.com/user-attachments/assets/f0f05341-4e69-4454-9223-eb5daad35b0a" />

The app shows:
- A search bar to look up any city
- City name with country flag emoji 🇮🇳
- A weather condition icon (sun, cloud, rain, etc.)
- Current temperature in Celsius (°C)
- Weather condition label (e.g., haze, sunny, cloudy)
- Two info cards — **Clouds %** and **Humidity %**

## 🚀 Features

- Search weather by city name
- Real-time data from a free public weather API (no API key required)
- Displays temperature, cloud coverage, and humidity
- Country flag shown alongside city name
- Clean card UI with color-coded info tiles
- Mobile-friendly centered layout

## 🛠️ Tech Stack

- **HTML** — Page structure
- **CSS** — Card layout and color-coded info tiles
- **JavaScript** — Fetch API calls and dynamic DOM updates
- **Public Weather API** — No sign-up or API key needed
- **GitHub Codespaces** — Hosted via `github.dev`

## 🔧 Setup & Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/mishrashivi1/Weather-app-2.0
   cd weather-app
   ```

2. **Open in browser:**

   No dependencies or build tools required. Just open `index.html`:

   ```bash
   open index.html
   ```

   Or run with a live server:

   ```bash
   npx live-server
   ```

## 🖥️ How It Works

1. The user types a city name (e.g., `Lucknow`) into the search bar and hits the search icon.
2. The app calls a **free public weather API** using `fetch()`:

   ```javascript
   fetch(`https://wttr.in/${city}?format=j1`)
   ```

3. The JSON response is parsed to extract:
   - Temperature
   - Weather description
   - Cloud coverage percentage
   - Humidity percentage
   - Country information (for the flag)
4. The UI card updates dynamically with the fetched data.

## 📁 Project Structure

```
weather-app/
├── index.html       # App structure and weather card layout
├── style.css        # Card styling, color tiles, and layout
├── script.js        # API fetch logic and DOM rendering
└── README.md        # Project documentation
```

## ⚠️ Notes

- Uses a **free public API** — no registration or API key needed.
- Public APIs may have occasional downtime or rate limits.
- City names should be spelled correctly for accurate results.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
