---
layout: default
title: Interactive Map and Viewer
---

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"/>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500">
<link rel="stylesheet" href="https://unpkg.com/mirador@latest/dist/mirador.min.css">

<div style="margin: 2rem 0;">
  <div id="map" style="height: 500px; width: 100%;"></div>
</div>

<div style="margin: 2rem 0;">
  <div id="my-mirador" style="height: 500px; width: 100%;"></div>
</div>

<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<script>
  var map = L.map('map').setView([41, 21], 5);

  L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; OpenStreetMap'
  }).addTo(map);

  L.marker([40.3790045245, 19.7001398474]).addTo(map).bindPopup('Amantia');
  L.marker([39.7455951494, 20.0204278959]).addTo(map).bindPopup('Buthrotum');
  L.marker([39.60813, 19.906703]).addTo(map).bindPopup('Corcyra');
  L.marker([39.0157, 20.7360035]).addTo(map).bindPopup('Nicopolis');
  L.marker([32.5, 37.5]).addTo(map).bindPopup('Phoenice');
</script>

<script src="https://unpkg.com/mirador@latest/dist/mirador.min.js"></script>

<script>
  const mirador = Mirador.viewer({
    id: "my-mirador",
    manifests: {
      "https://edh.ub.uni-heidelberg.de/iiif/edh/HD005856.manifest.json": {
        provider: "Epigraphic Database Heidelberg"
      }
    },
    windows: [
      {
        loadedManifest: "https://edh.ub.uni-heidelberg.de/iiif/edh/HD005856.manifest.json",
        canvasIndex: 0,
        thumbnailNavigationPosition: 'none'
      }
    ]
  });
</script>
