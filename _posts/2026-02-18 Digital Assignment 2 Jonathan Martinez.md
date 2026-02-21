---
layout: default
title: Interactive Map and Viewer
---

blah blah blah blah
<html>
<div style="margin: 2rem 0;">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
    var map = L.map('map').setView([42, 20], 6);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([40.3790045245, 19.7001398474]).addTo(map).bindPopup('Amantia').openPopup();
var marker = L.marker([39.7455951494, 20.0204278959]).addTo(map).bindPopup('Buthrotum').openPopup();
var marker = L.marker([39.60813, 19.906703]).addTo(map).bindPopup('Corcyra').openPopup();
var marker = L.marker([39.60813, 19.906703]).addTo(map).bindPopup('Nicopolis').openPopup();
var marker = L.marker([32.5, 37.5]).addTo(map).bindPopup('Phoenice').openPopup();
</script>
</div>
</html>
