# Martian Map — Genesiss 2026

An interactive Mars exploration and route-planning model created for the NASA Space Apps Challenge 2026 challenge **Interplanetary Survival Guide: Martian Map**.

**Live site:** [genesiss-2026-martian-map.netlify.app](https://genesiss-2026-martian-map.netlify.app/)

## What it does

Martian Map brings terrain, reference imagery, candidate locations, hazards, and route planning into one interactive view. Visitors can inspect a point on Mars, review its elevation and nearby features, choose a route start and goal, and compare estimated distance, elevation gain, travel time, and risk.

The model includes:

- Globe, orthographic, flat 2D, terrain 3D, isometric, dimetric, trimetric, parallax, and polar views.
- Map layers for elevation, solar energy, water-ice estimates, fuel-stop range, sites, hazards, rover routes, day and night, and the subsolar point.
- Mission and landing-site markers, hazard zones, and fuel stops.
- Route planning for astronauts on foot, pressurised rovers, and robotic rovers, with a traverse simulation.
- Mars time and season controls, plus Phobos and Deimos orbit visualizations.

## NASA data and resources

- [MGS MOLA MEGDR topography](https://pds-geosciences.wustl.edu/missions/mgs/megdr.html) — the embedded elevation grid informs terrain relief and the model’s elevation, slope, and roughness inputs. The app also links to the [MEGDR product label](https://pds-geosciences.wustl.edu/mgs/urn-nasa-pds-mgs_mola_topography_derived/meg004/megt90n000cb.xml).
- [NASA Mars Trek](https://trek.nasa.gov/mars/) — live Viking MDIM 2.1 imagery and MOLA shaded-relief map tiles. See the [Mars Trek tile API documentation](https://trek.nasa.gov/tiles/apidoc/trekAPI.html?body=mars).
- [NASA GISS Mars24](https://www.giss.nasa.gov/tools/mars24/) — reference for Mars time, seasons, and the Sun’s position.
- Additional references: [NASA Mars](https://science.nasa.gov/mars/), [Mars Fact Sheet](https://nssdc.gsfc.nasa.gov/planetary/factsheet/marsfact.html), [HiRISE](https://www.uahirise.org/), and the [Planetary Data System](https://pds.nasa.gov/).

## What is estimated

Water ice, solar energy, dust exposure, temperature, pressure, communications, and the fuel network are application estimates. Viking and MOLA imagery provide visual context; imagery is not used as measured resource data. Site scores and route risk are for exploration and learning. They are not official NASA recommendations, mission certifications, or guarantees of landing safety or human survivability.

## How to use it

1. Open the live site and rotate the map by dragging. Zoom with the wheel, pinch gestures, or the **+ / −** controls.
2. Select a location to see its coordinates, elevation, and nearby site information.
3. Set a start and goal on the map or in the Route Planner, select a travel mode, and review the route analysis. Choose **Simulate traverse** to view the route animation.
4. Open **Layers** to change the map background and overlays. Use **Sites**, **Hazards**, **Sun & seasons**, and **Moons of Mars** to explore other views and controls.
5. Use **Help** in the app for the full control guide.

## Technology and running locally

The main model is a single HTML page with inline CSS and JavaScript. Three.js r128 is loaded from [cdnjs](https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js); the app has no separate build step. To run it locally, open the HTML file in a modern browser with internet access. Internet access is needed for the Three.js CDN and live Mars Trek map tiles. See the [Three.js license](https://github.com/mrdoob/three.js/blob/r128/LICENSE).

## Project links

- **Main interactive model:** [genesiss-2026-martian-map.netlify.app](https://genesiss-2026-martian-map.netlify.app/)
- **Presentation:** [genesiss-2026-presentation.netlify.app](https://genesiss-2026-presentation.netlify.app/)
- **NASA Space Apps Challenge:** [Interplanetary Survival Guide: Martian Map](https://www.spaceappschallenge.org/2026/challenges/interplanetary-survival-guide-martian-map/?tab=details)
