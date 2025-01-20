# Route Finder

This is a web application built with Streamlit that helps users find routes between two locations using the OpenRouteService API. It allows users to select travel modes (Car, Walk, Bike) and provides a dynamic map with directions, along with the ability to download the route as an HTML file.

## Features
- **Geocoding:** Converts city names or addresses into geographic coordinates using OpenRouteService.
- **Route Calculation:** Computes the route between the origin and destination for various travel modes.
- **Interactive Map:** Displays the route dynamically using Folium maps.
- **Downloadable Routes:** Allows users to download the route directions as an HTML file.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-repo-name>/route_finder.git
   cd route_finder
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Add your OpenRouteService API key:
   - Create a `.streamlit/secrets.toml` file in the project directory:
     ```
     [general]
     ORS_API_KEY = "your_openrouteservice_api_key"
     ```
4. Run the app:
   ```bash
   streamlit run app.py
   ```

## Usage
1. Enter the origin and destination locations in the text boxes (e.g., "San Francisco, CA").
2. Choose the travel mode: Car, Walk, or Bike.
3. Click the **Get Directions** button to calculate and display the route on the map.
4. Optionally, download the route as an HTML file.

## Dependencies
The app requires the following Python libraries:
- `streamlit`
- `folium`
- `streamlit-folium`
- `requests`

All dependencies are listed in the `requirements.txt` file.

## Credits
This app is based on the course material from the **Mapping and Data Visualization with Python (Full Course)** by [Ujaval Gandhi](https://spatialthoughts.com), © 2022 Spatial Thoughts. Special thanks to Ujaval Gandhi for providing the foundational scripts and knowledge.

## License
This project is licensed under the MIT License.
