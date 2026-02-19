---
layout: post
author: Aiden Reed
title: Aiden Reed Digital Tools 2
excerpt_separator: <!--more-->
---

<html>
<div style="margin: 2rem 0;">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
    const map = L.map('map').setView([44.1686866150398, 27.952688949963544], 6);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([44.7230597111, 28.0618802039]).addTo(map).bindPopup('Cius').openPopup();
L.marker([44.5477874, 28.77512875]).addTo(map).bindPopup('Istrus').openPopup();
L.marker([43.22504, 27.585033]).addTo(map).bindPopup('Marcianopolis').openPopup();
L.marker([44.5, 26.5]).addTo(map).bindPopup('Novae').openPopup();
L.marker([43.2061605, 27.9134725]).addTo(map).bindPopup('Odessus').openPopup();
L.marker([43.710420238, 24.4661329357]).addTo(map).bindPopup('Oescus').openPopup();
L.marker([44.1728565, 28.6497375]).addTo(map).bindPopup('Tomi').openPopup();
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
          "https://technologies-of-history.github.io/spring-2026-data/iiif/reed.json": { provider: "Epigraphic Database Heidelberg" }
        },
        windows: [
          { loadedManifest: "https://technologies-of-history.github.io/spring-2026-data/iiif/reed.json", canvasIndex: 0, thumbnailNavigationPosition: 'none' }
        ]
      })();
</script>
</div>
</html>
<!--more-->

The inscription I chose was found in the ancient fortress of Novae, which is now Svishtov, Bulgaria and is predicted to be from around 151-250 AD. There is very little information about who wrote it and when it was found. We do know that this inscription is housed in a historical museum in Svishtov. The content of the inscription seems pretty easy to read. The database shows the words "Bono", "Event", and "Sacrum". We also see the words "Aur", which could refer to Marcus Aurelieus, a Roman emporeror and stoic philosopher, although aurelieus was a common Roman name and "Reg". When researching what Bono and Event meant together, I came across "Bonus Eventus", which was a Roman deity meaning "Good Outcome" or "Good Success". Knowing that the inscription was located in an ancient fortress, I predict that this was probably a transcription written possibly by soldiers dedicated to this deity, in hope of a good outcome of the battle.

Because the database has thousands of inscriptions and the map only includes a few, we know that the Romans heavily valued writing in stone. The wrote in fortresses cities, and along major roads. The Romans wanted their writing to be seen, not kept in secret. Showing off these inscriptions is kind of a brag to those who didn't know how to read or write. Writing showed power, strength, and wealth. Because the map has the possibility to include many more inscriptions than just the ones shown, we understand that writing was a practice that moved across the entire continent and not just used by the Romans. Writing was used by some other people, not just the higher ups. Predicting that thousands of soldiers learned to write, many others probably learned to over time.

Digital tools definitely help modern people understand these inscriptions. Although they may be a little damaged or worn out, HD imaging and digital availability lets people come together to help decode the inscriptions, understand them, and share them. Digital mapping, as I said earlier, shows how widespread the habit of writing became. The Romans embedded writing in their everyday environment. One negative effect of viewing the inscriptions digitally could be that we don't feel the same effect as actually seeing and reading the stone in person. It may be more a more special and meaningful experience to see/feel the stone rather than just looking at an online database. Overall, digital tools and mapping change how the public understand the presence of epigraphy in Roman society in more of a better way than a negative way.
