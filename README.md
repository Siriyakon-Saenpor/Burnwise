# BurnWise

Satellite-based detection of crop burning vs. tillage in rice fields, with a plot-level priority matrix for targeting farmer subsidies.

GeoHackathon 2026 "Pixel to Policy" (GISTDA) — final 12 teams.

## What it does
1. Detects burn vs. no-burn signal in rice plots (Sentinel-2 dNBR, NDVI; thresholds calibrated with VIIRS hotspots)
2. Delineates field boundaries (Fields of The World)
3. Compares detections with GISTDA burned-area products (product agreement, not field validation)
4. Builds a Green / Yellow / Red priority matrix per plot (road access via OSMnx, tambon-level income)

Pilot area: Tha Tako, Nakhon Sawan (rice, main season).

## Data sources
- Sentinel-2 imagery (Google Earth Engine)
- VIIRS 375 m fire hotspots (NASA FIRMS)
- Fields of The World (field boundaries)
- Burned-area polygons (GISTDA)
- OpenStreetMap road network (OSMnx)
- Tambon-level household income: Basic Minimum Needs (จปฐ.) survey, Community Development Department, Ministry of Interior; data year B.E. 2568 (2025), last updated 26 Mar 2026 on the source site, accessed 30 Sep 2026.

## Limitations
- Burned and ploughed fields can look similar in imagery
- Socio-economic data is at tambon level, not plot level

## My contribution
Validated burn detection against GISTDA polygons; computed road access with OSMnx; prepared tambon income data; built the priority matrix; prepared slides and presented to mentors.

## Live demo
Dashboard: https://burnwise-dashboard-appbctyh2gj9ddbwadjall.streamlit.app/

## Team
Team "ทีมไม่เอาควัน" (BurnWise), GeoHackathon 2026
1. Rattanatham Saopha
2. Thanawat Boriboonthanaruk
3. Siriyakon Saenpor
4. Thanjira Wongsa
