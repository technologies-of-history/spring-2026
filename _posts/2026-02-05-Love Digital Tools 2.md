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
          "https://technologies-of-history.github.io/spring-2026-data/iiif/love.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "https://technologies-of-history.github.io/spring-2026-data/iiif/love.json", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html> 

## Historical Inscriptions in Roman Sardania
The inscription I chose comes from Turris Libisonis, a Roman town in Sardinia, modern day Porto Torres. The inscription features the names CN CORNELIVS and CLADIVS, which translates to Cn(aeus) Cornelius and Cladus I(sidi) v(otum) s(olvit), meaning Cornelius dedicated a statue to the Egyptian goddess Isis. At first I was surprised to find Egyptian religious influence in Sardinia, but when I researched further I found just how influential the goddess Isis was across the Rome. In Sardinia she was worshipped as a goddess of navigation and fertitlity, similar to more common Roman deities like Venus and Aphrodite. The letters on the inscription were relatively easy to make out since they are large, deeply carved, and all capitalized.

My map of surviving inscriptions from Sardinia shows that the "epigraphic habit" was primarily in towns around the island, such as Bosa, Turris Libisonis, and Carales. This shows that Romans in Sardinia used inscriptions primarily as a public way of recording religious dedications, honoring people, and keeping records in community spaces rather than private areas.

As MacMullen argues, the "epigraphic habit" rose and fell between shifts in Roman society and culture. I don't think digital tools take away from how historians interpret this at all. I believe they change how we engage with these inscriptions. High resolution imaging lets us examine details that would be hard to see in person, and digital mapping helps us visualize patterns across entire provinces. Together they give us a better and more accessible understanding of how Romans used writing in their everyday lives.
