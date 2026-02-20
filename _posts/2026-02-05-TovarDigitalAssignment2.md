---
layout: post
author: Katie Tovar
title: Digital Assignment 2
excerpt_separator: <!--more-->
---
# Epigraphs and their effect on the Fall of Rome 
  My chosen inscription is a small part of a bigger stone epigraph. The top ¾ quarters of the a panel is having a warrior with a spear and a shield and on the bottom it has rectangle with very organized letters. It seems rather important since it is such a big statue. This epigraph was founded around Sea of Marmara where they primarily spoke Greek. Even though I do not understand Greek I am assuming what was written below was very important.
  <!--more--> 
  In looking at the inscriptions this is what letters I can make out or at least try to. (Any E could also be the gamma letter it was just really hard to tell the difference). At the Very top in Huge Letters there was a D with a L inside it and Huge M with on top of it. The Second Line is: APRILIS SPECTATVS M N M ELE. Third Line Reads: NVESE NENRIKECT KRATRIAPR. Fourth Line: ECTEROM DIVITESTVMVEXIEV (upside down). Fifth Line: NIS XXIEMDTV(upside down) SEV (lowercase) VISVV (upsidedown) EKVNC. The ancient find spot is Perinthus a town in the province Thracia which is present day Istanbul, Turkey. Perinthus was around from 330BC – 300 AD. 
  The other epigraphs seen within this province what I found interesting was the two different carvings that were commonly seen above the inscriptions. One was a carving of a warrior with the shield and the spear (the inscription I am focusing in this project) and the other carving is a person with a cape riding a horse with someone guiding the house from the back. In my inference, the two different carvings showed two different cities within the province of Thracia. It was cool to the difference in towns based on epigraphs to show what each city was reporting on at the time. It makes it easier for historians now to match an epigraph with a ancient city instead of having to guess.
  I think the high-res images can help historians understand what was deemed important by the government for civilians to know. It is physical history that is still around that even us to see today. The panels of the stone shows historians now that whatever was carved into the stone should be known by not just their generations but all generations after as well. Permanency is a status of power not all nations were able to offer it at that time. Permanency means that regardless of what is going on their nation at one moment, there is enough stability to last through it. These stone memorials were not easy to build nor were they small pieces that can easily be destroyed or moved. They are almost seen as a luxury to have them. In a failing nation, there are almost no resources that would be able to allow for such luxury as a huge stone statue of sorts because the nation would be on survival mode. When a nation is in frenzy there is no time for stone statues to be built and no good news to be shared. There is no security in the permanency when the future of the nation is being threatened. The decreases in these epigraphs can be an example in what was happening in the world and a good time frame in the Fall of Rome and help us understand different reasons behind the fall as well. 
---- 

<html>
  <div style="margin: 2rem 0;">
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
    const map = L.map('map').setView([41.00, 27.28], 8);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([40.97, 27.50]).addTo(map).bindPopup('Bisanthe/Rhaedestus').openPopup();
var marker = L.marker([41.57, 27.765]).addTo(map).bindPopup('Bizye').openPopup();
var marker = L.marker([41.00, 28.96]).addTo(map).bindPopup('Constantinopolis').openPopup();
var marker = L.marker([42.38, 27.28]).addTo(map).bindPopup('Deultum').openPopup();
var marker = L.marker([40.97, 28.87]).addTo(map).bindPopup('Hebdomon').openPopup();
var marker = L.marker([40.97, 27.95]).addTo(map).bindPopup('Perinthus').openPopup();
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
          "https://technologies-of-history.github.io/spring-2026-data/iiif/tovar.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "https://technologies-of-history.github.io/spring-2026-data/iiif/tovar.json", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html>



