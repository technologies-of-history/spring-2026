---
layout: post
author: Aiden Reed
title: Aiden Reed Digital Tools 2
excerpt_separator: <!--more-->
---

<html>
<div style="margin: 2rem 0;">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
    const map = L.map('map').setView([44.1686866150398, 27.952688949963544], 6);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([44.7230597111, 28.0618802039]).addTo(map).bindPopup('Cius').openPopup();
L.marker([44.5477874, 28.77512875]).addTo(map).bindPopup('Istrus').openPopup();
L.marker([43.22504, 27.585033]).addTo(map).bindPopup('Marcianopolis').openPopup();
L.marker([44.5, 26.5]).addTo(map).bindPopup('Novae').openPopup();
L.marker([43.2061605, 27.9134725]).addTo(map).bindPopup('Odessus').openPopup();
L.marker([43.710420238, 24.4661329357]).addTo(map).bindPopup('Oescus').openPopup();
L.marker([44.1728565, 28.6497375]).addTo(map).bindPopup('Tomi').openPopup();
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
          "https://technologies-of-history.github.io/spring-2026-data/iiif/reed.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "https://technologies-of-history.github.io/spring-2026-data/iiif/reed.json", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html>
