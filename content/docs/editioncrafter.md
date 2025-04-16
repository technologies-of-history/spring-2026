---
draft: false
type: docs
weight: 3
title: EditionCrafter
---

Playing around with embedding an EditionCrafter viewer in my site.

<html>
<div id="ec"></div>

 <script type="text/javascript" src="https://www.unpkg.com/@cu-mkp/editioncrafter-umd" ></script>

 <script type="text/javascript">

     EditionCrafter.viewer({
         id: 'ec',
         documentName: 'Trinity College Cambridge MS O.8.35',
         iiifManifest='https://github.com/technologies-of-history/spring-2026/dyngley/iiif/manifest.json',
         transcriptionTypes: {
           text: 'Transcription'
         }
     });

 </script>
