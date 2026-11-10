# Space City Dashboard 🌌🚀

Space City Dashboard is a sleek, responsive web application that fetches and displays live cosmic data directly from NASA's Astronomy Picture of the Day (APOD) infrastructure. The application features a custom dark space theme inspired by NASA and the Houston Astros.

## 🚀 Features
* **Modern Production Endpoint:** Directly integrated into NASA's active WordPress REST API (`science.nasa.gov/wp-json/wp/v2/apod-basic`) to bypass legacy server instabilities and deliver crisp, high-definition imagery (`hdurl`).
* **Keyless Public Fetching:** Architected to run cleanly in open-source repositories without requiring registration tokens or exposing secret API keys.
* **Interactive Mission Date Picker:** Allows space explorers to travel back in time by converting standard calendar dates (`YYYY-MM-DD`) into NASA's `YYMMDD` archive path format.
* **Smart Date Locking:** Automatically locks the calendar ceiling to today's mission date so users can't accidentally time-travel into the future. ⏳
* **Multi-Tier Telemetry & Fail-Safe Fallbacks:** Built with resilient CORS proxy routing (`corsproxy.io` and `codetabs.com`) and an automatic backup feed to the **NASA Image and Video Library API** (`images-api.nasa.gov`), ensuring Mission Control stays online even on restricted networks. 🛰️
* **Rich Media & Video Detection:** Dynamically renders high-resolution space photography or displays a direct Astros-orange launch link whenever NASA features an astronomy video. 🎬
* **Twinkling Star Background:** Custom layered CSS animations that simulate a moving, twinkling deep-space starfield. ✨
* **Houston-Inspired Visual Theme:** Features signature "Astros Orange" neon glow effects (`#F4911E`), "NASA Blue" backgrounds (`#0B3D91`), and live green/amber/red telemetry status indicators. ⚾🧡
* **Cinematic Proportional Layout:** Built with an expanded, wider display panel (`max-width: 1000px`) to showcase high-resolution astrophotography across desktop monitors while remaining fully responsive on mobile.

## 🛠️ Built With
* **HTML5:** Semantic markup for dashboard interface structure and native mission date controls.
* **CSS3:** Custom keyframe animations (`twinkle`, `pulse`), radial-gradient starfields, neon text/box shadows, and a mobile-friendly responsive layout.
* **JavaScript (ES6+):** Asynchronous telemetry requests using `async/await`, Fetch API multi-fallback routing, `YYMMDD` date string formatting, and safe HTML DOM injection.

## 🔧 Architecture & Migration History
The codebase was upgraded to keep pace with NASA's 2026 server migration and browser security standards:

* **Legacy Setup:** The project previously pulled data via the legacy bridge endpoint (`api.nasa.gov`) using a registered `api_key` parameter and standard `data.url` image fields.
* **Current Setup:** Ahead of the December 2026 legacy API retirement, the telemetry pipeline was re-engineered to target NASA's modern WordPress REST endpoint (`science.nasa.gov/wp-json/wp/v2/apod-basic`), extract direct `hdurl` image assets, format archive dates as `YYMMDD` path slugs, and route requests through CORS-safe fallbacks with a live NASA Image Library backup feed.

## 📝 Author
Created by **Zoe Canfield** | Space City Dashboard 🌠
