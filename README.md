# Space City Dashboard 🌌

Space City Dashboard is a sleek, responsive web application that fetches and displays live space data directly from NASA's Astronomy Picture of the Day (APOD) API. The application features a custom dark space theme inspired by NASA and the Houston Astros.

## 🚀 Features
* **Live NASA API Integration:** Automatically fetches the latest image, title, and descriptive explanation from NASA's official servers upon loading.
* **Interactive Mission Date Picker:** Allows users to travel back in time and view historical space photos dating back to June 1995.
* **Smart Date Locking:** Automatically restricts the calendar interface to prevent users from selecting future dates.
* **Twinkling Star Background:** Custom layered CSS animations that simulate a moving, twinkling starfield.
* **Themed Visual Assets:** Features custom "Astros Orange" glow effects (`#F4911E`) and "NASA Blue" backgrounds (`#0B3D91`).
* **Cinematic Proportional Layout:** Updated with an expanded, wider display panel (`max-width: 1000px`) to properly showcase high-resolution space photography across desktop monitors while remaining fully responsive on mobile.
* **System Status Indicators:** Includes a pulsing notification text that updates dynamically based on network connection health.

## 🛠️ Built With
* **HTML5:** Semantic markup for application structure.
* **CSS3:** Custom keyframe animations (twinkle, pulse), CSS radial gradients for stars, and a mobile-friendly responsive layout.
* **JavaScript (ES6+):** Asynchronous network requests using `async/await`, Fetch API integration, and dynamic DOM manipulation.

## 🔧 Setup Instructions
To run this dashboard locally or complete your hosting setup, you will need an API key from NASA.

1. Visit [api.nasa.gov](https://nasa.gov) and sign up for a free developer API key.
2. Open your `index.html` file.
3. Locate the JavaScript section at the bottom of the file.
4. Replace the placeholder value with your live secret token:
   ```javascript
   const myApiKey = "YOUR_NASA_API_KEY_HERE";
   ```
5. Save the file and open it in any modern web browser.

## 📝 Author
Created by **Zoe Canfield** | Space City Dashboard
