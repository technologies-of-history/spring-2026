---
layout: post
author: Katie Tovar
title: Digital Assignment 2
excerpt_separator: <!--more-->
---


<html>
  <div style="margin: 2rem 0;">
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
    const map = L.map('map').setView([41.00, 27.28], 8);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([40.97, 27.50]).addTo(map).bindPopup('Bisanthe/Rhaedestus').openPopup();
var marker = L.marker([41.57, 27.765]).addTo(map).bindPopup('Bizye').openPopup();
var marker = L.marker([41.00, 28.96]).addTo(map).bindPopup('Constantinopolis').openPopup();
var marker = L.marker([42.38, 27.28]).addTo(map).bindPopup('Deultum').openPopup();
var marker = L.marker([40.97, 28.87]).addTo(map).bindPopup('Hebdomon').openPopup();
var marker = L.marker([40.97, 27.95]).addTo(map).bindPopup('Perinthus').openPopup();
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
          "https://technologies-of-history.github.io/spring-2026-data/iiif/tovar.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "https://technologies-of-history.github.io/spring-2026-data/iiif/tovar.json", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html>

