# 🌤️ Weather App

A clean, responsive weather app built with vanilla HTML, CSS, and JavaScript. Search for any city and get real-time temperature, weather description, humidity, and wind speed — powered by the OpenWeatherMap API.


## Features

- 🔍 Search weather by city name
- 🌡️ Real-time temperature (in °C)
- ☁️ Dynamic weather icons based on conditions (Clear, Clouds, Rain, Mist, Snow)
- 💧 Humidity and wind speed display
- 🚫 Graceful "location not found" handling for invalid city names
- 📱 Simple, responsive single-card UI

## Tech Stack

- **HTML5** – structure
- **CSS3** – styling and layout (Flexbox)
- **JavaScript (ES6+)** – fetch API, async/await, DOM manipulation
- **[OpenWeatherMap API](https://openweathermap.org/api)** – weather data
- **[Font Awesome](https://fontawesome.com/)** – icons

## Getting Started

### Prerequisites

You'll need a free API key from [OpenWeatherMap](https://openweathermap.org/api).

### Installation

1. Clone the repo
   ```bash
   git clone https://github.com/your-username/weather-app.git
   cd weather-app
   ```

2. Open `script.js` and add your API key:
   ```js
   const api_key = "YOUR_API_KEY_HERE";
   ```

3. Open `index.html` in your browser — no build step or server required.

   > Tip: for the best experience (and to avoid any CORS quirks), serve it locally with a tool like the VS Code **Live Server** extension instead of opening the file directly.

## Project Structure

```
weather-app/
├── index.html
├── style.css
├── script.js
├── pictures/
│   ├── clear.png
│   ├── cloud.png
│   ├── rain.png
│   ├── mist.png
│   ├── snow.png
│   ├── 404.png
│   └── kalen-emsley-Bkci_8qcdvQ-unsplash.jpg
└── README.md
```

> **Note:** Make sure the `pictures/` folder is included in your repo with all the images referenced in `index.html`, `style.css`, and `script.js` — the icons and background image won't load without them.

## How It Works

1. User types a city name and clicks search (or the app calls `checkWeather()`).
2. The app fetches current weather data from the OpenWeatherMap API.
3. If the city isn't found (`cod === 404`), an error state is shown.
4. Otherwise, temperature, description, humidity, wind speed, and a matching weather icon are rendered.

## Credits

- Background photo by [Kalen Emsley](https://unsplash.com/@kalenemsley) on [Unsplash](https://unsplash.com/)
- Weather data from [OpenWeatherMap](https://openweathermap.org/)
- Icons from [Font Awesome](https://fontawesome.com/)

## License

This project is open source and available under the [MIT License](LICENSE).
