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

## My project

Fill in (either in English, or in Slovak):

**Application description**: `I made four scenarios upon Bratislava map. The first make possible to show two streets with distinct colors(two seperate) layers on my map. The second scenario makes pg routing between one and second street. The third scenario makes available to make pg routing from street one to street second through street that is the closest to specific polygon building on a map. The fourth scenratio makes available to show some amount of polygons on a map, with points on those polygons, for example all shops Kaufland on a map in bratislava with specific distance meters from Fontain "Zem" before president palace. The fifth scenario is boosted heatmap of all shops in the city, that has the closest and the most of bus stops near by. That information is suitable for imobile people who on their own want to have as much as possible shop opportunities and do not have to travel on foot a lot. Moreover it can be used by MHD company to find out, what parts of central city are the worst supported with transports in order to build new bus stops.`

**Data source**: `<fill in>`

**Technologies used**: `<fill in>`
