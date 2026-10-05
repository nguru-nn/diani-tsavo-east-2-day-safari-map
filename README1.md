# Diani Beach → Tsavo East: 2-Day Safari Route Map

This is an interactive 3D map of a 2-day overnight safari from **Diani Beach** on Kenya's south coast to **Tsavo East National Park**, one of the largest national parks in Kenya and home of the famous red elephants. Guests stay overnight at **Voi Safari Lodge**, which overlooks a busy waterhole.

🗺️ **See the full itinerary and the live map:**
[Dwa dni zwiedzania – Park Narodowy Tsavo Wschodni](https://safarikenia.com.pl/dwa-dni-zwiedzania-park-narodowy-tsavo-wschodni) on **Safari Kenia**

---

## The route

| Day | Plan | Accommodation |
|-----|------|---------------|
| Start | Departure from Diani Beach | — |
| Day 1 | Game drive through Tsavo East | Voi Safari Lodge |
| Day 2 | Morning game drive and return to the coast | Diani Beach |

**Day 1:** Diani Beach → Likoni Ferry → Mariakani → Buchuma (Bachuma) Gate → game drive across Tsavo East → Voi Safari Lodge
**Day 2:** Voi Safari Lodge → game drive back through the park → Buchuma Gate → Mariakani → Likoni Ferry → Diani Beach

The interface labels are in Polish, matching the tour page it's embedded on.

## Features

- **The game drive is traced inside the park.** Waypoints inside Tsavo East keep the route on the park tracks between Buchuma Gate and Voi, on both the outbound day and the return day.
- **Satellite basemap with 3D terrain.** The map uses the Mapbox Standard Satellite style with DEM terrain at 1.5× exaggeration and a steeply tilted camera, which shows the red-earth plains of Tsavo.
- **Road-accurate route.** Each leg is fetched from the Mapbox Directions API (driving profile) and stitched into one line. If a request fails, the map falls back to a straight segment.
- **Animated route line.** A golden "marching ants" dashed line runs over a soft glow layer.
- **Interactive itinerary panel.** A glassmorphism sidebar lists each stage of the trip. Clicking a card flies the camera to that stop and opens its popup.
- **Custom markers.** Gold SVG pins mark the main stops. Hidden waypoints shape the route without cluttering the map.
- **Mobile-friendly.** On small screens the sidebar becomes a bottom sheet, and cooperative gestures keep page scrolling smooth.
- **WordPress-ready.** Styles are scoped to a single container, so the map can be pasted into a Custom HTML block.

## Tech stack

- [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) v3.9.0
- [Mapbox Directions API](https://docs.mapbox.com/api/navigation/directions/)
- Vanilla JavaScript, with no build step
- Plus Jakarta Sans (Google Fonts)

## Usage

1. Copy the HTML into a WordPress **Custom HTML** block or any web page.
2. Replace the Mapbox access token with your own, and restrict it to your domain in your [Mapbox account](https://account.mapbox.com/access-tokens/).
3. Adjust the container height in `.wp-safari-itinerary-container` to fit your layout.

To change the route, edit the `itineraryData` array. Entries with `isWaypoint: true` shape the route only. Every other entry gets a marker and a sidebar card.

## About

Built for [Safari Kenia](https://safarikenia.com.pl/), Polish-language safari tours and travel guides for Kenya.

➡️ [View this 2-day Tsavo East safari itinerary](https://safarikenia.com.pl/dwa-dni-zwiedzania-park-narodowy-tsavo-wschodni)
