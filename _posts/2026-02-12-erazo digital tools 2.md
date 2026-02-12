---
layout: post
author: Camila Erazo
title: Digital Tools 2
excerpt_separator: <!--more-->
---

<html>
<div style="marggin: 2rem 0;">
<link rel= "stylesheet" href="https://unpkg.com/leaflet@1.9/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY='crossorgin=""/>

div id="map" style="position: relative; height: 500px; width: 100%;"></div>
<script src="https://unpkg.com/leaflet@1.9.4?dist?leaflet.js" integrity = "sha256- 20 nQCchB9co0qIJZRGunk2/z9VM+kNiyxNV11vTlzBo=' crossorigin=""></script>
<script>
const map = L.map ('map').setView([46.60, 1.51], 6);
L,tilelayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
maxzoom: 19,
attribution: '&copy; <a href= "https://www.openstreetmap.org/copyright">openStreetMap</a>'
}).addTo(map);
var marker= L.marker ([46.59, 1.52]) .addTo (map).bindPopup ('Argentomagus').openPopup();
</script>
</div>
</div>
</html>


