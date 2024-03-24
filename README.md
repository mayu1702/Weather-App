# Weather-App
This is a JavaScript application that creates a weather widget. It fetches weather information from the OpenWeatherMap API based on the user's selected city and displays it dynamically on the web page.

1. **Configuration:**
   - Defines a `config` object containing API endpoints and keys for the Country State City API (`cUrl` and `cKey`) and the OpenWeatherMap API (`wUrl` and `wKey`).

2. **Functions:**
   - `getCountries`: Fetches a list of countries, states, or cities based on the provided field name (e.g., "countries", "states", "cities").
   - `getWeather`: Fetches weather information for a specific city using the OpenWeatherMap API.
   - `getDateTime`: Converts a Unix timestamp to a human-readable date format.
   - `tempCard`: Generates HTML for displaying temperature information.
   - `displayWeather`: Updates the weather widget with the retrieved weather data.

3. **Event Listeners:**
   - `DOMContentLoaded`: Executes when the HTML document has been fully loaded. It populates the countries dropdown menu with options retrieved from the Country State City API.
   - `change` event listeners: Listen for changes in the selected country, state, and city dropdown menus. When a selection is made, it fetches weather information for the selected city and displays it.
   - `click` event listener: Listens for clicks on temperature unit links (`°C` and `°F`). When clicked, it updates the displayed temperature units and re-fetches weather information accordingly.

4. **HTML Elements and CSS Classes:**
   - The weather widget is constructed using HTML elements such as `<div>` and `<h5>`, and styled using CSS classes defined in an external stylesheet (not provided in the code snippet).

Overall, this application creates a dynamic weather widget that allows users to select a country, state, and city to view current weather information, and toggle between Celsius and Fahrenheit temperature units.
