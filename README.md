# Terrain360-Public-API v1.1
## About

Introducing the Terrain360 JSON API for third party map integration (Google Maps, ESRI/ARC GIS, Mapbox, Leaflet, etc). 
Benefits include leveraging over +10 million points of data across 1000's of trails and maps collected by Terrain360 and partners. 

Access is open to anyone upon request - To request an API Token and Account [Click Here](https://www.terrain360.com/about#contact)

# API Documentation
## Trail JSON with scenes 

Endpoint: https://terrain360.com/api/getTrail/{id}?api_token={token} <br/>
Returns all scenes & general trail data for specific trail. Trail ids can be found in admin panel. 

**Additional Trail options**
 <br/>
&basic  - Returns only basic trail information and url - no scene data
 <br/>
&embed - Returns embed url in place of general url
 <br/>
&embed_map=1 Adds map to embedded trails *&embed required
 <br/>
&embed_graph=1 Adds elevation graph to embedded trails *&embed required

## Map JSON 

Endpoint: https://terrain360.com/api/getMap/{id}?api_token={token} <br/>
 Default returns all trails assigned to map with ids and trail name, including general map information.
 Map ids can be located in admin panel. 
 <br/> <br/>
 **Additional Map options**
 <br/>
 &scenes - Returns all scenes for all trails 
 <br/>
 &embed -Returns all trail embed urls in place of general url
 <br/>
 &embed_map=1 Adds map to embedded trails  *&embed required
 <br/>
 &embed_graph=1 Adds elevation graph to embedded trails *&embed required

 


