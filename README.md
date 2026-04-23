# 🌦️ Weather App

A simple, elegant weather application that fetches real-time weather data using the OpenWeatherMap API.

## Features ✨

- 🔍 Search weather by city name
- 🌡️ Display temperature, humidity, wind speed, and "feels like" temperature
- 💾 Local caching for faster repeated searches
- 📱 Responsive design with beautiful gradient background
- ⌨️ Enter key support for quick searches
- ⚠️ Helpful error messages with setup guidance

## Setup Instructions 🚀

### 1. Get Your Free API Key
1. Visit [OpenWeatherMap API](https://openweathermap.org/api)
2. Click **Sign Up** and create a free account
3. Verify your email
4. Log in and go to **API Keys** section
5. Copy your default API key

### 2. Configure Your API Key

**Option A: Direct in HTML (Local Testing)**
- Open `index.html`
- Find the line: `const apiKey = "YOUR_API_KEY";`
- Replace `YOUR_API_KEY` with your actual API key

**Option B: Using .env File (Recommended for Production)**
1. Copy `.env.example` to `.env`
   ```bash
   cp .env.example .env
   ```
2. Edit `.env` and add your API key:
   ```
   OPENWEATHER_API_KEY=your_actual_api_key_here
   ```
3. `.env` is in `.gitignore` - it won't be committed to GitHub

### 3. Test the App
- Open `index.html` in your browser
- Search for any city
- You should see the weather data instantly! 🎉

## ⚠️ Security Note

**Never commit your API key to GitHub!**
- The `.gitignore` file protects `.env` files
- Use the `.env.example` as a template
- For production, use GitHub Secrets or environment variables

## File Structure

```
weather-app/
├── index.html          # Main application file
├── README.md           # This file
├── .gitignore          # Git ignore rules
├── .env.example        # Template for environment variables
└── .env                # Your personal API key (not committed)
```

## How It Works

1. User enters a city name
2. App fetches weather data from OpenWeatherMap API
3. Results are cached locally for efficiency
4. Weather data is displayed with emojis and formatting

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

Free to use and modify for personal projects.

## Support

If you encounter issues:
1. Check that your API key is correct and active
2. Verify your internet connection
3. Make sure the city name is spelled correctly
4. Check the browser console (F12) for error messages