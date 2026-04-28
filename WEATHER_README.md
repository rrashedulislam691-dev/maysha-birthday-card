## 🌤️ Weather Dashboard

A modern, responsive weather dashboard application that fetches real-time weather data from OpenWeatherMap API. Featuring beautiful animations, hourly forecasts, and 7-day predictions.

### ✨ Features

- 🌍 **Real-time Weather Data** - Current weather, temperature, humidity, wind speed, and more
- 📍 **Geolocation Support** - Get weather for your current location
- 🔍 **City Search** - Search weather for any city in the world
- 📋 **Recent Searches** - Quick access to previously searched cities (saved in localStorage)
- ⏰ **Hourly Forecast** - 8-hour forecast with hourly intervals
- 📅 **7-Day Forecast** - Extended forecast with daily highs/lows
- 🎨 **Dynamic Backgrounds** - Background changes based on weather conditions
- 📱 **Fully Responsive** - Works on desktop, tablet, and mobile devices
- 🎭 **Smooth Animations** - Beautiful transitions and hover effects
- 🌙 **Dark Mode Ready** - Modern gradient design

### 🎯 Displayed Information

**Current Weather:**
- Temperature (feels like)
- Weather description
- Humidity percentage
- Wind speed
- Atmospheric pressure
- Visibility distance
- Sunrise/Sunset times
- UV Index
- Dew Point

### 🚀 Getting Started

#### 1. Get API Key
1. Visit [OpenWeatherMap](https://openweathermap.org/api)
2. Sign up for a free account
3. Get your Free API key
4. Replace `API_KEY` in `weather-dashboard.js`

#### 2. Local Setup
```bash
# Clone or download the repository
cd weather-dashboard

# Open in your browser
open weather-dashboard.html
```

#### 3. Deploy on GitHub Pages
1. Push files to your GitHub repository
2. Go to repository Settings → Pages
3. Select `main` branch
4. Your site will be live at `https://yourusername.github.io/repo-name/weather-dashboard.html`

### 📂 File Structure

```
weather-dashboard/
├── weather-dashboard.html    # Main HTML file
├── weather-dashboard.css     # Styling and animations
├── weather-dashboard.js      # JavaScript logic and API calls
└── README.md                 # Documentation
```

### 🔧 API Endpoints Used

- **Geocoding API** - Convert city name to coordinates
- **Current Weather API** - Real-time weather data
- **Forecast API** - 5-day forecast with 3-hour intervals

### 🎨 Customization

#### Change Color Scheme
Edit CSS variables in `weather-dashboard.css`:
```css
:root {
    --primary-color: #667eea;
    --secondary-color: #764ba2;
    --accent-color: #f5576c;
    /* ... more variables ... */
}
```

#### Change Default City
Edit `weather-dashboard.js`:
```javascript
if (recentSearches.length === 0) {
    searchWeather('Your City'); // Change this
}
```

#### Update API Key
In `weather-dashboard.js`, line 5:
```javascript
const API_KEY = 'your_api_key_here';
```

### 📱 Features by Breakpoint

**Desktop (1024px+)**
- 3-column current weather layout
- 4-column hourly forecast grid
- Full sidebar with all details

**Tablet (768px - 1023px)**
- 2-column current weather
- Adjusted grid layouts
- Optimized spacing

**Mobile (< 768px)**
- Single column layout
- Simplified hourly forecast
- Touch-friendly buttons
- Optimized font sizes

### 🔐 Security Notes

- API key is exposed in frontend (acceptable for free tier with rate limits)
- For production, use a backend to hide API key
- Set up API key restrictions on OpenWeatherMap dashboard

### 🌐 Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile browsers (iOS Safari, Chrome Mobile)

### 📊 API Rate Limits

**Free Tier:**
- 1,000 calls/day
- 60 calls/minute

### 🚨 Error Handling

- City not found error messages
- Geolocation permission errors
- Network error handling
- Auto-hide error messages after 5 seconds

### 💾 Data Storage

- Recent searches stored in browser's `localStorage`
- Persists across browser sessions
- Maximum 10 recent searches

### 🎓 Learning Resources

- [OpenWeatherMap Documentation](https://openweathermap.org/api)
- [Geolocation API](https://developer.mozilla.org/en-US/docs/Web/API/Geolocation_API)
- [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
- [localStorage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage)

### 🐛 Troubleshooting

**Weather not loading?**
- Check API key is correct
- Verify internet connection
- Check browser console for errors
- Ensure API calls haven't exceeded rate limit

**Geolocation not working?**
- Allow location permission in browser
- Use HTTPS (required for geolocation)
- Check browser privacy settings

**Recent searches empty?**
- Clear browser storage and search again
- Check if localStorage is enabled

### 📝 Future Enhancements

- [ ] Weather alerts and warnings
- [ ] Air quality index (AQI)
- [ ] Pollen count
- [ ] Radar map integration
- [ ] Weather comparison between cities
- [ ] Historical weather data
- [ ] Export weather report as PDF
- [ ] Multiple language support
- [ ] Voice search
- [ ] Weather notifications

### 👤 Author

Created by Rashed | [GitHub](https://github.com/rrashedulislam691-dev)

### 📄 License

This project is open source and available under the MIT License.

### 🙏 Credits

- Weather data provided by [OpenWeatherMap](https://openweathermap.org/)
- Icons by [Font Awesome](https://fontawesome.com/)
- Fonts by [Google Fonts](https://fonts.google.com/)

### ✅ Checklist for Setup

- [ ] Get OpenWeatherMap API key
- [ ] Update API key in JavaScript file
- [ ] Test search functionality
- [ ] Test geolocation feature
- [ ] Check responsive design on mobile
- [ ] Verify all weather icons display correctly
- [ ] Test error handling
- [ ] Deploy to GitHub Pages (optional)

---

**Enjoy tracking your weather! 🌤️⛅🌦️**
