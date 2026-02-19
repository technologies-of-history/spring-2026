---
layout: post
title: "Digital Tools Assignment 2: Arabia Maps and Mirador Viewer"
author: Fiona Corrigan
---
## Arabia Inscriptions Leaflet Map

<html>
<div style="margin: 2rem 0;">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
    const map = L.map('map').setView([32.2, 36.2], 7);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([32.5204513362, 36.4813007519]).addTo(map).bindPopup('Bostra').openPopup();
var marker = L.marker([32.754205, 36.6183555]).addTo(map).bindPopup('Canatha').openPopup(); 
var marker = L.marker([33.511612, 36.309102]).addTo(map).bindPopup('Damascus').openPopup(); 
var marker = L.marker([32.280087, 35.891091]).addTo(map).bindPopup('Gerasa').openPopup();
var marker = L.marker([31.717339, 35.794519]).addTo(map).bindPopup('Medaba').openPopup();
var marker = L.marker([31.767959, 35.725677]).addTo(map).bindPopup('Nebo').openPopup();
var marker = L.marker([31.767959, 35.725677]).addTo(map).bindPopup('Nebo, bei').openPopup();
var marker = L.marker([30.328611, 35.441944]).addTo(map).bindPopup('Petra').openPopup();
var marker = L.marker([31.954951, 35.934624]).addTo(map).bindPopup('Philadelphia').openPopup();
var marker = L.marker([32.853765, 36.627525]).addTo(map).bindPopup('Philippopolis').openPopup();
</script>
</div>
</html>


<html>
<div style="margin: 2rem 0;">
  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500">
  <link rel="stylesheet" href="https://unpkg.com/mirador@latest/dist/mirador.min.css">
  
  <div id="my-mirador" style="position: relative; height: 500px; width: 100%;"></div>
  
  <script src="https://unpkg.com/mirador@latest/dist/mirador.min.js"></script>
    <script>
      const mirador = Mirador.viewer({
        id: "my-mirador",
        manifests: {
        "https://technologies-of-history.github.io/spring-2026-data-iiif/corrigan1.json":
          "https://technologies-of-history.github.io/spring-2026-data-iiif/corrigan1.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "[URLforyourmanifest.json](https://edh.ub.uni-heidelberg.de/iiif/edh/F002340.manifest.json)", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html
