---
layout: post
author: Jane Allinger 
title: First Post
excerpt-separator: <!--more-->
---

<html>
<div style="margin: 2rem 0;">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
    const map = L.map('map').setView([35.30, 25.16], 6);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([35.30, 25.16]).addTo(map).bindPopup('Cnossus').openPopup();
var marker = L.marker([35.06, 24.95]).addTo(map).bindPopup('Gortyn').openPopup();
var marker = L.marker([35.01, 25.74]).addTo(map).bindPopup('Hierapytna').openPopup();
var marker = L.marker([35.19, 25.72]).addTo(map).bindPopup('Lato').openPopup();
var marker = L.marker([35.21, 25.37]).addTo(map).bindPopup('Lyttos').openPopup();
var marker = L.marker([35.08, 25.20]).addTo(map).bindPopup('Pyrathos').openPopup();
var marker = L.marker([35.01, 24.95]).addTo(map).bindPopup('Rhizenia').openPopup();  
</script>
</div>
</html>
