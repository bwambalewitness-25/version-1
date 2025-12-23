# Expo Weather App

A minimal React Native (Expo) weather app that:

- Requests device location and shows current weather for that location
- Allows searching weather by city name
- Caches last fetched weather for offline viewing
- Uses OpenWeatherMap (free tier)

Requirements
- Node.js (16+ recommended)
- Expo CLI or use `npx expo`
- An OpenWeatherMap API key: https://openweathermap.org/api

Quickstart
1. Create a new project folder and copy these files into it.
2. Install dependencies:
   ```bash
   npm install
   # or
   yarn
   ```
3. Create a config file:
   - Copy `config.example.js` to `config.js`
   - Put your OpenWeatherMap API key in `config.js`:
     ```js
     export default {
       OPENWEATHER_API_KEY: "your_api_key_here"
     };
     ```
4. Run the app:
   ```bash
   npx expo start
   ```
   Open in Expo Go or an emulator.

Notes
- Location permission is requested at runtime. If denied, use the search to get weather by city.
- The app caches the last successful weather response locally.
- This is a starting point—features you might add: 5-day forecast, background updates, unit switching (C/F), pull-to-refresh, improved UI/animations, TypeScript.

If you want, I can:
- Convert this to TypeScript
- Add forecast pages and charts
- Integrate a remote sync or authentication
- Provide CI or stores (Redux/Zustand)