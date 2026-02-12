---
layout: post
author: David Smith
title: Smithdocument
excerpt_separator: <!--more-->
---

This is a test of the scripts.

<html>
<div style="margin: 2rem 0;">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
    const map = L.map('map').setView([35.00744350691586, 33.17782134001847], 6);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([34.6654290132, 32.8858604166]).addTo(map).bindPopup('Kourion').openPopup();
L.marker([34.757212, 32.406593]).addTo(map).bindPopup('Nea Paphos').openPopup();
L.marker([34.7053255, 32.579086]).addTo(map).bindPopup('Paphos').openPopup();
L.marker([35.179581302, 33.9028569668]).addTo(map).bindPopup('Salamis').openPopup();
L.marker([35.138224, 32.813067]).addTo(map).bindPopup('Soli, bei').openPopup();
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
          "https://technologies-of-history.github.io/spring-2026-data/iiif/smith.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "https://technologies-of-history.github.io/spring-2026-data/iiif/smith.json", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html>
