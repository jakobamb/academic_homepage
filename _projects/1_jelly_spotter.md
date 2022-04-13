---
layout: page
title: Jelly Spotter App
description: A citizen science application to support jellyfish population research
img: assets/img/projects/logo_gojelly.png
importance: 1
category: work
---

To support jellyfish research in the EU Horizon 2020 funded project [GoJelly](https://gojelly.eu/), I teamed up with a fellow student to implement a cross-platform citizen science application to track jellyfish sightings submitted by volunteers around the baltic sea. The application was developed under the supervision of Professor Dr. Jamileh Javid Pour from the University of Southern Denmark (SDU), Department of Biology.

[Jelly Spotter App on the App Store (Apple iOS)](https://apps.apple.com/de/app/gojelly/id1498675707?l=en&platform=iphone)

[Jelly Spotter App for the browser (All Devices)](https://jelly-spotter.web.app/)

<!-- <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/1.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/3.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/5.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div> -->
<!-- <div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div> -->

<br />
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/projects/gojelly_appstore.png title: "App Store page" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Screenshot of the <a href="https://apps.apple.com/de/app/gojelly/id1498675707?l=en&platform=iphone">App Store page</a>
</div>

The jellyfish sightings are used by scientists to enable modelling and prediction of jellyfish bloom in the future. For example, this will enable swimmers in the baltic region to be warned about the stinging lion's mane jellyfish. Warnings and jellyfish forecasts are planned to be added to the Jelly Spotter App in the future.
In the first season of launching the app, we have registered over 600 jellyfish sightings, most of which were submitted with a picture of the jellyfish.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% responsive_image path: assets/img/projects/lions_mane_jellyfish.jpg title: "Lion's mane jellyfish" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Lion's mane jellyfish. Image by W. Carter, CC0 (<a href="https://en.wikipedia.org/wiki/Lion%27s_mane_jellyfish#/media/File:Lion's_mane_jellyfish_in_Gullmarn_fjord_at_S%C3%A4mstad_3.jpg">Source</a>)
</div>

## Jelly Spotter App in the Media

We are proud that major German media reported about the Jelly Spotter App :) Here are some example articles (in German):

[[DLF Nova] Quallenplage: Sie werden mehr und sollen bald vorhersagbar sein](https://www.deutschlandfunknova.de/beitrag/ostsee-quallen-breiten-sich-aus-sind-aber-kaum-vorhersehbar)

[[Galileo] Der große Glibber: Quallen erobern die Weltmeere](https://www.galileo.tv/natur/quallen-in-der-ostsee-ausbreitung-gefaehrlich-oder-nicht-fuer-den-klimawandel/)

[[MOPO] Quallen-Ärger in der Ostsee: Eine App soll jetzt helfen](https://www.mopo.de/im-norden/schleswig-holstein/quallen-aerger-in-der-ostsee-eine-app-soll-jetzt-helfen/)

[[NDR] Quallen in der Ostsee: Vorhersagen bald möglich](https://www.ndr.de/nachrichten/schleswig-holstein/Quallen-in-der-Ostsee-Vorhersagen-bald-moeglich,quallen216.html)

[[RTL] Diese App soll Quallen vorhersagen](https://www.rtl.de/cms/diese-app-soll-quallen-vorhersagen-4793626.html)

[[Zeit Online] Forscher arbeiten an Quallen-Vorhersage-App](https://www.zeit.de/news/2021-07/11/forscher-arbeiten-an-quallen-vorhersage-app?utm_referrer=https%3A%2F%2Fwww.google.com%2F)

## Implementation

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/projects/webapp_screenshot.png title: "Webapp Screenshot" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Screenshot of the <a href="https://jelly-spotter.web.app/">web application</a>
</div>


The Jelly Spotter App was developed cross-plattform for the web, with native applications for Apples iOS and iPad OS. We used [Google Firebase](https://firebase.google.com/) for a simple 'serverless' backend for both versions. The web application was developed as a responsive, single-page application using [React.js](https://firebase.google.com/) and TypeScript. For displaying the map on the web version, we used the [Mapbox API](https://www.mapbox.com/).