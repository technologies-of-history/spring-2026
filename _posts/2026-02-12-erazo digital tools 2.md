---
layout: post
author: Camila Erazo
title: Digital Tools 2
excerpt_separator: <!--more-->
---

<html>
<div style="margin: 2rem 0;">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>

  <div id="map" style="position: relative; height: 500px; width: 100%;"></div>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
    <script>
    const map = L.map('map').setView([47.77, 14.85], 6);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);
var marker = L.marker([32.52, 36.48]).addTo(map).bindPopup('bostra').openPopup();
var marker = L.marker([32.75, 36.61]).addTo(map).bindPopup('canatha').openPopup();
var marker = L.marker([33.51, 36.28]).addTo(map).bindPopup('damascus').openPopup();
var marker = L.marker([30.31, 35.47]).addTo(map).bindPopup('petra').openPopup();
var marker = L.marker([31.81, 35.96]).addTo(map).bindPopup('philadelphia').openPopup();
var marker = L.marker([32.85, 36.63]).addTo(map).bindPopup('philippopolis').openPopup();
var marker = L.marker([33.43, 35.73]).addTo(map).bindPopup('kfeir abu sarbut').openPopup();
var marker = L.marker([35.00, 38.76]).addTo(map).bindPopup('ll haiyât').openPopup();
var marker = L.marker([36.33, 36.85]).addTo(map).bindPopup('qal at sim an').openPopup();
var marker = L.marker([32.63, 36.09]).addTo(map).bindPopup('hauran').openPopup();
var marker = L.marker([32.73, 36.06]).addTo(map).bindPopup('tafas').openPopup();
var marker = L.marker([31.88, 36.82]).addTo(map).bindPopup('qasr al-azraq').openPopup();
</script>
</div>
</html>
{
  "@context": "http://iiif.io/api/presentation/2/context.json",
  "@id": "https://edh.ub.uni-heidelberg.de/iiif/edh/F002818.manifest.json",
  "@type": "sc:Manifest",
  "attribution": "Heidelberger Akademie der Wissenschaften / Epigraphische Datenbank Heidelberg",
  "description": "Image(s) taken from the Epigraphic Database Heidelberg",
  "label": "EDH Image F002818",
  "license": "https://www.deutsche-digitale-bibliothek.de/content/lizenzen/rv-fz",
  "metadata": [
    {
      "label": "Provinz / Italische Region",
      "value": "Pannonia superior"
    },
    {
      "label": "Land",
      "value": "Austria"
    },
    {
      "label": "Fundort antik",
      "value": "Gerulata, bei"
    },
    {
      "label": "Fundort modern",
      "value": "Zurndorf"
    },
    {
      "label": "Aufbewahrung",
      "value": "Mosonmagyaróvár, Hansági Múz."
    }
  ],
  "sequences": [
    {
      "@type": "sc:Sequence",
      "canvases": [
        {
          "@id": "https://edh.ub.uni-heidelberg.de/iiif/edh/canvas/F002818",
          "@type": "sc:Canvas",
          "height": 1573,
          "images": [
            {
              "@context": "http://iiif.io/api/presentation/2/context.json",
              "@id": "https://edh.ub.uni-heidelberg.de/iiif/edh/annotation/F002818",
              "@type": "oa:Annotation",
              "motivation": "sc:painting",
              "on": "https://edh.ub.uni-heidelberg.de/iiif/edh/canvas/F002818",
              "resource": {
                "@id": "https://edh.ub.uni-heidelberg.de/iiif/edh/resource/F002818",
                "@type": "dctypes:Image",
                "format": "image/png",
                "height": 1573,
                "service": {
                  "@context": "http://iiif.io/api/image/2/context.json",
                  "@id": "https://heidicon.ub.uni-heidelberg.de/iiif/2/1415590%3A763891",
                  "profile": "http://iiif.io/api/image/2/level2.json"
                },
                "width": 982
              }
            }
          ],
          "label": "F002818",
          "metadata": [
            {
              "label": "Foto ID",
              "value": "https://edh.ub.uni-heidelberg.de/edh/foto/F002818"
            },
            {
              "label": "Photo credits",
              "value": "© G. Alföldy"
            }
          ],
          "width": 982
        }
      ],
      "label": "EDH Sequence"
    }
  ]
}

