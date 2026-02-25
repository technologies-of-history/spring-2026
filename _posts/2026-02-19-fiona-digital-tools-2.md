---
layout: post
title: Digital Tools Assignment 2: Arabia Maps and Mirador Viewer
author: Fiona Corrigan
excerpt_separator: <!--more-->
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
        "https://technologies-of-history.github.io/spring-2026-data/iiif/corrigan1.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "https://technologies-of-history.github.io/spring-2026-data/iiif/corrigan1.json", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html

<!--more-->

## Written Analysis 

My chosen inscription was found in the Roman Province of Arabia, in what is now modern-day Jordan. The original date of my inscription is unknown, and at first glance, I was able to recognize many individual Greek letters, although I could not immediately understand the full message. After further research, this inscription uses Koine Greek, suggesting it was made during the Roman imperial period when Greek was a widely used language in the eastern provinces, just like where my inscription was found. After translating my inscription, it reads as a commemoration of someone’s death, saying “Prokopas, son of Mnon, (and) Anastasius Karpo-geron Philagon, and Statina his mother, (set this up) in memory.” This shows that the stone was put up as a memorial to remember and honor the deceased. The stone is carefully carved and durable, which mirrors the Roman practice of creating long-lasting memorials. 

While examining the map of inscriptions from the Arabian province, it is clear that these inscriptions are mostly found in towns, cities, and along major routes rather than being evenly distributed across the region. A lot of these inscriptions were found near settlements and important infrastructure, likely because they may be connected to areas where Roman administration was active. It is very likely that these memorial monuments would be found in hubs of activity for the people in these civilizations. 

Digital tools like high-res imaging and digital mapping are incredibly impactful in terms of how historians interpret the rise and fall of the “epigraphic habit” in Roman society. The inscriptions served not only as records for practical purposes but also demonstrate how these Romans saw themselves and their place in society. MacMullen argues that inscriptions were “a specially useful window through which we may examine that world,” because of how they reveal what and who people chose to memorialize. High-res imaging allows historians to look closer at these habits. They’re able to see inscriptions that have been damaged or worn up closer, making it simpler to identify letters and produce more accurate translations. Digital mapping allows historians to think in terms of geography and analyze how different inscriptions were distributed across a region, allowing them to identify patterns in where they are found and why they are created. It also helps to better understand cultural diffusion across a province. Digital tools strengthen our ability to understand the rise and decline of the epigraphic habit by making inscriptions more accessible, visible, and analyzable than ever before.
