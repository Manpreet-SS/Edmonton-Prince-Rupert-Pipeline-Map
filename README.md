# Edmonton–Prince Rupert Pipeline — Interactive Route Map 🛢️

An interactive, self-contained web map visualising the **Edmonton–Prince Rupert crude oil pipeline** route — 1,715 km across Alberta and British Columbia, with 29 waypoints, pump stations, HDD crossings, Indigenous territory corridors, and a live elevation profile.

## How to Open

Simply open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge). No server or build step required — all dependencies are loaded from CDN.

```
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

Or serve it locally:

```
npx serve .              # Node.js
python3 -m http.server   # Python
```

## Features

| Feature | Details |
|---|---|
| **Interactive Map** | Leaflet.js + OpenStreetMap / OpenTopoMap base layers |
| **Pipeline Route** | Solid red polyline (standard sections) + orange dashed (micro-optimised zone, km 1185–1475) |
| **29 Waypoints** | Circle markers with popups showing name, km mark, elevation, and segment info |
| **15 Pump Stations** | Gold/yellow markers with popup details |
| **5 HDD Crossings** | Blue markers for critical horizontal directional drill crossings |
| **7 Indigenous Territory Zones** | Semi-transparent corridor polygons (Treaty 6, Treaty 8 AB, Treaty 8 BC/Carrier Sekani, Wet'suwet'en ⚠, Gitxsan ⚠, Kitselas/Kitsumkalum, Tsimshian) |
| **Elevation Profile** | HTML5 Canvas chart with all 29 waypoints + virtual Pine Pass peak (875 m), colour-coded by section |
| **Layer Controls** | Toggle overlays and switch base maps |
| **Info Panel** | Collapsible stats panel (capacity, cost, specifications) |
| **Legend** | All symbol and colour references |
| **Responsive** | Works on desktop and mobile |

## Route Statistics

- **Length:** 1,715 km
- **Capacity:** 900,000 bpd
- **Max Elevation:** 875 m (Pine Pass)
- **Pipe Spec:** 36" API 5L X70
- **Pump Stations:** 15
- **HDD Crossings:** 16 total (5 critical)
- **Block Valves:** 30
- **Estimated Cost:** ~$24.8B CAD
- **Indigenous Nations Crossed:** ~34

## Technology

- [Leaflet.js 1.9.4](https://leafletjs.com/) — interactive map library
- OpenStreetMap tiles — base map
- OpenTopoMap tiles — topographic base map option
- HTML5 Canvas — elevation profile chart
- No build tools, no frameworks, no dependencies beyond CDN links

