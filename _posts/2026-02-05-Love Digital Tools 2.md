---
layout: post
author: Kasia Love
title: Ancient Texts in Sardinia
excerpt_separator: <!--more-->
---


<html>
<div style="margin: 2rem 0;">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
    const map = L.map('map').setView([40.21, 9.02], 6);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
      maxZoom: 19,
      attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([40.29, 8.49]).addTo(map).bindPopup('Bosa').openPopup();
var marker = L.marker([39.21, 9.10]).addTo(map).bindPopup('Carales').openPopup();
var marker = L.marker([40.09, 8.50]).addTo(map).bindPopup('Cornus').openPopup();
var marker = L.marker([38.98, 9.015]).addTo(map).bindPopup('Nora').openPopup();
var marker = L.marker([40.92, 9.50]).addTo(map).bindPopup('Olbia').openPopup();
var marker = L.marker([39.16, 8.48]).addTo(map).bindPopup('Sulci').openPopup();
var marker = L.marker([40.83, 8.39]).addTo(map).bindPopup('Turris Libisonis').openPopup();  
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
          "https://edh.ub.uni-heidelberg.de/iiif/edh/HD025182.manifest.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "https://edh.ub.uni-heidelberg.de/iiif/edh/HD025182.manifest.json", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html> 
