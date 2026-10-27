# Space City Dashboard 🌌

Space City Dashboard is a sleek, responsive web application that fetches and displays live cosmic data directly from NASA's Astronomy Picture of the Day (APOD) infrastructure. The application features a custom dark space theme inspired by NASA and the Houston Astros.

## 🚀 Features
* **Modern Production Endpoint:** Directly integrated into NASA's active WordPress REST API to safely bypass backend framework instabilities.
* **Keyless Public Fetching:** Architected to run cleanly in open open-source repositories without requiring registration tokens or exposing secret configurations.
* **Interactive Mission Date Picker:** Allows users to travel back in time and view historical space photos dating back to June 1995.
* **Smart Date Locking:** Automatically restricts the calendar interface to prevent users from selecting future dates.
* **Twinkling Star Background:** Custom layered CSS animations that simulate a moving, twinkling starfield.
* **Themed Visual Assets:** Features custom "Astros Orange" glow effects (`#F4911E`) and "NASA Blue" backgrounds (`#0B3D91`).
* **Cinematic Proportional Layout:** Built with an expanded, wider display panel (`max-width: 1000px`) to properly showcase high-resolution space photography across desktop monitors while remaining fully responsive on mobile.
* **Fail-Safe Fallbacks:** Engineered with intelligent data property interceptors to block broken layout elements or default logo strings from disrupting UI render workflows.

## 🛠️ Built With
* **HTML5:** Semantic markup for dashboard interface structure.
* **CSS3:** Custom keyframe animations (twinkle, pulse), CSS radial gradients for dynamic star fields, and a mobile-friendly responsive grid layout.
* **JavaScript (ES6+):** Asynchronous web resource requests using `async/await`, native browser Fetch API configuration, structural object norming, and dynamic DOM injection.

## 🔧 Architecture & Migration History
The codebase was updated to adapt to NASA's server migration. 

* **Legacy Setup:** The project previously pulled data via the legacy bridge endpoint (`api.nasa.gov`) using a registered `api_key` query string parameter. 
* **Current Setup:** To future-proof the application ahead of the official legacy API archive deadline, the request pipeline was re-routed directly to the modern public endpoint (`science.nasa.gov/wp-json/wp/v2/apod-basic`). This modification completely eliminates the reliance on access tokens, fixes object property mismatches, and guarantees structural stability.

## 📝 Author
Created by **Zoe Canfield** | Space City Dashboard
