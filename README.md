# 🌤️ Weather App

A simple and clean weather application built with **HTML, CSS, and JavaScript** that fetches real-time weather data using the OpenWeatherMap API.

## 📸 Preview

> Search any city to get live weather updates including temperature, humidity, and wind speed.

## 🚀 Features

- 🔍 Search weather by city name
- 🌡️ Displays current temperature in °C
- 💧 Shows humidity percentage
- 💨 Shows wind speed in Km/H
- 🖼️ Dynamic weather icons (Clouds, Clear, Rain, Mist, Snow)
- ❌ Friendly error UI for invalid/unknown locations

## 🛠️ Tech Stack

- **HTML5**
- **CSS3**
- **JavaScript (ES6+)**
- **OpenWeatherMap API**
- **Font Awesome Icons**

## 📁 Project Structure

```
weather-app/
│
├── index.html        # Main HTML structure
├── style.css         # Styling and layout
├── script.js         # API logic and DOM manipulation
└── assets/
    ├── cloud.png
    ├── clear.png
    ├── rain.png
    ├── mist.png
    ├── snow.png
    └── 404.png
```

## ⚙️ Setup & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/weather-app.git
   cd weather-app
   ```

2. **Get an API key**
   - Sign up at [OpenWeatherMap](https://openweathermap.org/api)
   - Generate a free API key

3. **Add your API key**
   - Open `script.js`
   - Replace the value of `api_key` with your own key:
     ```js
     const api_key = "c1b6f71c72447b4cb78499bb154473c6";
     ```

4. **Run the app**
   - Open `index.html` directly in your browser, or use a live server extension (e.g., VS Code Live Server)

## 🔑 API Reference

This project uses the [OpenWeatherMap Current Weather API](https://openweathermap.org/current):

```
GET https:`https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${api_key}`
```

## 📌 Notes

- Temperature is converted from Kelvin to Celsius manually (`temp - 273.15`)
- The app handles invalid city names with a custom 404 UI

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
