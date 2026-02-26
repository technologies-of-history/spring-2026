---
layout: post
author: Vivian Velazquez
title: Mapping the Epigraphic Habit in Roman Numidia
excerpt_separator: <!--more-->
---

# Stone, Space, and the Epigraphic Habit in Roman North Africa

Roman inscriptions were not just texts; they were public technologies. Cut into stone and placed in shared spaces, inscriptions shaped how memory, authority, and identity were communicated across the empire. The “epigraphic habit,” as Ramsay MacMullen describes it, was a cultural pattern in which ordinary social and political life increasingly became something written down, displayed, and preserved in durable form. In this post, I look at inscriptions from Roman North Africa (modern Algeria) to consider what mapping and high-resolution imaging can reveal about where inscriptions survive, how they worked as communication, and what digital tools add to historical interpretation.

<!--more-->

## A Single Inscription as Public Communication

The inscription I selected from the Epigraphic Database Heidelberg (EDH Foto F000065) comes from Roman North Africa and is dated to the imperial period, a time when epigraphic production in the region was particularly dense. Like many inscriptions from this area, it reflects a culture in which public commemoration and civic identity were expressed materially in stone. Even without fully reconstructing every line, the monument’s visual grammar communicates meaning: carefully carved capital letters, an ordered layout, and the permanence of stone all signal that the text was meant to be seen and trusted. This is what makes inscriptions such a distinctive form of communication technology. Unlike a letter or a private document, epigraphy assumes an audience; it asks to be read in public, to fix a memory, and to ensure authority is visible.

Using Mirador to view the inscription through the course IIIF manifest makes this publicness easier to appreciate. Zoomable imaging changes what “reading” an inscription looks like: rather than relying only on transcription, the historian can pay attention to letter forms, spacing, damage, and carving depth. The image becomes not just an illustration, but evidence. The ability to examine details at high resolution highlights the material side of epigraphy: how writing is produced, not only what it says.

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
    "https://technologies-of-history.github.io/spring-2026-data/iiif/velazquez.json": {
      provider: "Epigraphic Database Heidelberg"
    }
  },
  windows: [
    {
      loadedManifest: "https://technologies-of-history.github.io/spring-2026-data/iiif/velazquez.json",
      canvasIndex: 0,
      thumbnailNavigationPosition: 'none'
    }
  ]
});
</script>
</div>
</html>

## Spatial Patterns of Epigraphic Survival

To understand the broader pattern beyond a single monument, I mapped inscription findspots from Algeria/Numidia using Leaflet. The resulting distribution is not random. Inscriptions cluster around major towns and Romanized urban centers, such as Thamugadi (Timgad), Lambaesis, and Cirta, rather than spreading evenly across the landscape. This pattern supports MacMullen’s argument that the epigraphic habit is tied to social structures: inscriptions appear where institutions, civic life, and public audiences are concentrated. Where there are forums, roads, military bases, and administrative networks, we also find more stone texts.

The map also suggests that epigraphy was deeply connected to infrastructure and movement. These were spaces where people gathered, traveled, served, traded, and governed—meaning inscriptions functioned alongside architecture as part of the empire’s public messaging system. In other words, the “habit” was not just a taste for writing; it was embedded in a built environment that made inscription-reading a normal part of life.

<html>
<div style="margin: 2rem 0;">
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"/>

<div id="map" style="position: relative; height: 500px; width: 100%;"></div>

<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
<script>

const map = L.map('map').setView([35.8, 6.8], 7);

L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
maxZoom: 19,
attribution: '&copy; OpenStreetMap'
}).addTo(map);

L.marker([35.45026, 7.949211]).addTo(map).bindPopup("Aquae Caesaris");
L.marker([36.4623320806, 6.48238089616]).addTo(map).bindPopup("Castellum Tidditanorum");
L.marker([36.3681146667, 6.61330266667]).addTo(map).bindPopup("Cirta");
L.marker([36.321014003, 5.73538618658]).addTo(map).bindPopup("Cuicul");
L.marker([35.7798225608, 6.07746431754]).addTo(map).bindPopup("Diana Veteranorum");
L.marker([35.435644, 7.148368]).addTo(map).bindPopup("Mascula / Khenchela");
L.marker([35.489664231, 6.25484105102]).addTo(map).bindPopup("Lambaesis");
L.marker([35.796796, 7.3928]).addTo(map).bindPopup("Marcimeni");
L.marker([35.44507275, 6.51820125]).addTo(map).bindPopup("Thamugadi (Timgad)");
L.marker([35.404174, 8.1223145]).addTo(map).bindPopup("Theveste");
L.marker([36.382567, 7.250033]).addTo(map).bindPopup("Thibilis");
L.marker([35.4887175, 6.2897085]).addTo(map).bindPopup("Verecunda");
L.marker([36.137412, 7.080887]).addTo(map).bindPopup("Vicus Phosphorus");
L.marker([35.802187, 5.677421]).addTo(map).bindPopup("Zarai");

</script>
</div>
</html>

## Digital Tools as Historical Methods

MacMullen’s argument focuses on the rise, intensity, and decline: why epigraphy becomes so common in the Roman world and what that saturation tells us about society. Digital tools do not replace that interpretive work, but they sharpen it. Mapping makes the scale of epigraphic survival visible and helps identify patterns that a list of results can hide, especially clustering, regional density, and the relationship between inscriptions and civic centers. Meanwhile, IIIF-based viewing restores the inscription as a material object rather than a detached text, further inviting attention to craft, legibility, and physical context.

Together, Leaflet and Mirador make a basic point clearer: the epigraphic habit was not only writing, but a system of public communication that depended on place, audience, and material durability. Seeing inscriptions in both space (the map) and material detail (the IIIF) changes what historians can ask.

