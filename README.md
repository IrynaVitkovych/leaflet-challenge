## leaflet-challenge
# Module 15 

This code fetches earthquake data from the USGS (United States Geological Survey) -  USGS GeoJSON Feed  and displays it on a Leaflet map. It visualizes earthquakes that occurred within the past week.

# Instructions:
Clone the repository to your local machine.
Open the index.html file in a web browser.

# Code Overview:
The GeoJSON earthquake data is fetched from the USGS API.
A Leaflet map is created and centered at latitude 37.8 and longitude -96, with a zoom level of 7.
A tile layer from OpenStreetMap is added to the map to provide a base layer.
Each earthquake feature from the GeoJSON data is represented as a circle marker on the map.
The size and color of the circle markers indicate the magnitude and depth of the earthquakes, respectively.
Pop-up information is displayed when a circle marker is clicked, showing the magnitude, location, and depth of the earthquake.
A legend is added to the bottom-right corner of the map to correlate colors with earthquake depths.

# Libraries and APIs Used:
Leaflet: A JavaScript library for interactive maps.
D3.js: A JavaScript library for data visualization.
USGS API: Provides earthquake data in GeoJSON format.

# Files:
index.html: HTML file containing the map and script references.
(In order to make visualization work, I changed the position of lines inside index.html from what was given to this 
  <!-- Leaflet CSS -->
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
    integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY="
    crossorigin="" />

    <!-- Leaflet JS -->
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
  integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
  crossorigin=""></script>

  <!-- Our CSS -->
  <link rel="stylesheet" type="text/css" href="static/css/style.css">
  )




static/css/style.css: CSS file for custom styling.
(Also I add some lines to this file to be able vizualise legend on the bottom right corner
.legend {
  line-height: 25px;
  color: #555;
}
.legend i {
  width: 18px;
  height: 18px;
  margin-right: 8px;
  opacity: 0.7;
  display: inline-block;
  clear: both;
}

.info {
  padding: 6px 8px;
  font: 14px/16px Arial, Helvetica, sans-serif;
  background: white;
  background: rgba(255,255,255,0.8);
  box-shadow: 0 0 15px rgba(0,0,0,0.2);
  border-radius: 5px;
  
}
.info h4 {
  margin: 0 0 5px;
  color: #777;
})

static/js/logic.js: JavaScript file containing the code to fetch earthquake data and display it on the map.

# Dependencies:
Leaflet: leaflet.css and leaflet.js are included via CDN (Content Delivery Network) links.
D3.js: d3.v7.min.js is included via a CDN link.

# Notes:
Ensure an internet connection to fetch earthquake data from the USGS API.
Customize the CSS in style.css for any additional styling changes.
Update the Leaflet and D3.js versions if needed, by modifying the CDN links in index.html.
Consider hosting the application on a web server for better performance and stability.

