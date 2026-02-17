---
layout: post
author: Jane Allinger 
title: Digital Tools Assignment Two
excerpt-separator: <!--more-->
---

The inscription I chose is an honorific inscription originally found In Cnossus Greece, which is now modern day Heraklion in Crete. This inscription is written in Latin by an unknown author. The inscription itself is in relatively good shape, except it looks like the top half of the monument could be missing. The translation of the inscription refers to a male by the name of Q. Refrio Thegenis f. Col. Theageni or Quintus Refrius Theagens. The inscription goes on to say that he is the son of Collina Theageni, whether this is an order, tribe, or person is not completely clear. It also mentions he is a member of local office of the decurial order. This is labeled as a honorific and not a epitaph or tombstone. 

<!--more-->

My map shows that Roman epigraphs were not limited to one specific town or village. But were spread along multiple miles of land. I narrowed my map down to only seven locations, but there was originally over forty inscriptions, and those are just the ones that had digital images. I think this shows that the Roman attitude towards stone inscriptions was positive. As they made it a point to create multiple public monuments that included this stone writing all over the region, even on a relatively small island like Crete. 

In MacMullen's Epigraphic Habit he mentions how stone epigraphs were culturally important to the Roman Empire. He specifically says "…the habit was an aspect of culture, not a practical necessity." (MacMullen 238) His reference to cultural significance highlights why we have so many well documented and surviving inscriptions. These writings were meant for communities. Thought, effort, and funds were required to create them and they were erected for all to see, not for just one person. This concept isn't hard to wrap your head around, but getting to have a visual representation helps people understand even better the importance of epigraphy in Roman society. The use of digital tools, imaging, and especially mapping, shows us just how vast a collection of stone inscriptions there are. Making it way easier for the general population to understand this was not a one off way of communicating, this was the way. Epigraphy was significant, extensive, and meaningful to the Roman people. Which is something I don't think you'd be able to fully grasp unless you had the backing digital tools provide. 


<html>
<div style="margin: 2rem 0;">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
  const map = L.map('map').setView([35.30, 25.16], 10);
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
          "https://technologies-of-history.github.io/spring-2026-data/iiif/allinger.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "https://technologies-of-history.github.io/spring-2026-data/iiif/allinger.json", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html>
