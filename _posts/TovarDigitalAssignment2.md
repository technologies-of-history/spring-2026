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
    const map = L.map('map').setView([(35.80590 25.56563, 42.29700 44.81766)], 6);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([40.978415, 27.508023]).addTo(map).bindPopup('Bisanthe / Rhaedestus').openPopup();
var marker = L.marker([41.572702, 27.765289]).addTo(map).bindPopup('Bizye').openPopup();
var marker = L.marker([41.0072009115, 28.9653901156]).addTo(map).bindPopup('Constantinopolis').openPopup();
var marker = L.marker([42.3886719103, 27.2808172535]).addTo(map).bindPopup('Deultum').openPopup();
var marker = L.marker([40.976033, 28.876487]).addTo(map).bindPopup('Hebdomon').openPopup();
var marker = L.marker([40.971013, 27.952973]).addTo(map).bindPopup('Perinthus').openPopup();
</script>
</div>
</html> 
