---
layout: default
title: Digital Tools Assignment 2 Jonathan Martinez
---
excerpt_separator: <!--more-->```
  For this assignment, I have chosen a inscription that was found in the province of Epirus in Buthrotum. The inscription is an epitaph (sort of words dedicated for someone who passed) which was predicted to have been "used" in 50 BC - 50 AD. Since it was found in the Roman Empire, the language it was found in was latin. It was written on a tabula (in this case on Marmor), wit its dimensions being 32 cm in height, 24 cm in width and with the letters being 2.1 cm. It was written for a "Caecilius Epagatus" a man. There are a couple letters that can be made it simply with just looking at it, for example some word "PAGAT"

  What the map I made of the surviving inscriptions that were found can actually help us identify the way that Roman people practiced epigraphs. For example, one of the locations, Buthrotum, seems to show an epigraph that happens to be in a sort of monuments, whilst the one that I have shown an image of below is simply just a piece of marble, by itself. This can show that that epigraph was found in a town.

  Finally referring to MacMullen's "epigraphic habit", do I think that that digital tools helped historians understand the rise and fall of the "epigraphic habit" in Roman society, I would say definitely. If we consider the way that historians tried to understand the rise and fall of epigraphic habit, they had to depend off of physical samples to be able to do research. With it being physical, which for example a epigraph, that menas that there would only be one copy, thus making it really difficult for multiple historians to do research at their own pace.

  With the addition of digital tools, all these issues pretty much just go away. With digital tools, historians can do research on inscriptions through images at their own pace. With digitil tools this also means that multiple historians can check on other historians research to compare or something else. Digital tools can also allow historians to see all types of inscriptions instead of waiting for a historian to finish researching its physical copy. Therefore, digital tools definitely helped historians understand the rise and fall of epigraphic habit.
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
          "https://technologies-of-history.github.io/spring-2026-data/iiif/martinez.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "https://technologies-of-history.github.io/spring-2026-data/iiif/martinez.json", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html>
