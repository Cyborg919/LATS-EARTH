# LATS Earth — GitHub Pages Ready

LATS Earth is a static HTML/JavaScript prototype for location-aware weather, public environmental-station observations, local weather/news resources, and the LATS landslide-risk demonstration.

## Included

- Interactive 3D Earth/globe view
- Place search for cities, districts, villages, localities and neighbourhoods
- Current weather and forecast
- Public environmental station lookup through openSenseMap when available
- Open-Meteo weather/model fallback, clearly separated from physical observations
- Location-specific weather/news resources and official emergency links
- Street View / directions links for selected locations
- LATS prototype risk indicators
- Physical LATS ESP32 station section kept separate from public stations

## No API keys required

The browser app uses public endpoints and does not contain private API keys or passwords.

### Main data sources

- openSenseMap — public environmental station observations
- Open-Meteo — weather/model data
- OpenStreetMap Nominatim — place search/geocoding
- ArcGIS World Imagery / reference tiles — map imagery
- MapLibre GL JS / Leaflet — map rendering
- GDELT and official weather/news links where available

Public-station availability varies by location and time. The application must not label a public station as an LATS-owned station.

## Publish with GitHub Pages

1. Create a GitHub repository.
2. Upload **all files in this folder**, keeping `index.html` at the repository root.
3. Open **Settings → Pages**.
4. Choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`.
6. Save and wait for the Pages deployment.

The resulting project site will normally be:

`https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`

## Important testing note

Use the published HTTPS GitHub Pages URL when testing live APIs. Opening the HTML directly as `file://` can cause browser cross-origin restrictions and can make external APIs appear unavailable.

## Physical ESP32 station

The physical station is intentionally not simulated. It should remain OFFLINE until real ESP32 hardware, a calibrated rain gauge and a soil-moisture sensor are connected to a real backend or public station service.

## Prototype limitation

The LATS risk score is a prototype decision-support indicator based on available weather/sensor inputs. It is not a validated landslide probability, certified warning system, or replacement for official disaster warnings.

## Creator

Created by Vignesh P — Instagram: https://www.instagram.com/vignesh_pgd/
