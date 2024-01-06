# Terrain360-Public-API v2.1

## About
Introducing the Terrain360 JSON API for third-party map integration (Google Maps, ESRI/ARC GIS, Mapbox, Leaflet, etc). Benefits include leveraging over 10 million points of data across thousands of trails and maps collected by Terrain360 and partners. 

Access is open to anyone upon request - To request an API Token and Account [Click Here](https://www.terrain360.com/contact)

## API Documentation

### Trail JSON with scenes

**Endpoint:** `https://terrain360.com/api/getTrail/{id}?api_token={token}`  
Returns all scenes & general trail data for a specific trail. Trail IDs can be found in the admin panel.

#### Additional Trail options
- `&basic` - Returns only basic trail information and URL - no scene data
- `&embed` - Returns embed URL in place of general URL
- `&embed_map=1` - Adds map to embedded trails (*&embed required)
- `&embed_graph=1` - Adds elevation graph to embedded trails (*&embed required)

### Map JSON

**Endpoint:** `https://terrain360.com/api/getMap/{id}?api_token={token}`  
By default, it returns all trails assigned to a map with IDs and trail names, including general map information. Map IDs can be located in the admin panel.

#### Additional Map options
- `&scenes` - Returns all scenes for all trails (used to build tracks in mapping platforms, includes thumbnail image for each scene)
- `&embed` - Returns all trail embed URLs in place of the general URL
- `&embed_map=1` - Adds map to embedded trails (*&embed required)
- `&embed_graph=1` - Adds elevation graph to embedded trails (*&embed required)

### Get Scene Options for ML/AI

**Endpoint:** `https://terrain360.com/api/getScene/{id}/{scene_id}?api_token={token}`
