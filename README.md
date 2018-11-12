# General course assignment

Build a map-based application, which lets the user see geo-based data on a map and filter/search through it in a meaningfull way. Specify the details and build it in your language of choice. The application should have 3 components:

1. Custom-styled background map, ideally built with [mapbox](http://mapbox.com). Hard-core mode: you can also serve the map tiles yourself using [mapnik](http://mapnik.org/) or similar tool.
2. Local server with [PostGIS](http://postgis.net/) and an API layer that exposes data in a [geojson format](http://geojson.org/).
3. The user-facing application (web, android, ios, your choice..) which calls the API and lets the user see and navigate in the map and shows the geodata. You can (and should) use existing components, such as the Mapbox SDK, or [Leaflet](http://leafletjs.com/).

## Example projects

- Showing nearby landmarks as colored circles, each type of landmark has different circle color and the more interesting the landmark is, the bigger the circle. Landmarks are sorted in a sidebar by distance to the user. It is possible to filter only certain landmark types (e.g., castles).

- Showing bicykle roads on a map. The roads are color-coded based on the road difficulty. The user can see various lists which help her choose an appropriate road, e.g. roads that cross a river, roads that are nearby lakes, roads that pass through multiple countries, etc.

## Data sources

- [Open Street Maps](https://www.openstreetmap.org/)

# My fiit-pdt-project - Bratislava
Project for subject PDT on FIIT, STU - Geo queries with Bratislava

## Detailed description

This project serves for example manipulation upon geo datasets of Bratislava city and consists of client and server side communication. Client dispose with .html file to control UI through browser where client can see his map, options and client input. Server side communicate with client and PSQL database server.

## Used technologies

In this project I used following technologies:
* Node.js
* JavaScript
* HTML
* CSS
* PSQL
* Socket.io
* Mapbox

## Client side

My client side consists of files for browser common with client-server communication. Most of work here involve processing user input and response from my server to show it on map.

Example of UI looks like follows:

![My UI picture](https://github.com/Marek-Bernad/fiit-pdt/assignment-gis/blob/master/images/ui.png)

## Server side

My server side is based on Node.js server with socket.io communication between user and this server. In this project server run client UI on localhost: http://localhost:8080/. 

![My server-side picture](https://github.com/Marek-Bernad/fiit-pdt-project/blob/master/images/server.png)

## Scenarios / what can it do?

Project allows user to use following scenarios:
* Show street A (map layer1)(Input: text field)
* Show street B (map layer2)(Input: text field)
* Show PgRouting betwwen A & B (map layer 3) (Input: 2x text field)
* Show PgRouting from A to C but needs to go through B (map layer 4)(input: 3x text field)
* Show polygon/polygons with edge points of specific objects like 'Billa', 'Kaufland' ... (map layer 5,6)(input: 1 text field)
* Show polygon/polygons with edge points with given distance from middle point of Bratislava (input: 1 text field)

## Datasets details

* openStreetMap of Bratislava (cut area)
* traffic in Bratislava

## How to run this project

1. Run your psql local server
2. Import databases
3. Update DB access in nodeServer.js file
4. Navigate to fodler with file "nodeServer.js"
5. Run in cmd/terminal "node nodeServer.js" (if you miss modules, install it in order of error code you obtain)
6. Navigate to http://localhost:8080/
 

## Versions / settings

* PgAdmin 4 - v3.2
* openstreetmap - updated version 2018, Oct.
* Mapbox GL JS - v0.50.0
* Node.js - v10.11.0
* Socket.io-client@2.1.1
* HTML,JS,CSS - up to date Oct, 2018
* PostgreSQL 10.5, compiled by Visual C++ build 1800, 64-bit
* Tested with windows10 Pro, 64-bit


