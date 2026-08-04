# Sentinel Web MVP — Real Map Edition

This version keeps the rebuilt Sentinel MVP design and features, while adding:

- a real interactive OpenStreetMap map through Leaflet;
- real Singapore place coordinates for all safety markers;
- route planning that is automatically drawn on the Trips map;
- a **Stop current route** control that removes the active route and its safety advice from both maps without deleting saved trip history;
- the latest planned route also appears on the main Safety Map;
- route-specific safety advice generated from nearby Sentinel sample locations, travel time and transport mode;
- route distance when the free OSRM demo routing service is available;
- a direct-line fallback if the routing service is temporarily unavailable.

## Run the application

### Windows
1. Extract the ZIP.
2. Double-click `start_server.bat`.
3. Open `http://localhost:8000` in a browser.

### macOS or Linux
1. Extract the ZIP.
2. Open a terminal in the folder.
3. Run `chmod +x start_server.sh && ./start_server.sh`.
4. Open `http://localhost:8000`.

## Internet requirement

The application itself and sample data are local. An internet connection is required to load the real OpenStreetMap tiles, the Leaflet map library and the optional OSRM road-route geometry. No API key is required.

If OSRM is unavailable, Sentinel still displays the route using a direct fallback line and generates safety advice locally.

## Important MVP note

Safety scores, community reports and advice are simulated sample data for demonstration and coursework. Sentinel does not replace official emergency services or professional travel advice.
